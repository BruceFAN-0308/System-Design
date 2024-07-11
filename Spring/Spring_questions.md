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