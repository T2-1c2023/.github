# Taller 2 - FiuFit - 1c 2023

[Enunciado](https://taller-de-programacion-2.github.io/tasks/statement/2023/1/enunciado/)

FiuFit es una app de fitness diseñada para ayudar a atletas a descubrir nuevos entrenamientos, mantener un registro de metas propuestas, y socializar con otros atletas y entrenadores.

## Arquitectura general

![Diagrama de microservicios](./docs/images/microservice-diagram.jpg)

### Frontend

El frontend se basó en `React Native` para su parte mobile, y `React` para el desarrollo de la página web de backoffice. A su vez, el API Gateway fue desarrollado en `Node.js`.

Documentación de cada componente:

 - [App Mobile](https://github.com/T2-1c2023/AppMobile/blob/master/README.md)
 - [App Mobile - Guía de usuario](http://scapelli.ar/MobileAppGuide/)
 - [Backoffice Web](https://github.com/T2-1c2023/WebAdmin/blob/main/README.md)
 - [API Gateway](https://github.com/T2-1c2023/APIGatewayService/blob/main/README.md)

### Backend

El backend fue desarrollado en `Node.js` (microservicios de Usuarios y Entrenamientos), y `Golang` (microservicios de Recomendaciones y Notificaciones). Para los microservicios de Usuarios y Entrenamientos, se utilizó `PostgreSQL` como base de datos, mientras que en el microservicio de Recomendaciones se utilizó `MongoDB`.

Para conseguir métricas de uso de la aplicación y mostrarlas en el Backoffice, se utilizó `Datadog`. Mientras que tanto para subir fotos y videos, como para administrar el login federado con Google Sign-in se utilizó `Firebase`.

Documentación de cada componente:

 - [Trainings Service](https://github.com/T2-1c2023/TrainingsService/blob/main/README.md)
 - [Users Service](https://github.com/T2-1c2023/UsersService/blob/main/README.md)
 - [Recommendation Service](https://github.com/T2-1c2023/RecommendationService/blob/main/README.md)
 - [Notifications Service](https://github.com/T2-1c2023/NotificationsService/blob/main/README.md)
