# TestAuth for [vk.com](https://vk.com) without Backend
## Tasks
Сделать веб приложение, на выбранном вами языке, при открытии должно показать кнопку «авторизоваться» по нажатию делает oauth авторизацию ВКонтакте, и показывает имя авторизованного пользователя и 5 любых друзей пользователя. При последующих запусках/заходах на страницу сразу показывает всю информацию т.к. уже понимает, что авторизовано и авторизация запоминается. Бекенд если потребуется, на любой технологии на ваш выбор. 

#### How does it work?
1. show the #btn auth
2. click on the #btn
3. Redirect to this.window
4. Parse the location.hash (#access_token=)
5. write token in the localStorage
6. Send Ajax to api.vk.com
7. Data render

### Install
1. Clone the repo
2. Change URL in the #btn : [How to build the URL?](https://vk.com/dev/first_guide?f=3.%20%D0%90%D0%B2%D1%82%D0%BE%D1%80%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F)
```html
<a role="button" href="https://oauth.vk.com/authorize?client_id=ТВОЙ_ID_ПРИЛОЖЕНИЯ&redirect_uri=ТВОЯ_ССЫЛКА&scope=friends&response_type=token&v=5.52" id="btn">
  Авторизоваться
</a>
```
