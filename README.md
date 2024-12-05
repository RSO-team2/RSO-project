# RSO-project
Implementation of cloud-native application for ordering food and making reservations in restaurants. 

## Services Checklist
- [ ] Frontend
  - [ ] Login screen
  - [ ] Ordering screen
  - [ ] Display in orders screen
  - [ ] ...

- [ ] Order management
  - [ ] Storing in database
  - [ ] (Producer) Event sender
  - [ ] (Consumer) Receives events and produces updates

- [ ] Reservation management
  - [ ] Storing in database
  - [ ] (Producer) Event sender
  - [ ] (Consumer) Receives events and produces updates

- [ ] Server-less function
- [ ] External API integration

## Others
- [ ] Helm Charts
- [ ] Centralized logging (`stdout`, stderr, `stdwarn`) dashboard
- [ ] Centralized metrics (uptime, resources, etc.) dashboard
- [ ] Health check endpoints
- [ ] Multitenancy
- [ ] Error handling
- [ ] Event sourcing

---
> NOTE: The below points should be taken care of for every service, API endpoint, etc.
```
Service Completion Checklist
- [ ] Repository management (for each service seperately).
  - [ ] Documentation (specific documentation)
    - [ ] Input's and outputs
    - [ ] Types management
  - [ ] READMEs (general documentation)
    - [ ] Purpouse
    - [ ] Use-cases
  - [ ] CI/CD Pipeline
  - [ ] Cloud deployment
```
---
> TA MEETING TAKEAWAYS

Recommended microservices:
- User Management Microservice
- Notification Microservice
- Order Management Microservice
- Reservation Management Microservice

Guidelines:
- Message function isn't meant for frontend
- Plug-and-play tools are permitted (even encouraged)
- Implementation of message passing can be demonstrative, that is not crucial for the projects functionalities, as long as it's well explained.
- Server-less function and external API can be combined together (implemented in the same part of the project, e.g. geolocation API).
- It's good to use an external API that requires authentication via an API key.
- README's are supposed to be deployment and use-case documentation and license.
- API documentation done via Swagger or OpenAPI automatically.
