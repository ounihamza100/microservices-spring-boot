**Microservices with Spring Boot**

_Eureka Server_

It’s the naming server, or called service registry. It’s duty to give names to each microservice. Why?

1-No need to hardcode the IP addresses of microservices.

2-What if services use dynamic IP addresses; when autoscaling.

So, every service registers itself with Eureka, and pings Eureka server to notify that it’s alive.

If Eureka server didn’t receive any notification from a service. This service is unregistered from the Eureka server automatically.
