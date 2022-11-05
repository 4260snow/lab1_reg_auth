# Лаборатоная работа 1
## Цель
Спроектировать и разработать систему авторизации пользователей на протоколе HTTP
## Ход работы
* Разработаем пользовательский интерфейс и опишем пользовательские сценарии работы

![Рис. 1 - Интерфейс](https://github.com/4260snow/lab1_reg_auth/blob/main/ui.drawio.png)

* Описание clien-server
    * Правильная регистрация

        ![Рис. 2 - client-server](https://github.com/4260snow/lab1_reg_auth/blob/main/std_reg.png)

* Структура базы данных (json)

    | Название         | Описание                              |
    |------------------|---------------------------------------|
    | LOGIN            | Логин пользователя                    |
    | PASSWORD         | Хеш пароля с солью                    |
    | PASSWORD_EXP_DATE| Дата истечения пароля                 |

* Алгоритмы

    * Регистрирация (reg.php)
 
    ![](https://github.com/4260snow/lab1_reg_auth/blob/main/reg_bd.drawio.png)
  
    * Вход в аккаунт (login.php)
  
    ![](https://github.com/4260snow/lab1_reg_auth/blob/main/login_bd.drawio.png)
  
    * Выход из аккаунта (exit.php ДОБАВИТЬ ВЫХОД c удалением куки)
  
    ![](https://github.com/4260snow/lab1_reg_auth/blob/main/logout_bd.drawio.png)
  
    * Смена пароля, если он забыт (forgot_password.php сообщение, что пользователя не существует)
  
    ![](https://github.com/4260snow/lab1_reg_auth/blob/main/forgot_pwd_bd.drawio.png)
  
    * Новый пароль (изменение старого пароля) (change_password.php)
  
    ![](https://github.com/4260snow/lab1_reg_auth/blob/main/cng_pwd_bd.drawio.png)

