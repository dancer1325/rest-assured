* == Spring MVC module of `RestAssured`
* JavaDoc == Spring MVC's test documentation
* `void mockMvc(MockMvc mockMvc){}`
  * set a `MockMvc` instance
    * uses
      * when you make requests
  * -- can be overwritten by -- `MockMvcRequestSpecification`
* TODO:
* `MockMvcRequestSpecification given(){}`
  * 👁️if you need to specify request's parameters or body -> main entry-point of the API 👁️
  * 👁️ == `MockMvcRequestSpecification with(){}` / another syntax 👁️
* TODO: