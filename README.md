<DOCTYPE html>
<html>
  <head>
<title>WebInfo</title>
<meta charset="Utf-8">
<link rel="stylesheet" href="WebInfo.css">
  </head>
   <body>
    <header>

      <div id="logo" onclick="slowScroll('#top')">
        <span>WebInfo</span>
      </div>

      <div id="about">
        <a href="#" title="Возможности" onclick="slowScroll('#main')">Что это?</a>
        <a href="#" onclick="slowScroll('#overview')" title="Преимущества">Что изучать?</a>
        <a href="https://vk.com/slishkom_sladki" target="_blank" title="Контакты">Контакты</a>
      </div>

    </header>


    <div id="top">
      <h1>Web Программирование</h1>
      <h3>Основные сведения</h3>
    </div>

    <div id="main">

      <div class="intro">
        <h2>Что это ?</h2>
        <span></span>
      </div>

      <div class="text">
        <span><strong>Веб-разработка </strong>— процесс создания веб-сайта или веб-приложения. Основными этапами процесса являются веб-дизайн, вёрстка страниц, программирование для веб на стороне клиента и сервера, а также конфигурирование веб-сервера.</span>
      </div>

    </div>


    <div id="overview">
      <h2>Что учить ?</h2>
      <h4>Основные вещи , которые обязательно понадобятся:</h4>

      <div class="img">
        <img src="https://s3.tproger.ru/uploads/2018/08/html-770x270.jpg">
        <span>Изучение HTML</span>
      </div>

      <div class="img">
        <img src="https://seodiz.ru/wp-content/uploads/2011/06/1_qg3ot-9cer8nt-p7kr3ypw.jpg">
        <span>Изучение CSS</span>
      </div>

      <div class="img">
        <img src="https://media.proglib.io/wp-uploads/2018/11/1_hLSiwh3HW9Pqw0M3gLEMOg.png">
        <span>Изучение JS</span>
      </div>

      <div class="img">
        <img src="https://freesoft.ru/storage/images/news/3/23/2222/2222_text.png">
        <span>Изучение Photoshop</span>
      </div>

    </div>

    
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    <script>
      function slowScroll(id) {
        $('html , body').animate({
          scrollTop: $(id).offset().top
        },500);
      } 

      $(document).on("scroll", function() {
        if($(window).scrollTop() === 0)
        $("header").revomeClass("fixed");
        else
        $("header").attr("class" , "fixed");
      });

    </script>
  </body>
</html>
