# Net Azure Cloud
Learning project for .NET Azure Cloud.

By Rafael Xolio


## Cloud-native environments
You'll design and maintain integrations, APIs, and event-driven solutions on Azure.


### Monolithics core application

<img width="645" height="281" alt="image" src="https://github.com/user-attachments/assets/fa1d0940-ea67-447a-8020-6e38da201688" />

- Large _core application_ containing all of your domain logic.
- It includes _modules_ such as Identity, Catalog, Ordering, and more.
- The modules directly communicate with each other within a single server process.
- The modules share a large relational database.
- The core exposes functionality via an HTML interface and a mobile app.

### Cloud-native design
<img width="623" height="404" alt="image" src="https://github.com/user-attachments/assets/28baa738-36fd-40aa-8404-6d5458d72d12" />


- Note how the application is decomposed across a set of small isolated microservices.
- Each service is self-contained and encapsulates its own code, data, and dependencies.
- Each service is deployed in a software container and managed by a container orchestrator.
- Instead of a large relational database, each service owns it own datastore, the type of which vary based upon the data needs.
- Note how some services depend on a relational database, but other on NoSQL databases. One service stores its state in a distributed cache.
- Note how _all traffic routes through an API Gateway service_ that is responsible for routing traffic to the core back-end services and enforcing many cross-cutting concerns.
- Most importantly, the application takes full advantage of the _scalability, availability, and resiliency features_ found in modern cloud platforms.


## What is Cloud Native?
The Cloud Native Computing Foundation provides the official definition:

_Cloud-native technologies empower organizations to build and run scalable applications in modern, dynamic environments such as public, private, and hybrid clouds. Containers, service meshes, microservices, immutable infrastructure, and declarative APIs exemplify this approach._

_These techniques enable loosely coupled systems that are resilient, manageable, and observable. Combined with robust automation, they allow engineers to make high-impact changes frequently and predictably with minimal toil._

- Cloud native is about speed and agility.
- Cloud-native systems are designed to embrace rapid change, large scale, and resilience.

<img width="640" height="269" alt="image" src="https://github.com/user-attachments/assets/7ba462c5-4c98-41cb-9ffe-581c9c5b7a9a" />

## The Twelve-Factor Application

The following table highlights the Twelve-Factor methodology:
<img width="648" height="406" alt="image" src="https://github.com/user-attachments/assets/516a4e73-71c6-4d88-ba9b-aa027322ea51" />
<img width="647" height="413" alt="image" src="https://github.com/user-attachments/assets/80855828-affb-46cb-81c4-8ccc8ed2e0b8" />
<img width="644" height="433" alt="image" src="https://github.com/user-attachments/assets/7d52defc-becd-4b61-8128-8333d1c0410a" />

Three new factors:
<img width="643" height="263" alt="image" src="https://github.com/user-attachments/assets/009d10bf-9058-4694-aecb-e5618a636f48" />







