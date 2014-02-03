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
 
   <h1>Border Özellikleri</h1>
   


----------
 Turmix içinde kodlamayı hızlandıracak çeşitli kullanımı kolay border mixinleri barındırır. 
 
 <h3>Temel Border</h3>
  
  Temel border özellikleri **br;** mixini tarafından sağlanmaktadır. 
  

    #box{
     width:100px;
     height:100px;
     .br; 
    }
> Yukarıdaki kodu çalıştırdığımızda <a href="http://img202.imageshack.us/img202/2453/c5wc.png">link</a>tekine benzer bir görüntü çıkaracaktır.

  Tabiki temel border mixinimizde çeşitli düzenlemelerimizi yapabiliyoruz. Parametrelerimiz ise şunlar:
  
  

 >  **.br(renk,boyut,tip);**
    
    #box{
    width:100px;
    height:100px;
    .br(@f-pum,3px,dotted);
    }
    
> Yukarıdaki kodu çalıştırdığımızda ise şuna benzer bir görüntü verecektir. <a href="http://img37.imageshack.us/img37/7372/2mg6.png">Link</a>
>> **NOT:** @f-pum değişkeni kütüphaneye dahil olan flat bir rengin değişkenidir.


----------
 <h3>2D Border</h3>
 
 2D border özelliği **.br-2d;** mixini ile sağlanır. Uygulandığı nesneye aslında basit bir şekilde 3D efekti uygular.Varsayılan renkleri **#ddd** ve **#bbb** 'dir.
 
 

    #box{
    width:200px;
    height:200px;
    .br-2d;
    }
> Yukarıdaki kod bize şu çıktıyı verecektir. <a href="http://i.imgur.com/EGLqAOy.png">Link</a>

Bu basit efektin mantığında iki koyu border, iki açık border vardır. Bu mixinide parametrelerle kendinize göre özelleştirebilirsiniz. Parametreler:   
>**.br-2d(koyurenk , acikrenk);**

    #box{
    width:300px;
    height:300px;
    .br-2d();
    }
