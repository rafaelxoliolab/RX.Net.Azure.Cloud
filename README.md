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


### What is Cloud Native?
The Cloud Native Computing Foundation provides the official definition:

_Cloud-native technologies empower organizations to build and run scalable applications in modern, dynamic environments such as public, private, and hybrid clouds. Containers, service meshes, microservices, immutable infrastructure, and declarative APIs exemplify this approach.

These techniques enable loosely coupled systems that are resilient, manageable, and observable. Combined with robust automation, they allow engineers to make high-impact changes frequently and predictably with minimal toil._



