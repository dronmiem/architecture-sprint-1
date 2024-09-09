ЗАДАНИЕ № 1

Уровень 1. Проектирование
Выбирал фреймворк Module Federation.
Выбирал из Single SPA и Module Federation (наиболее хорошо освещенных в лекциях). Выбрал Module Federation, т.к. нет необходимости в разных стеках разработки. Ленивая загрузка есть в обоих фрейм ворках как и независимость разработки и развёртывания микрофронтендов. (Ну и наиболее понятно как с ним работать)

Уровень 2 Планирование изменений
для разбиения монолита выбрал стратегию вертикальной нарезки (Domain-Driven Design, DDD),
Обоснование: ярко выражены границы доменов , по анализу структуры использование DDD не выглядит проблематичным.

Разбиение будет сделано на хост и следующие микрофронтенды :

Авторизация. В нее войдут модули:
1.1. Авторизация
1.2. Выход

Профиль пользователя. В нее войдут модули:
2.1. Регистрация
2.1. Редактирование профиля

Работа с фото. В нее войдут модули:
3.1. Добавление, удаление, просмотр фото
3.2. Лайки карт

Структуры проектов
host - port 8080:
frontend\microfrontend\host\src\App.jsx
frontend\microfrontend\host\src\index.css
frontend\microfrontend\host\src\index.html
frontend\microfrontend\host\src\index.js
frontend\microfrontend\host\src\blocks\footer…
frontend\microfrontend\host\src\components\Footer.js
frontend\microfrontend\host\src\components\Header.js
frontend\microfrontend\host\src\images\logo.svg
frontend\microfrontend\host\src\vendor…

Микрофронтенд authorization - port 8081:
frontend\microfrontend\authorization\src\App.jsx
frontend\microfrontend\authorization\src\index.css
frontend\microfrontend\authorization\src\index.html
frontend\microfrontend\authorization\src\index.js
frontend\microfrontend\authorization\src\blocks\auth-form…
frontend\microfrontend\authorization\src\components\Login.js
frontend\microfrontend\authorization\src\contexts\CurrentUserContext.js
frontend\microfrontend\authorization\src\utils\auth.js

Микрофронтенд userProfile - port 8082:
frontend\microfrontend\userProfile\src\App.jsx
frontend\microfrontend\userProfile\src\index.css
frontend\microfrontend\userProfile\src\index.html
frontend\microfrontend\userProfile\src\index.js
frontend\microfrontend\userProfile\src\blocks\profile…
frontend\microfrontend\userProfile\src\components\EditAvatarPopup.js
frontend\microfrontend\userProfile\src\components\EditProfilePopup.js
frontend\microfrontend\userProfile\src\components\Register.js
frontend\microfrontend\userProfile\src\images\avatar.jpg
frontend\microfrontend\userProfile\src\utils\api.js

Микрофронтенд photo - port 8083:
frontend\microfrontend\photo\src\App.jsx
frontend\microfrontend\photo\src\index.css
frontend\microfrontend\photo\src\index.html
frontend\microfrontend\photo\src\index.js
frontend\microfrontend\photo\src\blocks\card…
frontend\microfrontend\photo\src\blocks\page…
frontend\microfrontend\photo\src\blocks\places…
frontend\microfrontend\photo\src\blocks\popup…
frontend\microfrontend\photo\src\components\AddPlacePopup.js
frontend\microfrontend\photo\src\components\Card.js
frontend\microfrontend\photo\src\components\ImagePopup.js
frontend\microfrontend\photo\src\components\InfoTooltip.js
frontend\microfrontend\photo\src\components\Main.js
frontend\microfrontend\photo\src\components\PopupWithForm.js
frontend\microfrontend\photo\src\components\ProtectedRoute.js
frontend\microfrontend\photo\src\images
frontend\microfrontend\photo\src\images\add-icon.svg
frontend\microfrontend\photo\src\images\card_1.jpg
frontend\microfrontend\photo\src\images\card_2.jpg
frontend\microfrontend\photo\src\images\card_3.jpg
frontend\microfrontend\photo\src\images\close.svg
frontend\microfrontend\photo\src\images\delete-icon.svg
frontend\microfrontend\photo\src\images\edit-icon.svg
frontend\microfrontend\photo\src\images\error-icon.svg
frontend\microfrontend\photo\src\images\like-active.svg
frontend\microfrontend\photo\src\images\like-inactive.svg
frontend\microfrontend\photo\src\images\success-icon.svg
frontend\microfrontend\photo\src\utils\api.js



ЗАДАНИЕ № 2
https://drive.google.com/file/d/1INSmIkMrrXFgngBrVydZDTm5rqdhlDzF/view?usp=sharing
так же положил в репозитории task2\Demyantsev_sprint1_task2.drawio