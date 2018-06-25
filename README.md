# GoruntuIslemeliMobilRobot
 Teknolojinin her geçen gün gelişmesiyle mobil robot araştırmaları ve yapılan çalışmalar mobil robotların hayatımızda ki yerini giderek arttırmıştır. 
 Eğitim, sanayi, endüstri, sağlık ve günlük yaşamda birçok uygulamada mobil robotlar vazgeçilmez hale gelmiştir.
  Bu projede görme tabanlı, düzgün yüzeylerde kablosuz olarak hareket edebilen, robotun mekaniğinin basit, kontrolünün kolay olması ve gözlem, keşif gibi uygulamalarda kullanılabilecek özelliklere sahip olması hedeflenmiştir. 
  Projede mikrodenetleyici olarak raspberry pi kullanılıp nesneleri algılaması kamera aracılığı ile yapılmıştır.
  Kameradan alınan görüntüler, OpenCV görüntü işleme kütüphanesi kullanılarak işlenmiştir.
   OpenCV ile görüntü işleme yapılırken öncelikle kamera aygıtından alınan görüntü üzerinde belirlenen bazı renkler tespit edilerek bu renge sahip objeler bulunmuştur.
   Öncelikle bir renk aralığı belirlenmelidir. 
   Daha sonra kamera aygıtından yakalanan RGB renk uzayına sahip görüntüyü HSV renk uzayına çevrilmelidir. Görüntü üzerinde eşikleme, aşındırma ve genişletme gibi görüntü işleme teknikleri kullanılır. Kenar bulma gibi metotları kullanarak renklerin ayrımını tespit edip nesneler işaretlenir.          Renk tespiti için HSV uzayı kullanılmalıdır çünkü RGB renk uzayında yapılacak olan threshold HSV renk uzayında yapılacak threshold’a göre yetersizdir. 
   HSV de H (HUE) değeri daha ayırt edilebilir şekilde değiştiği için farklı renkli objelerin resimde tespiti çok daha kolay olmaktadır. 
