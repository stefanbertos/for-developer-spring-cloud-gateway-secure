# for-developer-spring-cloud-gateway-secure

cd keycloak-20.0.3
cd bin
kc.bat start-dev

admin/password

1.create new user admin/password
2.login to the admin console
3.create realm SpringBootKeycloak
4.create client spring-cloud-gateway-secure-service - Client authentication = ON, Standard Flow, Direct grant access
5.Settings -> set valid redirect urls = http://localhost:9000
6.Credentials-> copy credential secret and place into this application.yml
7.Roles->create role user
8.User -> create user test -> Credentials -> set password test

http://localhost:8080/realms/SpringBootKeycloak/.well-known/openid-configuration


http://localhost:9000/api/v1/client

jwt.io

https://docs.spring.io/spring-security/reference/servlet/oauth2/client/index.html


https://github.com/ThomasVitale/spring-cloud-gateway-resilience-security-observability
