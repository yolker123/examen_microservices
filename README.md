# examen_microservices
VOLPELLIERE Anthony


EXO1

**create the package.json**

npm init -y 

**create the package-lock.json**

npm install http

**Create the image from the Doclerfile**

docker build -t examen-nodejs .

**Run the container**

docker run -p 8080:8080  examen-nodejs

**Push on docker hub**

docker login
docker tag examen-nodejs:latest yolker123/examen-nodejs:latest
docker push yolker123/examen-nodejs:latest

**KUBERNETES**

minikube start

kubectl apply -f node-deployment.yaml
kubectl apply -f autoscaling_hpa.yaml


EXO2

Q1 : With microservices architecture, a program is created as a collection of tiny, self-contained services that interface with one another using HTTP APIs and each execute a distinct process. This contrasts with a monolithic application, in which every process is closely connected to every other and functions as a single unit.

Q2 : Microservices: - Benefits include ease of maintenance, scalability, flexibility, autonomous deployment, robustness, and integration with new technologies.  
- Drawbacks: Complicated management, difficult inter-service communication, requirement for dispersed configuration management and monitoring.
    - Unchanging:  
Benefits: Easy testing, straightforward development, deployment, and management.  
- Drawbacks: Tough to scale, tightly coupled, one deployment for the entire application, challenging to integrate new technologies.

Q3 : The application must be divided according to functionalities.  On a large application, each service can have its own frontend, backend and database. A small application can separate these parts into 3. This reduces complexity, improves maintainability and facilitates scalability and upgrades.

Q4 : The CAP theorem states that a distributed IT system cannot simultaneously guarantee consistency, availability and partition tolerance. In Microservices, a trade-offs often have to be made between these three aspects. This affects the way services interact and manage data.

Q5 : Architectural consequences are the need to choose between consistency and availability when partitioning.

Q6 : Using containers to create autonomous services that can be scaled dynamically based on demand using Kubernetes is one way that microservices can enhance scalability in a cloud setting.

Q7 : Statelessness is the absence of state preservation between requests and the independence of each request made to the service. This enables requests to be processed by any service instance, which is crucial for scalability and robustness in microservices systems.

Q8 : An unique point of entry for external customers is an API gateway. It directs requests to the relevant services, handles cross-domain concerns like authentication and debit limits, and may offer data filtering or aggregation functions.