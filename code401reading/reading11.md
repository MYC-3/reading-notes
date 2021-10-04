# Spring

## Spring Initialzr

1. Navigate to start.spring.io
2. Choose Gradle.
3. Add Dependencies:
    1. Spring Web
    2. Spring Boot DevTools
    3. Thymeleaf
4. Cick Generate to download zip file.

## Create Web Controller

- HTTP requests are handled by a controller.
- Controllers are identified by the `@Controller` annotation.
- `@GetMapping` handles mapping get requests to the proper method.
- `@RequestParam` binds the value of the query string parameter to the argument in the appropriate method.

## Thymeleaf

- Spring MVC's *model attributes* = *context variables* in Thymeleaf.
- Request Parameters Example:

> <https://example.com/query?q=Thymeleaf+Is+Great>!

- 

[Back to HOME](../README.md)