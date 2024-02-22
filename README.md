# Microservice
The spring boot project consists of API gateway, Service Registry, Config server,Zipkin for tracing and Internal communication between two microservice with the use of RestTemplate
Services: employee-service, Department-service, Api-gateway service, Config-server and security implementation using keycloak
#Zipkin - for log tracing I used Zipkin and sleuth
#Fault tolerance handling - I used Resilience4j Circuit Breaker
#API gateway - i used API gateway for routing the request, load balancing and Also authentication by redirecting request to specific Realm in keycloak .
#However we can implement security using IAM tools like KEYCLOAK, which will handle and manage all security related tasks.
to use keycloak i just need to replace my Identity-service With Keycloak and delegate all the request to Keycloak before Routing it to requested service, 
we Route the Request if only Authenticated by Keycloak. We can also bypass some the URL that we do not need to authenticate .

