# Требования
1. Регистрация новых учетных записей по вводу email и пароля
  - Пароль должен быть зашифрован
  - Email должен быть уникальный
2. Авторизация пользователей
  - Роли авторизированых пользователей
    * Пользователь - имеет доступ только к основному функционалу веб приложения перечисленного в пунктах 5
    * Модератор - имеет доступ к основному функционалу веб приложения перечисленного в пунктах 5, а также имеет админ меню, подробней в            пункте 3
3. Админ меню
  -  Доступ к админ меню есть только у модератора
  -  Должна быть возможность для редактирования/удаления/создания всех сущностей из пункта 4
  -  Должна быть возможность назначить модератора
  -  Должна быть возможность убрать роль модератора
4. Основные сущность и их функции
  - Блюдо
    * Состоит из продуктов и компонентов
    * Имеет рейтинг
    * Новое блюдо может создать только модератор
  - Продукт
    * Состоит из компонентов
    * Имеет рейтинг
    * Имеет 'вес', который влияет на на рейтинг по формуле рейтинг += вес_продукта*(-1||1)
    * Новый продукт может создать только модератор
  - Компонент
    * Имеет рейтинг
    * Имеет 'вес', который влияет на на рейтинг по формуле рейтинг += вес_компонента*(-1||1)
    * Новый компонент может создать только модератор
  - Пользователь
    * Хранит все голоса, которые он отдал за блюда
    * Имеет предпочтения в блюдах
    * Содержит email, пароль, логин
    * Основные взаимодействия с программным продуктом перечислены в пункте 5.
  - Голос
    * Аккумулирует только 2 состояния 1(лайк), -1(дизлайк)
    * Связан с блюдом
    * Связан с пользователем
5. Основное вззаимодействие пользователем с программным продуктом
  * Пользователь может проголосовать за блюдо(лайк, дизлайк)
  * Пользователю выведен список всех блюд
  * Список блюд отсортирован по рейтингу от большего с меньшему
  * Список перестраивается каждый раз при голосовании
  * Пользователь может отредактировать свой профиль(nickname, фото)
  * Пользователь может подробней посмотреть о каждом блюде(рецепт, фото, ккларий и т.д.)
6. Требования к функционалу
  * Предпочтения должны быть основаны на рейтинги блюд для каждого пользователя
  * Нужно, на основе выбраных пользователем любимых компонентов, находить пользователей с такимиже вкусовыми предпочтениями, для определния возможного блюда, которое может понравиться пользователю
  * Разработать возможность формирования 'диет'
7. Требовния к дизайну программного продукта
  * Дизайн должен быть выполнен в светлых тонах, с включеним салатогого цвета
  * Дизайн должен быть корректно отображаться на всех видах устройств
  * Дизайн должен быть интуитивно понятным
  * Дизайн должен быть выполнен в стили минимализм
8. Требования к тестированиям
  * Тестированием должно быть покртыты весь функционал из пункта 6
9. Исполнитель должен запустить тестовую версию не познее 01.01.2020 

