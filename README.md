# Тема для сайта [shikimori.org](https://shikimori.org)
Данная тема предназначена для облагораживания сайта. Затрагивается каждая страница, практически каждый элемент. Наиболее интересна эта тема будет владельцам широкоформатных мониторов с разрешением 1920x1080px и более, а также владельцам мобильных телефонов под управлением Android с разрешением 360x640px и более. Тема настроена таким образом, что устройства с разрешением менее 320px не считаются подходящими – на таких устройствах будут отключаться лишние картинки, кнопки и прочее оформление.

## Установка
Для большинства пользователей предполагается установка готового стиля с его последующей ручной настройкой. Список готовых стилей:
* [Светлая тема](../master/beta/theme-light.css)
* [Светлая тема + Обложка](../master/beta/theme-light-cover.css)
* [Темная тема](../master/beta/theme-dark.css)
* [Темная тема + Обложка](../master/beta/theme-dark-cover.css)

Выберите подходящий вам готовый вариант, скопируйте исходный код в настройки вашего профиля. Все свои настройки указывайте в конце стиля в разделе "Мои настройки":
```css
/* МОИ НАСТРОЙКИ */

/* Фон меню */
.l-top_menu:before {
  background-color: #212121;
}
```

#### Установка обложки
Чтобы обложка отображалась в вашем профиле, замените все вхождения `2727` на ваш ID. Вы можете воспользоваться поиском по странице (сочетание клавиш `Ctrl+F` или `Command+F`). Чтобы узнать свой ID, скачайте свою аватарку: цифры в названии файла – это ваш ID. Ссылка на изображение указывается в самом конце файла:
```css
/* Моя обложка в профиле */
.p-profiles .profile-head[data-user-id = "2727"] .c-brief:before {
  background-image: url(); /* Моя обложка */
  background-position: center;
}
```

## Расширенная установка
Если вы хотите установить тему, используя свои цвета для оформления сайта, вам следует использовать расширенную установку вместо исправления цветов в готовых стилях. Старайтесь придерживаться следующей структуры стиля при сборке своей темы:

###### Структура стиля
1. Копирайт
2. Шрифт Roboto ¹
3. Настройки цвета
4. Минифицированный стиль
5. Экспериментальные функции ¹
6. Обложка ¹
7. Дополнительные части ¹
8. Мои настройки

> ¹ Если необходимы.

###### Настройки цвета
Следующий файл содержит настройки почти всех цветов сайта, доступных для изменения с помощью переменных языка `Sass`:
> https://github.com/grin3671/shiki-theme/blob/master/custom/color.sass

Используйте сайт http://sassmeister.com, чтобы конвертировать `Sass` в `CSS`. В меню сайта "Options" смените синтаксис "Syntax" на `Sass`.

###### Прочее
Остальные части темы можно скопировать из готовой темы.

## Дополнения
Некоторые задумки, к сожалению, не включены в основную тему из-за неопределенного влияния на остальной дизайн или недостаточного тестирования, однако они могут быть весьма полезны и удобны при ежедневном использовании темы. Список:
* [Шрифт Roboto](../master/part/font-roboto.css)

    > Для темы больше подходит шрифт Roboto, однако это он может долго грузится на медленном интернете.
    

## Превью
Альбом со скриншотами темы: https://imgur.com/a/tc7uV

## Благодарности
В тестировании темы принимало участие большое количество пользователей, отзывы которых помогли довести дело до победного конца и сделать тему действительно приятной для использования. Большое вам спасибо!

### Поддержать проект
Поддержать создание темы можно сообщив о найденных ошибках и неточностях [автору](https://shikimori.org/grin3671), либо материально:

Яндекс.Деньги: `41001258665103`
