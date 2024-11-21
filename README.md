# RSO-project
Implementation of cloud-native application

## Services Checklist
- [ ] Frontend
  - [ ] Login screen
  - [ ] Ordering screen
  - [ ] Displayin orders screen
  - [ ] ...

- [ ] Order management
  - [ ] Storing in database
  - [ ] (Producer) Event sender
  - [ ] (Consumer) Recieves events and produces updates

- [ ] Reservation management
  - [ ] Storing in database
  - [ ] (Producer) Event sender
  - [ ] (Consumer) Recieves events and produces updates

- [ ] Serverless function
- [ ] External API integration

## Others
- [ ] Helm Charts
- [ ] Centralized logging (stdout, stderr, stdwarn) dashboard
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