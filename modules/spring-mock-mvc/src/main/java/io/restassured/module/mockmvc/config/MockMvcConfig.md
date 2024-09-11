* == general configuration of Spring Mock MVC module
* `MockMvcConfig mockMvcConfig() {}`
  * new instance of `MockMvcConfig`
* `MockMvcConfig dontAutomaticallyApplySpringSecurityMockMvcConfigurer() {}`
  * new instance of `MockMvcConfig` / `automaticallyApplySpringSecurityMockMvcConfigurer=false`
    * check `MockMvcConfigurer` | "spring-security"