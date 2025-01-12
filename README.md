# RSO-project
Implementation of cloud-native application for ordering food and making reservations in restaurants. 

The goal of the project is to develop a cloud-native web application for food ordering and delivery, with the option to make restaurant reservations online. The application allows users to browse restaurants and their offerings, order food, receive updates on order status, and make reservations. Restaurants can register in the application as service providers, where they can manage their menus, accept orders, and review reservations made by customers.

## Implemented microservices
The application consists of four microservices. The requirements and specifics are discussed in their repositories. 
- user-management: A microservice for user management. Users can create a new account or log in to an existing one. Restaurants can register as food providers.
- order-management: A microservice for managing orders. Users can place new orders and view all their past orders. Restaurants can view their current orders. 
- restaurant-management: A microservice for managing reservations. Users can create new reservations at their desired restaurants and view their past and active reservations on their profile. The microservice also enables restaurants to review current reservations in their establishments. 
- reservation-management: A microservice for managing restaurants. This microservice handles the addition of new restaurants, dishes, and menus.

## CI/CD Pipeline
The appication is running on Digital Ocean Kubernetes cluster. The testing and deployments have been automated trough Github Actions. 

## Serverless functions
The application also implements three serverless functions that call to external APIs:
- geolocation: Retrieves users location from users ip using [ip-api API](https://ip-api.com/)
- SMTP: Sends an email to the user using [mailsender](https://www.mailersend.com/)
- Distance calculator: Calculates distance between two adresses by calling [Google distance matrix API](https://developers.google.com/maps/documentation/distance-matrix/overview)

## Metrics and health
- Health of microservices is managed trough Kubernetes
- Metrics are scraped via Prometheus and displayed in Grafana 

# Links
[Web application](king-prawn-app-iog8u.ondigitalocean.app) (HTTP request must be enabled in browser)
[Prometheus](http://67.207.78.243/)
Grafana: needs to be configured via CLI `kubectl port-forward svc/grafana 80:80` so it runs on `localhost:80` 


