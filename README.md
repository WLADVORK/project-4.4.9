# project-4.4.9

<!-- РЕГИСТРАЦИЯ --> 
<!-- Реквест --> 
POST https://blog.kata.academy/api/users
{
  "user": {
    "username": "NewKataUser2222",
    "email": "NewKataUser2222@mail.ru",
    "password": "12345"
  }
}
<!-- Реcпонс -->
200 OK
{
    "user": {
        "username": "newkatauser2222",
        "email": "newkatauser2222@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY2MjhmNzdiOGM4MjhkMWIwMDM5NjY2NCIsInVzZXJuYW1lIjoibmV3a2F0YXVzZXIyMjIyIiwiZXhwIjoxNzE5MTQ0ODI3LCJpYXQiOjE3MTM5NjA4Mjd9.HyW06QEiuL1osyCTSJBc1N2zY2l7rDsAsYPVVeEapdA"
    }
}
<!-- АВТОРИЗАЦИЯ --> 
<!-- Реквест --> 
POST https://blog.kata.academy/api/users/login
{
  "user": {
    "email": "newkatauser2222@mail.ru",
    "password": "12345"
  }
}
<!-- Реcпонс --> 
200 OK
{
    "user": {
        "username": "newkatauser2222",
        "email": "newkatauser2222@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY2MjhmNzdiOGM4MjhkMWIwMDM5NjY2NCIsInVzZXJuYW1lIjoibmV3a2F0YXVzZXIyMjIyIiwiZXhwIjoxNzE5MTQ1MDgyLCJpYXQiOjE3MTM5NjEwODJ9.iNuBTijyPomzy_w6VBvcfYsdKBOjrN7aRg-4quzThNQ"
    }
}
<!-- ПОЛУЧЕНИЕ ДАННЫХ О ПОЛЬЗОВАТЕЛЕ --> 
<!-- Реквест --> 
GET https://blog.kata.academy/api/user
token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY2MjhmNzdiOGM4MjhkMWIwMDM5NjY2NCIsInVzZXJuYW1lIjoibmV3a2F0YXVzZXIyMjIyIiwiZXhwIjoxNzE5MTQ0ODI3LCJpYXQiOjE3MTM5NjA4Mjd9.HyW06QEiuL1osyCTSJBc1N2zY2l7rDsAsYPVVeEapdA
<!-- Реcпонс --> 
200 OK
{
    "user": {
        "username": "newkatauser2222",
        "email": "newkatauser2222@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY2MjhmNzdiOGM4MjhkMWIwMDM5NjY2NCIsInVzZXJuYW1lIjoibmV3a2F0YXVzZXIyMjIyIiwiZXhwIjoxNzE5MTQ1MjA1LCJpYXQiOjE3MTM5NjEyMDV9.Cf7rbNRRYwOI0aMCqQVHisgJ6Ot7etPtV0dsz7gpqAU"
    }
}
