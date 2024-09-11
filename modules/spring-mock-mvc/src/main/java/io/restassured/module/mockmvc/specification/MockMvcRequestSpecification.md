* allows
  * specifying how the request look like
* `MockMvcRequestSpecification webAppContextSetup();`
  * requirements
    * `WebApplicationContext` -- must have been configured with -- `javax.servlet.ServletContext` 
  * allows
    * from the current MockMvc -> builds a new one / -- assign the -- `WebApplicationContext`
  * uses
    * `DispatcherServlet` will discover -- via `WebApplicationContext` --
      * Spring MVC infrastructure
      * application controllers
* `MockMvcRequestSpecification postProcessors(){}`
  * allows
    * extending `MockHttpServletRequest` | after initializing
  * recommendations
    * if you are going to set authentication/authorization -> use better `MockMvcAuthenticationSpecification.with()`
      * _Example:_ `given().auth().with(httpBasic("username", "password"))...`
* `MockMvcRequestAsyncSender when()`
  * uses
    * once you have set up the request specification -> invoke it
* TODO: