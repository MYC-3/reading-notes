# Spring Authorization

[Notes taken from this site](https://spring.io/guides/tutorials/spring-boot-oauth2/)

## Single Sign On With GitHub
- Here are some basic steps to create a site that uses Github for authentication.
- Create new application using `https://start.spring.io`
- Create a homepage, `index.html`within the `src/main/resources/static` folder.
- Add dependencies:
```Java
<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-oauth2-client</artifactId>
</dependency>
```
- Add a new Github App: `https://github.com/settings/developers`
- Configure by adding this to your application.yml:
```Java
spring:
  security:
    oauth2:
      client:
        registration:
          github:
            clientId: github-client-id
            clientSecret: github-client-secret
# ...
```

[Back to HOME](../README.md)