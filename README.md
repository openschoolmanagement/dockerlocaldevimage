# Docker Image for local development

## Prerequistes
1. Install Docker (https://docs.docker.com/install/#supported-platforms)
2. Clone the Repo
3. Run 'docker-compose' in Terminal or Command Line

## Used Backing Services

1.  MySQL for the planned services Calendar, User, Contacts and Class Management
2.  RabbitMQ for Messaging
3.  Redis as Cache for Key Value Pairs.

## VCAP SERVICES

VCAP_SERVICE shall be used as environment variables.

`{ "calendardb": { "uri": "jdbc:mysql://localhost/OSM_CALENDAR", "username": "dbu_calendar", "password": "school123" }, "classesdb": { "uri": "jdbc:mysql://localhost/OSM_CLASSES", "username": "dbu_classes", "password": "school123" }, "contactsdb": { "uri": "jdbc:mysql://localhost/OSM_CONTACTS", "username": "dbu_contacts", "password": "school123" }, "userdb": { "uri": "jdbc:mysql://localhost/OSM_USER", "username": "dbu_user", "password": "school123" }, "rabbitmq": { "hostname": "localhost", "password": "pass", "port": "5672", "uri": "amqp://rmq:pass@localhost:5672", "username": "rmq" }, "redis": { "hostname": "localhost", "password": "pass1", "port": "6379" } }`
