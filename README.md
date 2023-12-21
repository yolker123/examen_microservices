# examen_microservices
VOLPELLIERE Anthony

Q1 : Microservices architecture is a style of software architecture where an application is developed as a set of small, independent services, each running a unique process and communicating via HTTP APIs. This differs from a monolithic application where all processes are tightly coupled and run as a single entity.

Q2 : - Microservices :  
- Advantages: Scalability, flexibility, independent deployment, resilience, ease of maintenance and integration of new technologies.  
- Disadvantages: Management complexity, communication challenges between services, need for distributed configuration management and monitoring.
    - Monolithic:  
- Advantages: Simplicity of development, deployment and management, ease of testing.  
- Disadvantages: Difficulty of scaling, strong coupling, single deployment for the whole application, difficulty of integrating new technologies.

Q3 : The application must be divided according to functionalities.  On a large application, each service can have its own frontend, backend and database. A small application can separate these parts into 3. This reduces complexity, improves maintainability and facilitates scalability and upgrades.

Q4 : The CAP theorem states that a distributed IT system cannot simultaneously guarantee consistency, availability and partition tolerance. In Microservices, a trade-offs often have to be made between these three aspects. This affects the way services interact and manage data.

Q5 : Architectural consequences are the need to choose between consistency and availability when partitioning.

Q6 : Using containers to create autonomous services that can be scaled dynamically based on demand using Kubernetes is one way that microservices can enhance scalability in a cloud setting.

Q7 : Statelessness is the absence of state preservation between requests and the independence of each request made to the service. This enables requests to be processed by any service instance, which is crucial for scalability and robustness in microservices systems.

Q8 : An unique point of entry for external customers is an API gateway. It directs requests to the relevant services, handles cross-domain concerns like authentication and debit limits, and may offer data filtering or aggregation functions.