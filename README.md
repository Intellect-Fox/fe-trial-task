# Задание пробного занятия

### По инструкции у вас должна получиться такая страница:
![screen](https://res.cloudinary.com/intellectfox/image/upload/v1605010329/samples/fe-trial_xdagjw.gif)

## Описание
Страница состоит из трёх основных секций:
- верхняя секция;
- секция со списком проектов в виде шести плиток;
- футер (нижняя секция) со списком ссылок на наши социальные сети.

## Инструкция
1. Скачайте и установите редактор кода [VS Code](https://code.visualstudio.com). В нем вы будете писать код.
2. Создайте на вашем компьютере папку с именем `if-trial-task`.
3. Откройте VS Code и перетяните в него папку `if-trial-task`.
4. Создайте новый файл с именем `index.html` так, как это показано на изображениях ниже:
    ![screen-1](https://res.cloudinary.com/intellectfox/image/upload/v1605001743/samples/fe-trial-1_c2keb9.png)
    ![screen-2](https://res.cloudinary.com/intellectfox/image/upload/v1605001742/samples/fe-trial-2_jpgwtg.png)
5. Содайте таким же образом файл `style.css`.
6. Выберите файл `index.html`, введите `!` и нажмите клавишу `tab`. В итоге у вас получится такой код:
    ![screen-3](https://res.cloudinary.com/intellectfox/image/upload/v1605002081/samples/fe-trial-3_ipenlq.png)
7. Для того, чтобы сделать верхнюю секцию, для начала вам нужно вставить в `body` (между `<body>` и `</body>`) следующий html-код:
    ```html
    <section class="top-section">
      <div class="container">
        <h1>Hey👋</h1>
        <h4>I’m Intellect Fox.</h4>
        <img src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/fox_l7tdkz.png" alt="Fox">
      </div>
    </section>
    ```
8. Сохраните полученный результат (ctrl+s или cmd+s)
9. Откройте на вашем компьютере папку `if-trial-task`, нажмите правой клавишей мыши на файл `index.html` и выберите "Открыть с помощью -> Google Chrome". Если Google Chrome не установлен, вы можете открыть файл в другом браузере или установить Google Chrome на ваш компьютер. У вас должен получиться такой результат:
    ![screen-4](https://res.cloudinary.com/intellectfox/image/upload/v1605003943/samples/fe-trial-4_wktofo.png)
10. Согласитесь, что результат не такой, как можно увидеть на гиф-изображении выше. Для того, чтобы результат получился таким, как мы задумали, вам нужно добавить стили в файл `style.css` и подключить их к html-файлу. Перейдите в файл `style.css` и вставьте в него css-код, который задает стили основным элементам и верхней секции:
    ```css
    @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;1,400;1,500&display=swap');
    
    * {
      margin: 0;
      box-sizing: border-box;
      font-weight: 500;
    }
    
    body {
      font-family: 'Roboto', sans-serif;
      color: #333333;
      text-align: center;
    }
    
    h1 {
      font-size: 104px;
      color: #ffffff;
      margin-bottom: 40px;
    }
    
    h2 {
      font-size: 80px;
      color: #ffffff;
      margin-bottom: 80px;
    }
    
    h3 {
      font-size: 56px;
      margin-bottom: 100px;
    }
    
    h4, .h4 {
      display: block;
      font-size: 48px;
      color: #a14c4c;
      margin-bottom: 64px;
    }
    
    p {
      font-weight: 400;
    }
    
    .container {
      max-width: 1234px;
      margin: 0 auto;
      padding: 120px 16px;
    }
    
    .row {
      display: flex;
      margin: 48px -8px;
    }
    
    .col {
      width: 33.3333%;
      padding: 0 8px;
    }
    
    .top-section {
      display: flex;
      align-items: center;
      min-height: 100vh;
      background-color: #333333;
    }
    ```
11. Сохраните полученный результат (ctrl+s или cmd+s). Код должен выглядеть так:
    ![screen-5](https://res.cloudinary.com/intellectfox/image/upload/v1605006363/samples/fe-trial-5_d3qzbj.gif)
12. Перейдите в файл `index.html` и в `head`, после тега `title` подключите стили добавив следующую строку:
    ```html
    <link rel="stylesheet" href="./style.css">
    ```
    Код должен выглядеть так:
    ![screen-6](https://res.cloudinary.com/intellectfox/image/upload/v1605006613/samples/fe-trial-6_r1hoan.png)
13. Сохраните полученный результат (ctrl+s или cmd+s), перейдите в браузер и обновите страницу (F5 или cmd+r). Результат должен быть следующим:
    ![screen-7](https://res.cloudinary.com/intellectfox/image/upload/v1605006697/samples/fe-trial-7_kctjkg.png)
14. Приступим к секции со списком проектов, которые вы можете научиться делать, обучаясь в Intellect Fox. Добавьте перед закрывающим тегом `body` (`</body>`) следующий код:
    ```html
    <section class="projects">
      <div class="container">
        <h3 class=>These are projects which you will develop</h3>
        <div class="row">
          <div class="col">
            <div class="project">
              <img class="project__image" src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/foxtube_xwx0nd.png" alt="FoxTube">
              <h3 class="project__title">FoxTube</h3>
              <p class="project__description">Online video-sharing platform</p>
            </div>
          </div>
          <div class="col">
            <div class="project">
              <img class="project__image" src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/foxmusic_fgo7su.png" alt="Fox Music">
              <h3 class="project__title">Fox Music</h3>
              <p class="project__description">Music streaming service</p>
            </div>
          </div>
          <div class="col">
            <div class="project">
              <img class="project__image" src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/foxlibrary_lhzodm.png" alt="Fox Library">
              <h3 class="project__title">Fox Library</h3>
              <p class="project__description">Ebook service</p>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col">
            <div class="project">
              <img class="project__image" src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/foxexpress_y4suil.png" alt="FoxExpress">
              <h3 class="project__title">FoxExpress</h3>
              <p class="project__description">Online shop</p>
            </div>
          </div>
          <div class="col">
            <div class="project">
              <img class="project__image" src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/foxdelivery_ufgvuc.png" alt="Fox Delivery">
              <h3 class="project__title">Fox Delivery</h3>
              <p class="project__description">Food delivery service</p>
            </div>
          </div>
          <div class="col">
            <div class="project">
              <img class="project__image" src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/foxmatch_kkyr0x.png" alt="Fox Match">
              <h3 class="project__title">Fox Match</h3>
              <p class="project__description">Memory matching game</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    ```
15. Сохраните полученный результат (ctrl+s или cmd+s), перейдите в браузер и обновите страницу (F5 или cmd+r). Секция будет выглядеть так:
    ![screen-8](https://res.cloudinary.com/intellectfox/image/upload/v1605007199/samples/fe-trial-8_f0uhz6.png)
16. Секция со списком проектов выглядит не так, как показано на гиф-изображении выше. Для того, чтобы результат получился таким, как мы задумали, вам нужно добавить стили в файл `style.css` ниже тех, которые вы уже добавили:
    ```css
    .project {
      color: #ffffff;
      background-color: #333333;
    }
    
    .project__image {
      width: 100px;
      height: 100px;
      object-fit: contain;
      margin: 100px 0 78px;
    }
    
    .project__title {
      margin-bottom: 56px;
    }
    
    .project__description {
      padding: 18px 0;
      color: #a14c4c;
      border-top: 1px solid;
    }
    ```
17. Сохраните полученный результат (ctrl+s или cmd+s), перейдите в браузер и обновите страницу (F5 или cmd+r). Теперь секция будет выглядеть так:
    ![screen-9](https://res.cloudinary.com/intellectfox/image/upload/v1605007607/samples/fe-trial-9_qqqbyp.png)
18. Остался футер. Добавьте перед закрывающим тегом `body` (`</body>`) следующий код:
    ```html
    <footer class="footer">
      <div class="container">
        <h2>Let’s study together🤗</h2>
        <i class="h4">Follow us</i>
        <div class="social">
          <a href="https://www.facebook.com/intellectfoxby" class="social_link" target="_blank">
            <img src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/facebook_u3us5v.png" alt="Facebook">
          </a>
          <a href="https://vk.com/intellectfox" class="social_link" target="_blank">
            <img src="https://res.cloudinary.com/intellectfox/image/upload/v1605002398/fe/trial-task/vk_cxp8nx.png" alt="VK">
          </a>
          <a href="https://www.instagram.com/intellectfox/" class="social_link" target="_blank">
            <img src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/instagram_uaiggn.png" alt="Instagram">
          </a>
          <a href="https://www.linkedin.com/company/intellect-fox" class="social_link" target="_blank">
            <img src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/linkedin_ezy8wr.png" alt="LinkedIn">
          </a>
          <a href="https://t.me/pro_it_world" class="social_link" target="_blank">
            <img src="https://res.cloudinary.com/intellectfox/image/upload/v1605002397/fe/trial-task/telegram_rhvgh3.png" alt="Telegram">
          </a>
        </div>
      </div>
    </footer>
    ```
19. Сохраните полученный результат (ctrl+s или cmd+s), перейдите в браузер и обновите страницу (F5 или cmd+r). Футер будет выглядеть так:
    ![screen-10](https://res.cloudinary.com/intellectfox/image/upload/v1605008563/samples/fe-trial-10_rkcq6f.png)
20. Осталось добавить стили для футера. Добавьте следующие стили в файл `style.css` ниже тех, которые вы уже добавили:
    ```css
    .footer {
      background-color: #333333;
    }
    
    .social {
      display: flex;
      justify-content: center;
    }
    
    .social_link {
      margin: 0 32px;
    }
    ```
21. Сохраните полученный результат (ctrl+s или cmd+s), перейдите в браузер и обновите страницу (F5 или cmd+r). Ура! У вас всё получилось, наслаждайтесь готовым результатом:
    ![screen-11](https://res.cloudinary.com/intellectfox/image/upload/v1605010329/samples/fe-trial_xdagjw.gif)
22. Для того, чтобы получить обратную связь по вашему заданию, [отправьте](https://forms.gle/TqwgFu1dXf2TjraLA) файлы `index.html` и `style.css`, которые находятся в вашей папке `if-trial-task`. Мы дадим обратную связь в течение 2 дней.

## Поздравляем 🥳
P.S.: Страница, которую вы сделали, является самым простым примером. В реальности код не пишется копипастом. Более интересные проекты вы сможете сделать на нашем курсе.

Старт занятий — 9 февраля. Записаться можно по ссылке — https://intellectfox.by/. И не забывайте про ваш промокод `trial-fe-3`.