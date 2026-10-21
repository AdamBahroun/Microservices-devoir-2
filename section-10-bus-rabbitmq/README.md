# Section 10 : Spring Cloud Bus, RabbitMQ et Config Monitor

Lancement : copier .env.example en .env et renseigner les valeurs, puis docker compose up --build -d.

Ecarts par rapport au PDF :
- RabbitMQ est lance via docker-compose (hote rabbitmq dans les conteneurs au lieu de localhost).
- busrefresh est appele en POST (curl), pas depuis le navigateur.
- spring.cloud.refresh.never-refreshable ajoute (SPRING_CLOUD_REFRESH_NEVER_REFRESHABLE) : sans cela, le client Eureka plantait apres un refresh avec ces versions de Spring Cloud.
- Le Config Monitor (/monitor) a ete teste avec Postman.
