# spring_boot_demo
Spring boot API for a Person CRUD

## Getting Started

These are the basics steps to build a model CRUD API with Spring Boot. 

### Prerequisites

Java 11
(Optional) IntelijIDEA
Docker

### Steps

1. Go to [start.spring.io](https://start.spring.io) and create a Spring Boot 2 application with Maven, Java 11 and Spring Web Dependencies.
2. Open with Intellij by selecting the pom.xml file inside the project.
3. Now you can do the initial commit. 
4. Create the packages needed for the structure: api, dao, model and service.
5. Create initial classes:
* Model (person)
* Dao Interface to be able to change Database implementation later on. 
* In-Memory Database implementation of the Dao interface.
* The Service class to interact with the Database.
* The controller that handles user request to the API. 
6. Add Spring Boot annotations : 
* @Repository("name_of_the_repo_impl")
* @Service
* @Autowired
* @Qualifier("name_of_the_repo_impl")
* @RestController
* @RequestMapping("api/version/model")
* @PostMapping, @GetMapping(path = "{field}"), @DeleteMapping(path = "{field}"), @PutMapping(path = "{field}")
* @PathVariable("field")
* @RequestBody Model model
* @JsonProperty("field")
7. Implement the CRUD methods on the Dao In-Memory class and test on Postman client on localhost:8080/api/version/model
8. Add validation annotations on model fields, and controller 
* @Valid, @NonNull, @notBlank...
9. Create a Docker container for the Postgres Database
*

## Built With

* [Spring Boot](https://start.spring.io) - Framework used
* [Maven](https://maven.apache.org/) - Dependency Management



## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


