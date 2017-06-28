# Scissors2
如果想對圖片進行縮放+裁減

Scissors
https://github.com/lyft/scissors

使用方法:

1. 建立模組View, 任何放進來的圖片都可以任意縮放
  
![image](http://i.imgur.com/KkrDTjD.png)

2. compile 'com.lyft:scissors:1.1.1'
   目的是, 使用cropView 相關方法
   
3. 加載圖片到模組View
   cropView.setImageBitmap(bitmap1);
   
4. 把超出模組View的地方刪掉, 只保留View以內的
   並且取代原本的圖片
   bitmap2 = mCropView.crop();
   mCropView.setImageBitmap(bitmap2);

