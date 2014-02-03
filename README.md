turmix-lesslibrary
==================

<h1> Sayfaya Dahil Etme </h1>


----------
 Kullandığınız ana stil dosyasına aşağıdaki kodu ekleyin.

 
 `@import url('turmix/turmix.less');`
     
   > Turmix'i farklı bir dizinde saklıyorsanız LESS dosyasının yolunu doğru belirttiğinizden emin oldun.


----------

 <h1>Renklerin Kullanımı</h1>
 


----------

 Turmix'in içine dahil olan renkler http://flatuicolors.com sitesinden alınmıştır. 
   
    #div{
         background-color: @f-ali;
         height:100px;
         width:100px;
        } 

 > Kullanım kuralı : @f global Flat renk değişkeni "-" ve rengin ilk üç harfi.
 
 ![@f-ali][1]

 [1]: http://i.imgur.com/WteG0bm.png 
 
 > Örneğin ALIZARIN rengi için <b>@f-ali</b> yazmak yeterli olacaktır. 
 > Ayrıca Apple iOS 7 işletim sisteminin arayüzünde sık miktarlarda kullanılan temel  *yeşil*  *mavi* ve *kırmızı* renkler ; <b>@ios-red</b> , <b>@ios-blue</b> ve   <b>@ios-green</b> olarak barındırılmaktadır.   
