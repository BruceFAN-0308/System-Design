1. # Spring Core

1. ## What is IOC and AOP

IOC: Inversion of Control. Spring uses a container to control the object. We do not need to manage objects any more. For example, there are a lot of objects. They are dependent on each other. If we create them by ourselves. It is very complex. We give the manage power to the container, and IOC container helps us manage objects.

AOP: Aspect Oriented Programming. It is similar to OOP. The goal is module coding. It helps users just focus on business development. And make the module code together. Just use the annotation to set the aspect. Such as exception controlling, logging and authentication.



1. ## What are the Spring beans

The objects are instantiation, configured, wired and managed by Spring IOC container, which is called Spring beans.

The default creation scope is singleton.



1. ## How to define a Spring bean.

We can use xml and annotation. Usually we use annotation. Because it is easy to use, we can use @Component



1. ## Spring lifecyle

1. IOC Instantiates the beans by bean's defination. Give a memory address to this bean.

2. Spring sets the property which beans are dependent on beans.

3. Bean factory set the bean's ID. Usually the bean id is its name.

4. Constructor this bean. Call a lot of aware functions. Do the before-construction function, constructor function and post-construction function.

5. Creation finished. As a bean to use.

6. Destory the beans.

   

1. ## What is the difference between Spring and Spring Boot?

1. Spring Framework provides IOC, AOP and a lot of features to help developer build system easier and effective. Because Spring Framework might have a lot of configurations to configure. Spring Framework configurations might be very complex.
2. Spring Boot is a framework based on Spring. It helps us configure a lot of things by default. We do not need to configure a lot of things.

Example, configure a database and logging beans.

1. Spring: We need to configure a database and logging bean, we might use XML and configure a lot of things.
2. Spring Boot: We just need to write the properties in the properties file.

**There are a lot of beans Spring Boot helps us configure automatically.**



1. ## What is the difference between @RequestMapping and @RestController.

1. @RequestMapping

It is a router annotation for http request. A function or a class has this annotation. The same url request will call this class or class's function

2. @RestController

It is a combination annotation including @ResponseBody and @Controller

​	a. @ResponseBody: It will help us deserialize the JSON to Java objects. 

​	b. @Controller: It will configure this class as a bean and mark this class as a RESTful API web service by using Spring MVC.

```Java
@RestController
@RequestMapping("/controller_test")
public class Controller {

    @RequestMapping("/info")
    public BaseResponse<Object> info() {
        return BaseResponse.success("request successfully.");
    }
}
```