# Spring Authentication

## Spring Security
[Notes taken from this site](https://spring.io/guides/topicals/spring-security-architecture/)

- `AuthenticationManager` has only one method:
```Java
public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
```
- >Spring Security provides some configuration helpers to quickly get common authentication manager features set up in your application. The most commonly used helper is the AuthenticationManagerBuilder.
- >Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet Filters, so it is helpful to first look at the role of Filters generally.

## Spring Cheat Sheet
[Notes taken from this page](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)

1. Set up a user model and repository.
2. Create a controller for that model.
3. `UserDetailsServiceImpl implements UserDetailsService`
4. `ApplicationUser implements UserDetails`
5. `WebSecurityConfig extends WebSecurityConfigurerAdapter`
6. Registration Page
7. Login Page

[Back to HOME](../README.md)