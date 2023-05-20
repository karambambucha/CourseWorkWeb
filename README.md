##

Установите npm

Установите bower npm

	npm install -g bower
Установите polymer через bower

	bower install --save Polymer/polymer#^1.1.0
Подключите image-gallery, добавив в < head >

	<script src="bower_components/webcomponentsjs/webcomponents.js"></script>

	<link rel="import" href="bower_components/polymer/polymer.html">

	<link rel="import" href="simple-gallery.html">

Шаблон для добавления галереи:

    <image-gallery>
        <img data-original="путь к оригинальному изображению" data-description="описание 1" data-index='s1' on-click="load_popup" src="путь к миниатюре" alt="Картинка 1"> 
        <img data-original="путь к оригинальному изображению" data-description="описание 2" data-index='s2' on-click="load_popup" src="путь к миниатюре" alt="Картинка 2">
        <img data-original="путь к оригинальному изображению" data-description="описание 3" data-index='s3' on-click="load_popup" src="путь к миниатюре" alt="Картинка 3"> 
    </image-gallery>

Не забудьте указать правильные пути к оригинальному изображению и к миниатюрам. Описание не обязательно.

Индексы (data-index) пишутся строго в формате 's##', где ## - число, и строго в порядке возрастания. 