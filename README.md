# hello-world
## Hahha
Just Another Repository

1. Hlwle
   1. diddw
   2. jjdjd
   3. jdjjdjd
   4. jnccnc
   5. 
2. dhwhdwd
3. fjhfbfjf

##### **[**Daily Spring Routine**](https://docs.google.com/spreadsheets/d/1m0_7pcUk8FXwAH3Pp0hfb1UFfG-Wpcs58ipnYcivmX0/edit?usp=sharing) ****[**Spring - Google Drive**](https://drive.google.com/drive/u/4/folders/1O_2Ad86kEQTj0v-NwMheY6QoRoXA7_jh) ****[**Source code for the course: Spring Boot 3, Spring 6 and Hibernate for Beginners**](https://github.com/darbyluv2code/spring-boot-3-spring-6-hibernate-for-beginners)**Download PDF Files**All slides that are shown during the course are available also as a reference and can be downloaded here:<http://www.luv2code.com/download-spring-hibernate-pdfs>\---**Download FAQ Notes PDF Files**The course also includes a collection of FAQ Notes. These are available for download as PDFs:<http://www.luv2code.com/download-spring-hibernate-faq-notes>Symbols: 📂file symbol  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_Question: [java - why does Spring use XML for component wiring? - Stack Overflow](https://stackoverflow.com/questions/1124516/why-does-spring-use-xml-for-component-wiring)**


### Install Java Dependencies at first.


##### **1. Install Java
2. Install JDK, JDK might contain JRE
3. Install JRE**> JDK vs JRE vs JVM**JDK(Java Development Kit) is for development purposes whereas JRE(Java Runtime Environment) is for running the java programs. So, If you want to run Java programs, but not develop them, download the JRE. If you want to develop Java applications, download the Java Development Kit, or JDK. The JDK includes the JRE. Along with JRE, the JDK also consists of various development tools (Java Debugger, JavaDoc, compilers, etc.)JVM is the heart of the Java programming language and provides platform independence. If you choose to install JRE and JDK separately, JDK and JRE both contain JVM so that we can run a java program.**> Is it mandatory to have the same version of jdk and jre?** [Source](https://stackoverflow.com/questions/54417552/is-it-mandatory-to-having-same-version-of-jdk-and-jre)If your code is using features of Java 11, you will need the JRE 11 to run it. You can set your project in your IDE to a compatibility level of JRE 8 (like [here](https://stackoverflow.com/questions/22584427/what-is-compiler-compliance-level-in-eclipse)). This prevents any usage of features newer than Java 8.Example: Develop with JDK 11 but only use features from Java 8 -> code will run in JRE 8. **See the older versions as subsets of the newer ones.****


### Install an IDE


##### **Install Eclipse[What version of Java is running in Eclipse?](https://stackoverflow.com/questions/1944468/what-version-of-java-is-running-in-eclipse)menu Help > About Eclipse > Installation Details > Configuration tab. Locate the line that says: java.runtime.version=....Or  menu Window >preferences >java (expand the menu)> compiler (click the option) > “Compiler compliance level” , indicates which version of JDK will the compiler use.Or menu Window >preferences >java (expand the menu)> Installed JRE (expand the menu) > execution environmentTo check which version is installed in the computer, run this cmdjava -version ![](https://lh6.googleusercontent.com/4sv6MYFsBglYuZru9b-jNV3BOLcg45Ji2SaGVBhJskKjNOJW7zL1kUJxrG8oh_sF2deTtm3J6iBS2MkfisBJ17fausMzYuRyRJnkxUv9DLewThW-AGpDyMkyecSfFzE5IJnRN3U46fBUbIxZ1TwQiQ)![](https://lh4.googleusercontent.com/1zAv0AmhrNb4ExEOEpGtQpVzfsooD02mPVcsYGT1oULXsB44xcamq1OzmRZaYk5hs-7mml_cCoPZJWWBNzIUHjo7B4aCkT4_dUoMGbVWq0QuGolslap_-yBMUlFJkZTEB0teN3vwcrbaVQMbd76r9A)![](https://lh5.googleusercontent.com/T6CssMERA0vfh91ilJ0IoLFJ-LA4-ofUj1xL1bgFlczGokE7ryEBPyRZwb5L-e2tIaWim0XEk2uie_MZ71MkEjJDgIHPeXJ3GJKf3U_gL0xfhO8NFUdABqQcifJM-7IvAAU5SAcv4vGIjcnvXahnIbQ)Spring Boot[Spring Boot - Google Docs](https://docs.google.com/document/d/13_mvdnYogB2P1YmXW3bVpwCwyhYijAbuILSyve9SmqQ/edit)SpringSpring Initial Setup**


### How to Install Spring in your project?


##### **1. First step is to download the Spring Framework Jars from - [JFrog (spring.io)](https://repo.spring.io/ui/native/release/org/springframework/spring/). Unzip it and copy the Jars from the **lib** folder.
2. Select the project and create a folder inside it named “lib” and then paste the jar files inside the “lib” folder of spring framework bundle.
3. Select the project > right click > select  properties > java build path > select Libraries> select classpath> Add Jars > (a popup will appear) > select the files, you just pasted inside the current projects **lib** folder > press apply ![](https://lh4.googleusercontent.com/75B3ewhN37u-1jU3A73YGx-5TKpSu8zppaLlF1Qt2Y_08YDe2ES0j4ZERe7TVvon3P18jkhtVNFU_-0VREccPHjUNbFL8ncM2wyGFAl8dd49GRQ9oaFXERumSewMdgOzyL-lP6NVEIdBso4Ut7JkbCA)
4. After completion of installation, a new folder named “Reference Libraries” will be added.![](https://lh6.googleusercontent.com/K9jMKiRvC0wx93MiBp9cnTUO7GZBoVcd2Jre9OsZ0I2ry8xghkhhCkGRFR6tH-Tij_q7b3-kxaTf2glM7SzFSAzdqKzhs5lb5pHTnFZaLUvK42WJvdq6xJELNd04Irf50yXB2z5VPsoBKzxjLi1UFkI)\>>> Download Spring Framework Jars from - [JFrog (spring.io)](https://repo.spring.io/ui/native/release/org/springframework/spring/)**


### Eclipse is unable to import @PostConstruct or @PreDestroy


##### **When using Java 9 and higher, javax.annotation has been removed from its default classpath. That's why Eclipse can't find it.Solution1. Download the javax.annotation-api-1.3.2.jar from <https://search.maven.org/remotecontent?filepath=javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.jar>[javax.annotation : javax.annotation-api : 1.3.2 - Maven Central Repository Search](https://search.maven.org/artifact/javax.annotation/javax.annotation-api/1.3.2/jar)2. Copy the JAR file to the lib folder of your project. Use the following steps to add it to your Java Build Path.

   1. Right-click your project, select Properties
   2. On left-hand side, click Java Build Path
   3. In top-center of dialog, click Libraries
   4. Click Classpath and then Click Add JARs …
   5. Navigate to the JAR file &lt;your-project>/lib/javax.annotation-api-1.3.2.jar
   6. Click OK then click Apply and CloseSpring Framework Fundamentals**


### How does spring achieve dependency injection at runtime?


##### **Answer: [java - How does spring achieve dependency injection at runtime? - Stack Overflow](https://stackoverflow.com/questions/43514699/how-does-spring-achieve-dependency-injection-at-runtime)**


### Dependency Injection Frameworks: How do they work?


##### **[Dependency Injection Frameworks: How do they work? - Stack Overflow](https://stackoverflow.com/questions/3973779/dependency-injection-frameworks-how-do-they-work)**


### What is a Spring Bean?


##### **A "Spring Bean" is simply a Java object.When Java objects are created by the [Spring Container](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.228v69og4p3w), then Spring refers to them as "Spring Beans". Spring Beans are created from normal Java classes .... just like Java objects.- \-Here's a blurb from the Spring Reference Manual![](https://lh3.googleusercontent.com/rAeqoVjCEZx6cUJzbo5fMyDDS02uLGFuQtfLbs8tJtCPp3uvvSq7K-iF87sqiWsmF1GzRqmUSLRzVEjp6WU1eS3Ws3BUMYIyvkvhua9tlZnlHPlNJIAXwt6cj0QawPTRGxA9ElXN0adY_ZA8Epd1ZGw)Source: <https://docs.spring.io/spring/docs/current/spring-framework-reference/core.html#beans-introduction>In the early days, there was a term called "Java Beans". Spring Beans have a similar concept but Spring Beans do not follow all of the rigorous requirements of Java Beans.In summary, whenever you see "Spring Bean", just think of a Java object.**


## Achieving Inversion of Control through various mechanisms


##### ****Inversion of Control is a principle in software engineering which transfers the control of objects or portions of a program to a container or framework**. We most often use it in the context of object-oriented programming.We can achieve Inversion of Control through various mechanisms (design pattern) such as: Strategy design pattern, Service Locator pattern, Factory pattern, and [Dependency Injection](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.e4vfvmvykq4w) (DI).Read more: <https://www.baeldung.com/inversion-control-and-dependency-injection-in-spring>Requirement of Inversion of Control:1. App should be Configurable -> **How do we achieve this?**

2. Easily change the coach for another sport -> we can achieve this by Inheritance (extending coach class)

   1. Hockey, tennis, cricket etcWe can make the app configurable by the help of Spring Container. We can read the implementation of the hard codes by reading the configuration file. Thus we only need to change the configuration file for future updates and we don't have to change our java source code.See: https&#x3A;//youtu.be/VbqgSp-TpWg?t=206**


## Spring Modules


##### **The Spring framework comprises many modules such as core, beans, context, expression language, AOP, Aspects, Instrumentation, JDBC, ORM, OXM, JMS, Transaction, Web, Servlet, Struts etc. These modules are grouped into Test, Core Container, AOP, Aspects, Instrumentation, Data Access / Integration, Web (MVC / Remoting) as displayed in the following diagram.![](https://lh6.googleusercontent.com/WLbXIGoaRMZiLDgtfw3GVJgbF3CfmeBo3oGr7RFbj_ZTRs35GRBC28hgdeSHDJOyYcPPTTBbhXnGVCvGgofnMPHd6k0JTrx__xgvANSJLf-ssXPYsMaAnqvS_LLWrInUvH5B0CKn74Jf4ckAW9vNmPs)Spring Core**


## Spring Container


##### **The IoC container is responsible to instantiate, configure and assemble the objects. The IoC container gets information from the XML file and works accordingly. It's generally known as **ApplicationContext.** There is another IoC container called **BeanFactory.****


#### Using ApplicationContext


##### **The ClassPathXmlApplicationContext class is the implementation class of ApplicationContext interface. We need to instantiate the ClassPathXmlApplicationContext class to use the ApplicationContext as given below:|                                                                                                |
| ---------------------------------------------------------------------------------------------- |
| ApplicationContext context =   new ClassPathXmlApplicationContext("applicationContext.xml");   |The constructor of ClassPathXmlApplicationContext class receives a string, so we can pass the name of the xml file to create the instance of ApplicationContext.**


#### Specialized Implementations


##### **1. ClassPathXmlApplicationContext
2. AnnotationConfigApplicationContext
3. GenericWebApplicationContext
4. Others**


#### Primary Function


##### **1. Create object (when the configurable properties will be provided to spring) and mange object (**Inversion of control**)
2. Inject object dependency (Dependency Injection )**


#### Configuring Spring Container (3 ways)


##### **1. XML Configuration file(legacy, but most legacy app still use it)
2. Java Annotation(modern)
3. Java Source Code(modern)**


## Spring Development Process (Step by Step)


##### **Considering the fact that the object(TrackCoach, CricketCoach etc) that defines the beans has already been created. After that we can do the following steps,1. Configure your Spring Beans
2. Create a Spring Container
3. Retrieve Beans from your Spring Container**Step 1**: Configure your Spring Beans (In this case with xml file)📂applicationContext.xml|                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;?xml version="1.0" encoding="UTF-8"?> &lt;beans>    &lt;!-- Define your beans here -->     &lt;bean id="myCoach" class="com.diptopaul.springdemo.TrackCoach">&lt;/bean>&lt;/beans> |Format: &lt;bean id="an Id name like an alias" class="fully qualified class name of implemented class">&lt;/bean>**Step 2**: Create a Spring Container📂App.java|                                                                                                          |
| -------------------------------------------------------------------------------------------------------- |
| ClassPathXmlApplicationContext context =   new ClassPathXmlApplicationContext("applicationContext.xml"); |Format: new ClassPathXmlApplicationContext(name of config file);**Step 3**: Retrieve Beans from your Spring Container📂App.java|                                                          |
| -------------------------------------------------------- |
| Coach theCoach = context.getBean("myCoach",Coach.class); |Format: context.getBean("the id provided during the configuration of Bean", Interface class of implemented class provided during the configuration of Bean )**


### Why do we specify the Coach interface in getBean()?


##### **For example:Coach theCoach = context.getBean("myCoach", Coach.class); \---AnswerWhen we pass the interface to the method, behind the scenes Spring will cast the object for you.context.getBean("myCoach", Coach.class)  **-> the returned object will be casted by the Coach interface.**However, there are some slight differences from normal casting.From the Spring docs:Behaves the same as getBean(String), but provides a measure of type safety by throwing a BeanNotOfRequiredTypeException if the bean is not of the required type. This means that ClassCastException can't be thrown on casting the result correctly, as can happen with getBean(String).Source:  <http://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/beans/factory/BeanFactory.html#getBean-java.lang.String-java.lang.Class->**


### XML Based Injection


##### **Why XML? Answer: [XML-Based Injection in Spring | Baeldung](https://www.baeldung.com/spring-xml-injection) (Search more and write your own reason)**


# Dependency Injection (Read: [Dependency Injection in spring - javatpoint](https://www.javatpoint.com/dependency-injection-in-spring))


##### **The Dependency Injection is a design pattern that removes the dependency of the programs. In such cases we provide the information from an external source such as an XML file. It makes our code loosely coupled and easier for testing. In such case we write the code as:|                                                                                                                                                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| class Employee implements Person {//constructor injection Address address; Employee(Address address){   this.address=address;  } //setter injectionPrivate Address address2; public void setAddress(Address address){    this.address2=address;  }  } |Instance of Address class is provided by an external source such as XML file either by constructor or setter method.**


## Two ways to perform Dependency Injection in Spring framework


##### **Spring framework provides two ways to inject dependency- By Constructor(Constructor Injection) - we use a constructor inside the dependent class to inject the helper object. Example: [above](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.2uu7wtydvuo)
- By Setter method(Setter Injection) - we use a setter method inside the dependent class to inject the helper object. Example: [above](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.2uu7wtydvuo)
- By Fields(Field Injection) - we use a field inside the dependent class to inject the helper object. Example: [above](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.2uu7wtydvuo)We can use different approaches to implement the injection.**There are three ways to configure the Spring Container**,1. XML Based (Legacy)
2. Annotation Based 
3. Java Based**


## XML Based


### Constructor Injection - Dependency Injection by constructor


##### **Steps: 1. Define and Create the Dependency Interface and Class with their properties, eg: Address class or FortuneService(Interface) with HappyFortuneService.
2. Create a constructor in the class (that will use the Dependency Class) for Injection.
3. Configure the Dependency Injection in the Spring config file.Example 1: [Spring Constructor injection - javatpoint](https://www.javatpoint.com/spring-tutorial-dependency-injection-by-constructor) (with Primitive and Strings)|                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;?xml version="1.0" encoding="UTF-8"?> &lt;beans>     &lt;bean id="e" class="com.javatpoint.Employee">  &lt;!--Comment: -->       &lt;constructor-arg value="10" type="int">&lt;/constructor-arg>       &lt;constructor-arg value="10">&lt;/constructor-arg> &lt;!--Comment: with no type mentioned, by default it be treated as string -->       &lt;constructor-arg value="Sonoo">&lt;/constructor-arg>     &lt;/bean>  &lt;/beans> |Example2: [Spring Constructor Injection with Dependent Object - javatpoint](https://www.javatpoint.com/spring-tutorial-constructor-injection-with-dependent-object) (With Object)|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;beans>     &lt;bean id="a1"  class="com.javatpoint.Address">          &lt;constructor-arg value="ghaziabad">&lt;/constructor-arg>         &lt;constructor-arg value="UP">&lt;/constructor-arg>         &lt;constructor-arg value="India">&lt;/constructor-arg>       &lt;/bean>     &lt;bean id="e"  class="com.javatpoint.Employee">          &lt;constructor-arg value="12" type="int">&lt;/constructor-arg>         &lt;constructor-arg value="Sonoo">&lt;/constructor-arg>         &lt;constructor-arg>             &lt;ref bean="a1"/>         &lt;/constructor-arg>     &lt;!-- or short form         &lt;constructor-arg ref="a1"/>     -->     &lt;/bean> &lt;/beans> |Behind the scene spring will do:|                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Address address = new Address(city, state, country);//&lt;- It will be created using the first bean configuration data provided by xml, value of city = "ghaziabad", state = "UP" , country = "India";Employee employee = new Employee(id, name, Address);//&lt;- It will be created using the first bean configuration data provided by xml, value of id = 12, state = "Sonoo" , Address = will pass the address object; |Example 3: [Inheriting Bean in Spring - javatpoint](https://www.javatpoint.com/spring-tutorial-inheriting-bean-in-spring) **


### Dependency Injection by setter method (Setter Injection) - **XML Based**


##### **We can inject the dependency by setter method also. The **&lt;property>** subelement of **&lt;bean>** is used for setter injection.Example 1: [Spring Setter Injection - javatpoint](https://www.javatpoint.com/spring-tutorial-dependency-injection-by-setter-method) (with Primitive and Strings)|                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;?xml version="1.0" encoding="UTF-8"?> &lt;beans>     &lt;bean id="obj" class="com.javatpoint.Employee">          &lt;property name="id">              &lt;value>20&lt;/value>          &lt;/property>          &lt;property name="name">              &lt;value>Arun&lt;/value>          &lt;/property>          &lt;property name="city">              &lt;value>ghaziabad&lt;/value>          &lt;/property>     &lt;/bean>  &lt;/beans> |Example2: [Spring Setter Injection with Dependent Object - javatpoint](https://www.javatpoint.com/spring-tutorial-setter-injection-with-dependent-object) (With Object). Unlike constructor injection there is no special element to achieve SI. We use the property element to achieve SI.|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| &lt;?xml version="1.0" encoding="UTF-8"?> &lt;beans>     &lt;bean id="address1" class="com.javatpoint.Address">          &lt;property name="addressLine1" value="51,Lohianagar">&lt;/property>          &lt;property name="city" value="Ghaziabad">&lt;/property>          &lt;property name="state" value="UP">&lt;/property>          &lt;property name="country" value="India">&lt;/property>      &lt;/bean>     &lt;bean id="obj" class="com.javatpoint.Employee">          &lt;property name="id" value="1">&lt;/property>          &lt;property name="name" value="Sachin Yadav">&lt;/property>          &lt;property name="address" ref="address1">&lt;/property>      &lt;/bean>  &lt;/beans> |**


### Dependency Injection by fields (Field Injection) - **XML Based**


### Bean Scope : Singleton, Prototype


##### **|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("applicationContext.xml");  //try removing the Referenced Library and see if it works?  //retrieve bean from spring container Coach theCoach = context.getBean("myCoach",Coach.class); theCoach.setValue("theCoach");  // Coach myCoach = context.getBean("myCoach",Coach.class); myCoach.setValue("myCoach");  //call methods on the bean //example of singleton bean System.out.println(theCoach.getDailyWorkout());  //Singleton scope: two different objects but it uses the same bean resource, so the coachName of the bean that was initially assigned by the first object is being changed by the second object later on. System.out.println(theCoach.getValue()); System.out.println(myCoach.getValue());  boolean result = (theCoach == myCoach); System.out.println(result); //both point to the same address when scope is Singleton. Change the scope to Prototype and see the difference. System.out.println("Address of theCoach: " + theCoach); System.out.println("Address of myCoach: " + myCoach); | |                                                                                                                                                                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;?xml version="1.0" encoding="UTF-8"?>&lt;beans ...>&lt;!-- Define your beans here -->      &lt;bean id="myCoach" class="com.diptopauldip.springdemo.CricketCoach" scope="prototype">&lt;/bean>     &lt;!--  &lt;bean id="myCoach" class="com.diptopauldip.springdemo.CricketCoach" scope="singleton">&lt;/bean>  &lt;/beans> |Output when using **singleton** scope in xml bean configuration:![](https://lh4.googleusercontent.com/yrNFxg3uQdMR7PXvUpL_fz2jFee7R81wlX0EosR1M0Q6ZKjYJM1TpVngwtN1zHw1-foPWokV6AhaHblczRth2RQKGPr7gdGwV9YLikXFzdSvBsV4E_BV3KuxgDk2kost7g_h0J0CwgWTEIcGfqNRhGY)Output when using **prototype** scope in xml bean configuration:![](https://lh4.googleusercontent.com/FrtF0rj3VDNPKXQeHx4orZge3RZNevvv33Szzi_l7JRVS1QxlPxTWPPfhTTk8fQEL01PYF5ZNg3WN35IO_KFKPiyIXtZL82NoE2EsI9NIelX1YqhFOZ591qzdYnR-MGdmDlDcVHhlbXMJA1togmWT7k)**


### Bean Lifecycle: Bean Initialisation, Bean Destruction


##### **Bean Init Method ConfigurationBean Destroy Method Configuration<https://www.youtube.com/watch?v=GVb1wuF-p9Q&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=36&pp=sAQB><https://youtu.be/MIBk2_StDwU?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H>**


## Spring Configuration with Java Annotations ([Annotation Based](https://youtu.be/6FVJ3nigbk0?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)) : Component Scanning


##### **How do we pass values inside a spring xml file when using the Component Annotation approach?**


### Initial Setup


##### **Step 1: writing the part of xml file, adding **context:component-scan** element|                                                                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;?xml version="1.0" encoding="UTF-8"?>&lt;beans ...>&lt;!-- Define component-scan here -->    &lt;context:component-scan base-package="com.diptopaul.springdemo">&lt;/context:component-scan>&lt;/beans> |Step 2: Add component Annotations to Java classes.When Bean ID is specified.|                                                                                                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| import org.springframework.stereotype.Component; @Component("tennisCoach")//bean id specified public class TennisCoach implements Coach { @Override public String getDailyWorkout() { // TODO Auto-generated method stub return "Run 10 KM"; } } |When Bean ID is not specified, **by default the camel case name of the actual bean class name will be bean id**. Main method can be used.|                                                                                                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| import org.springframework.stereotype.Component;@Component //no specific bean id, public class FootballCoach implements Coach { @Override public String getDailyWorkout() { // TODO Auto-generated method stub return "Practice penalty kicks"; } } |Step 3: Retrieve bean from Spring container (Same/Common Final Step)AnnotationDemoApp.java|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| public static void main(String\[] args) { // read spring config files ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("annotation_applicationContext.xml");  // get the bean from spring container Coach myCoach = context.getBean("sillyTennisCoach",Coach.class);  // call a method on the bean System.out.println(myCoach.getDailyWorkout());  //An example of default bean ID, camelcase of subclass name Coach newCoach = context.getBean("footballCoach",Coach.class); System.out.println(newCoach.getDailyWorkout());  // close the context context.close(); } |7**


### Spring Configuration with Java Annotations - Dependency Injection


#### Keywords: Component, Autowiring, Qualifiers


##### **Spring framework provides two ways to inject dependency using Annotation Based approach- By Constructor
- By Setter method
- By Field Injection using **Java Reflection****


#### Step 1: 


##### **![](https://lh4.googleusercontent.com/xE8xBakLMIize3UQbG64wLf0GJ2AEwW43rF1EMRZflBqr1XQ8355MpFQH_CYBHJCtj_zBE5YXs2hxDe4XxvhsKT7wOylYOPav56dp2weZvhogcP9npGDex_TIcQ-XFhJygz1hQHH-tVoWHAT4Jb09Qs)**


#### Step 3: Configure the dependency injection. XML based vs Annotation Based.


##### **![](https://lh5.googleusercontent.com/F1-g5xH-9i6CvhIEPXoFoagJVlgYuFlI9uLdN85v9NOHcVNh5XyV8uyob_yhfH60n69U8Wtysrq3B5rpGiPHyiKNxXfxo_K_cOkxmXZ-Y0T6nCguSMQk9ZHCdwrs14G0HKPhGKezH0xrTbsPtoQtdNc)**


### By Constructor - Annotation Constructor Injection [22-annotation-constructor-injection.pdf](https://drive.google.com/file/d/1n7CH-0EL8goxCN4bTcsME4EaDzsWZ9Ir/view?usp=drive_link)  [ovwVideo ](https://www.youtube.com/watch?v=lZO_xRBCYYU&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=44&ab_channel=freeCodeCampBengali)\|[ codeVid1](https://youtu.be/LdLvhD1PWk0) [codeVid2](https://youtu.be/sosdTfpR4XQ?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)


##### **With adding Autowired annotation, Spring will look for a component that implements the FortuneService interface. In this case, after scanning all the components spring will have a list of components, out of this in this case, only HappyFortuneService implements the FortuneService interface, this HFS meets the requirement.**AFAQ**1. How does @Autowired work internally? 

   1. Best Answer: <https://stackoverflow.com/a/19419296> 
   2. Second best: <https://stackoverflow.com/a/3153617>

2. How is Spring able to inject @Autowired component or implement the @Autowired functionality?

   1. <https://stackoverflow.com/a/3538154>**FAQ**: - Using Qualifiers with Constructor?

  - [073-using-qualifier-with-constructors.pdf](https://drive.google.com/file/d/14V6aJTh_zUQ_ItzEZgZAGzdnP_Q6vDoc/view?usp=share_link)**


### By Setter method - Annotation Setter Injection [23-annotation-setter-injection-overview.pdf](https://drive.google.com/file/d/1QIJlHcMn1lryql3dQ4hMS34IpSyJnBZM/view?usp=share_link)  [ovwVideo ](https://youtu.be/tr4kogAm01A?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)\|[ codeVid1](https://youtu.be/LdLvhD1PWk0)


##### **Step1: Create setter method(s) in your class for injections|                                                                                                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Component  public class TennisCoach implements Coach {     private FortuneService fortuneService;     public TennisCoach() { }    public void setFortuneService(FortuneService fortuneService) {    this.fortuneService = fortuneService;    }     ... } |Step 2: Configure the dependency injection with Autowired Annotation |                                                                                                                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Component  public class TennisCoach implements Coach {     private FortuneService fortuneService;     public TennisCoach() { }        @Autowired     public void setFortuneService(FortuneService fortuneService) {    this.fortuneService = fortuneService;    }     ... } |
|                                                                                                                                                                                                                                                                              |With adding Autowired annotation, Spring will look for a component that implements the FortuneService interface. In this case, after scanning all the components spring will have a list of components, out of this in this case, only HappyFortuneService implements the FortuneService interface, this HFS meets the requirement.**AFAQ**3. How does @Autowired work internally? 

   1. Best Answer: <https://stackoverflow.com/a/19419296> 
   2. Second best: <https://stackoverflow.com/a/3153617>

4. How is Spring able to inject @Autowired component or implement the @Autowired functionality?

   1. <https://stackoverflow.com/a/3538154>**FAQ**: 1. More than one helper object of type FortuneService? Eg: databaseFortuneService, happyFortuneService, randomFortuneService, RESTFortuneService. Injection of autowired dependencies will fail without specifically mentioning which one to choose. 

   1. Solution? => Use **Qualifiers**, [26-annotation-qualifiers-overview.pdf](https://drive.google.com/file/d/1eSZN2ZIT9qQSLjbBf6XZf6H3JepAsua8/view?usp=share_link) \| [ovwVideo ](https://youtu.be/LdLvhD1PWk0)\|[ codeVid1](https://youtu.be/LdLvhD1PWk0)**


#### Qualifiers


##### **|                                                                                                                                                                                                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Component  public class TennisCoach implements Coach {     private FortuneService fortuneService;     public TennisCoach() { }        @Autowired     @Qualifier("happyFortuneService")//solution    public void setFortuneService(FortuneService fortuneService) {    this.fortuneService = fortuneService;    }    ... } |Spring is designed in a way that if you dont specify qualifier, you can still give the application runner some hints about the bean class by naming the object with the camelcase version of the target bean class name, in this case use like this, use happyFortuneService instead of fortuneService. @Autowired   public void setFortuneService(FortuneService happyFortuneService) {    this.fortuneService = fortuneService;    }**More on Qualifier****AFAQ:** 1. [****Spring @Bean(name ="name") vs @Bean @Qualifier("name")****](https://stackoverflow.com/questions/62822167/spring-beanname-name-vs-bean-qualifiername/76301719#76301719)

   1. **A detailed answer:** [****https://stackoverflow.com/a/76301719/7828981****](https://stackoverflow.com/a/76301719/7828981)
   2. **You can have multiple beans with same Qualifier name but bean name in spring application context needs to be unique**       **@Bean**    **@Qualifier("qualifier1")**    **Foo foo()**    **{**        **return new Foo();**    **}**    **@Bean**    **@Qualifier("qualifier1")**    **Bar bar()**    **{**        **return new Bar();**    **}****The above code is acceptable. but in the case of bean, it is not.**2. **Similar to First Question:** [****java - Why do we use a qualifier when we can have a name for the bean? - Stack Overflow****](https://stackoverflow.com/questions/71841035/why-do-we-use-a-qualifier-when-we-can-have-a-name-for-the-bean)

   1. [****Some important things discussed****](<https://stackoverflow.com/questions/71841035/why-do-we-use-a-qualifier-when-we-can-have-a-name-for-the-bean#:~:text=Beans%20have%20names.%20They%20don%27t%20have%20qualifiers.%20%40Qualifier,test1Repository%22)%20TestRepository%20testRepository)%20%7B%0A%20%20%20%20this.testRepository%3D%20testRepository%3B%0A%7D>)

3. [****Difference between @Qualifier("beanName") and @Component("beanName")****](https://stackoverflow.com/questions/53959005/difference-between-qualifierbeanname-and-componentbeanname#:~:text=%40Component%20is%20used%20to%20declare,eligible%20bean%20for%20that%20injection.)

   1. [****Answer****](https://stackoverflow.com/questions/53959005/difference-between-qualifierbeanname-and-componentbeanname#:~:text=Generally%2C%20you%20use,selected%20by%20default.)

4. **Convention of Bean naming**

   1. [****Bean Naming Conventions (Spring Framework Reference section 1.3.1)****](https://docs.spring.io/spring/docs/5.2.3.RELEASE/spring-framework-reference/core.html#beans-beanname)
   2. [Spring Bean Names | Baeldung](https://www.baeldung.com/spring-bean-names)[Spring @Qualifier Annotation | Baeldung](https://www.baeldung.com/spring-qualifier-annotation)**


#### Annotation Method Injection - [8 Method Injection - YouTube](https://www.youtube.com/watch?v=aiYHdSbPnDs&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=50&ab_channel=freeCodeCampBengali)


##### **Inject dependencies by calling ANY method on your class. Simply give: @Autowired**Step 2**: Configure the dependency injection with Autowired Annotation@Componentpublic class TennisCoach implements Coach {private FortuneService fortuneService;public TennisCoach() {}@Autowiredpublic void doSomeCrazyStuff(FortuneService fortuneService) {this.fortuneService = fortuneService;}...}**


### By Fields - Annotation Field Injection [pdf](https://drive.google.com/file/d/1TACnILb8i_TMM8g9_uV076t45ls5OtTg/view?usp=share_link) [ovvwVid](https://www.youtube.com/watch?v=0iwxLXuOnP0&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=50&ab_channel=freeCodeCampBengali) [codeVid](https://www.youtube.com/watch?v=euoeK-AD8ZE&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=51&ab_channel=freeCodeCampBengali)


##### **Behind the scene, Spring knows it needs to resolve a dependency. **_The first thing spring will do now is call the default constructor that means creating an object of dependent class. Then spring will inject the Implementation of Helper object directly to the dependent class._** This happens during runtime, it is achieved by using Java technology called Reflection.|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| public class TennisCoach implements Coach { //Test Purpose, no use case public TennisCoach() { System.out.println(">TennisCoach: Inside Default Constructor"); }  //Field Injection @Autowired private FortuneService fortuneService;  @Override public String getDailyWorkout() { // TODO Auto-generated method stub return "Run 10 KM"; } @Override public String getDailyFortune() { // TODO Auto-generated method stub return "Tennis Coach Fortune: " + fortuneService.getFortuneService(); }  } |**Output**|                                                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| \> TennisCoach: Inside Default Constructor Run 10 KM Tennis Coach Fortune: Happy New Year, the day will be great Practice penalty kicks FootballCoach Fortune: Happy New Year, the day will be great |**Which one to use? =>** [**11 Which Injection Type Should You Use - YouTube**](https://www.youtube.com/watch?v=uPBg5Y0V4cE&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=52&ab_channel=freeCodeCampBengali)**


### FAQ - Annotation Based


##### **1. How to inject properties file using Java annotations

   1. [074-faq-how-to-inject-properties-file-using-java-annotations.pdf](https://drive.google.com/file/d/1dLltE3a4xZCPXY0N3ERP6SPENdoMg6gc/view?usp=share_link)**


### Bean Scope  - Annotation Field Injection [27-annotations-bean-scopes-overview.pdf](https://drive.google.com/file/d/1py-Wd0cbZE280_aukYkpDbQZYgwaeaEi/view?usp=share_link) video1 video2


##### **Explicitly specifying bean scope:|                                                                                                        |
| ------------------------------------------------------------------------------------------------------ |
| @Component @Scope("singleton") //@Scope("prototype") public class TennisCoach implements Coach { ... } |**


### Bean Lifecycle  - Annotation Field Injection [28-bean-lifecycle-methods-overview.pdf](https://drive.google.com/file/d/11QDO9cCE1Yrydxxi6jiVYtNEvURDp9-a/view?usp=share_link) [ovvwBeanLifeVid](https://www.youtube.com/watch?v=W6ARUEuuE2c&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=58&pp=sAQB) [codeVideo](https://www.youtube.com/watch?v=UcZ0ft6bB30&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=59)


##### **Structure Example|                                                                                                                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Component public class TennisCoach implements Coach { @PostConstruct //Init:Method -> called during bean initialization public void doMyStartupStuff() { ... } @PreDestroy // Destroy:Method -> called during bean destruction public void doMyCleanupStuff() { ... } ... } |Practice Code Example:Practice Codes**


#### Special Note about @PostConstruct and @PreDestroy Method Signatures


##### **I want to provide additional details regarding the method signatures of @PostContruct and @PreDestroy methods.**Access modifier**The method can have any access modifier (public, protected, private)**Return type**The method can have any return type. However, "void' is most commonly used. If you give a return type just note that you will not be able to capture the return value. As a result, "void" is commonly used.**Method name**The method can have any method name.**Arguments**The method can not accept any arguments. The method should be no-arg.**


### Practice Activity


##### **[075-practice-activity-5-dependency-injection-with-annotations.pdf](https://drive.google.com/file/d/1KVjtBPkGiw-zsInysDmVFXR5mxk6giWg/view?usp=share_link)**


## Spring Configuration with Only Java (no XML) 


##### **- [ovvwVid](https://www.youtube.com/watch?v=mmhxp9SV7IE&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=57&ab_channel=freeCodeCampBengali) [codeVid](https://youtu.be/IDUNRhkPpGE)
- [29-java-config-overview.pdf](https://drive.google.com/file/d/1uhiLFQ2xhFLm4TwhZME0pQFXlTumUXzO/view?usp=sharing) 
- [30-java-config-bean-overview.pdf](https://drive.google.com/file/d/1If_g1bbu3B_yMMM3OSdJQ4XZ-m3HMGKv/view?usp=share_link) 
- [31-java-config-inject-props-overview.pdf](https://drive.google.com/file/d/1bDC5Y_GmyBCPV3tAzBR4FjrZUs82ODhb/view?usp=share_link)**


### 3 Ways of Configuring Spring Container


##### ****Full XML:**![](https://lh4.googleusercontent.com/tLSHS9K4l9mBb8VN1uMA5zuGSdtCYr6Ce0wPjpPgRiPNt3m3bEiHwzrjPTcJ9K_kCMl84yXw9bi_KIkClgSlQ5lM3guk1bTJliTSfldZV7K1lv7wuZjXUz9UjGB-IwGoqrIG8BP5_WbEFCZ6--eEEnc)**XML Component Scan: using the component-scan tag**![](https://lh4.googleusercontent.com/tLSHS9K4l9mBb8VN1uMA5zuGSdtCYr6Ce0wPjpPgRiPNt3m3bEiHwzrjPTcJ9K_kCMl84yXw9bi_KIkClgSlQ5lM3guk1bTJliTSfldZV7K1lv7wuZjXUz9UjGB-IwGoqrIG8BP5_WbEFCZ6--eEEnc)- Use @Component annotation at the bean definition class + Use @Autowire Annotation at the place where the bean will be used**Java Configuration Class: using componentScan annotation**![](https://lh6.googleusercontent.com/-OuCEShN-rKu0vP3OB_UoVv6ndzb5XpvfdcSl4LEmW9SDSf03IHG3rzeiuX7_ckCszQ9QP0u5nhyZp_2tjCRJJVVdgxJV1CHrxt_Tt2xBdjfVjgauK3l6IXSydFO1P7fnQdCgS-3LAUwyHVgGqniK-w)- Use @Component annotation at the bean definition class + Use @Autowire Annotation at the place where the bean will be used Or Define a new Bean with @Bean annotation**


### 2 Ways to Define Bean when we only use Java


##### **1. **Option 1**: Write a class, add @Comonenet annotation, and then use @ComponentScan annotation inside configuration so that it can find all the class which used @Component annotation to add those class as Beans into the Spring Container.
2. **Option 2:** Write a method inside configuration class, add @Bean annotation, it will automatically add the new Bean into the Spring Container. ****Example: [ Defining Beans Inside Configure Class](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.4c1c9iythpwc). Note @Bean is a method level annotation, thus have some limitations. You can not set qualifier.@Bean    //@Qualifier("personOne") - doesn't work - bean qualifier is method name    public Person personOne() {        return new Person("Joe", "Smith");    }**


### Development Process (only Java, no XML) using the ComponentScan annotation


#### **Step 1**: Create a Java class and annotate as **@Configuration**


##### **|                                             |
| ------------------------------------------- |
| @Configuration public class SportConfig { } |**


#### **Step 2**: Add component scanning support: **@ComponentScan(optional)**


##### **|                                                                                       |
| ------------------------------------------------------------------------------------- |
| @Configuration @ComponentScan("com.luv2code.springdemo") public class SportConfig { } |Or, Instead of Using @ComponentScan() we can define beans inside the Config file and then use them.**


#### **Step 3**: Read Spring Java configuration class


##### **|                                                                                                         |
| ------------------------------------------------------------------------------------------------------- |
| AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(SportConfig.class); |**


#### **Step 4**: Retrieve bean from Spring container


##### **|                                                               |
| ------------------------------------------------------------- |
| Coach theCoach = context.getBean("tennisCoach", Coach.class); |**


### Defining Beans Inside Configure Class - optional @Component annotation and @ComonentScan annotation (**Alternative Bean Defining)**


##### **Read the Documnetation - [2.2. @Bean (spring.io)](https://docs.spring.io/spring-javaconfig/docs/1.0.0.M4/reference/html/ch02s02.html)No @Component annotation, if all the Beans are defined like this no @ComonentScan needed as wellStep 1: Define method to expose bean|                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------- |
| @Configuration public class SportConfig { @Bean public Coach swimCoach() { SwimCoach mySwimCoach = new SwimCoach();  return mySwimCoach; } } |Step 2: Inject bean dependencies|                                                                                                                                                                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Configuration public class SportConfig { @Bean public FortuneService happyFortuneService() { return new HappyFortuneService(); } @Bean public Coach swimCoach() { SwimCoach mySwimCoach; //constructor InjectionmySwimCoach = new SwimCoach( happyFortuneService() ); return mySwimCoach; } } |Step 3: Read Spring Java configuration class|                                                                                                         |
| ------------------------------------------------------------------------------------------------------- |
| AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(SportConfig.class); |Step 4: Retrieve bean from Spring container|                                                             |
| ----------------------------------------------------------- |
| Coach theCoach = context.getBean("swimCoach", Coach.class); |**AFAQ**1. Understanding Spring Configuration Class

   1. [java - Understanding spring @Configuration class - Stack Overflow](https://stackoverflow.com/questions/24014919/understanding-spring-configuration-class)

2. Instantiating multiple beans of the same class with Spring annotations - 

   1. [Instantiating multiple beans of the same class with Spring annotations - Stack Overflow](https://stackoverflow.com/questions/2902335/instantiating-multiple-beans-of-the-same-class-with-spring-annotations)
   2. **One Way:**@Configurationpublic class PersonConfig {    @Bean    public Person personOne() {        return new Person("Joe", "Smith");    }    @Bean    public Person personTwo() {        return new Person("Mary", "Williams");    }}3. Accepted answer shown **another way** - <https://stackoverflow.com/a/2903373/7828981>3. Do we use @Autowire inside Configutation class annotated with @Configutation?

   1. Depends on the Situation 

      1. **Situation one:** If your are Trying to Inject a Bean defined outside of that particular Configuration class and also outside of other Configration class then you do not need to use @Autwired. See An example: <https://stackoverflow.com/a/32079923/7828981>

      2. **Situation Two:** But if you are Trying to Inject a Bean defined Inside another Configuration class, then you need to use @Autowire. In simple, You need autowire if you inject between different configuration classes. Example : [4.2. Referencing beans across @Configuration classes (spring.io)](https://docs.spring.io/spring-javaconfig/docs/1.0.0.M4/reference/html/ch04s02.html)

         1. **Way one**:**File: config1.java**@Configuration**public** **class** ConfigOne {    @Bean    **public** AccountRepository accountRepository() {        _// create and return an AccountRepository object_    }}**File: config2.java**@Configuration@AnnotationDrivenConfig**public** **class** ConfigTwo {    @Autowired AccountRepository accountRepository;    @Bean    **public** TransferService transferService() {        **return** **new** TransferServiceImpl(accountRepository);    }}**File: app.java**JavaConfigApplicationContext context =    **new** JavaConfigApplicationContext(ConfigOne.**class**, ConfigTwo.**class**);2. **Way 2**: Fully-qualified bean references with @Autowired; ( **Preferred )****File: config1.java**@Configuration**public** **class** ConfigOne {    @Bean    **public** AccountRepository accountRepository() {        _// create and return an AccountRepository object_    }}**File: config2.java**@Configuration@AnnotationDrivenConfig**public** **class** ConfigTwo {    @Autowired ConfigOne configOne;    @Bean    **public** TransferService transferService() {         _// transferService references accountRepository in a 'fully-qualified' fashion:_        **return** **new** TransferServiceImpl(configOne.accountRepository());    }}[DefiningBeanVid](https://youtu.be/1UTte5VLeTY) [codeVid](https://youtu.be/9pR_rq8FcXc) [codeVid2](https://youtu.be/2atQPVIpVpo)**FAQ**1. [spring - What happens when I declare beans and component-scan both in applicationContext.xml? - Stack Overflow](https://stackoverflow.com/questions/55702499/what-happens-when-i-declare-beans-and-component-scan-both-in-applicationcontext)
2.**


### Injecting Values from Properties File


##### ****Step 1**: Create Properties File File: sport.properties|                                                                 |
| --------------------------------------------------------------- |
| foo.email=myeasycoach@luv2code.com foo.team=Awesome Java Coders |**Step 2**: Load Properties file in Spring configFile: SportConfig.java|                                                                                               |
| --------------------------------------------------------------------------------------------- |
| @Configuration @PropertySource("classpath:sport.properties") public class SportConfig { ... } |**Step 3**: Reference Values from Properties FileFile: SwimCoach.java|                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------- |
| public class SwimCoach implements Coach {@Value("${foo.email}") private String email; @Value("${foo.team}") private String team; ... } |[InjectValuesFromPropertieFileVid](https://youtu.be/znY04US-plM) [codeVid](https://youtu.be/lHNabRQwTno) [codeVid2](https://youtu.be/p0LH21jqySM) [31-java-config-inject-props-overview.pdf](https://drive.google.com/file/d/1bDC5Y_GmyBCPV3tAzBR4FjrZUs82ODhb/view?usp=share_link)FAQ1. [understanding Classpath](https://stackoverflow.com/a/53697594)* * *Spring MVC[Spring MVC official documents](https://docs.spring.io/spring-framework/docs/current/reference/html/web.html)A spring framework based on mv design pattern for web application in java.**


# Chapter 1: Behind the Scene of Spring MVC


##### **[02-spring-behind-the-scenes.pdf](https://drive.google.com/file/d/1poHKHXBqdDd98qNwMMc93UFUQKVs8Z3Z/view?usp=share_link)**


### Components of Spring MVC Application


##### **- A set of **web pages** to layout UI components
- A collection of **Spring beans** (controllers, services, etc...)
- **Spring configuration** (XML, Annotations or Java)![](https://lh6.googleusercontent.com/R1kSoUoZvfQg5FrlphfsgnkRiLQmhtGyiu53bYz2TI6Nwo8qBB0zRyQxKbwCednAu7ISfatvWsiZe6G0f52khj6AHUSOtzxbWp9lm5BRJTdEfYKOoJWci9dMcY3-454p4MiEGnbfejYkFCaN5V7HyF4)**


# Chapter 2: Dev Environment Setup


##### **[03-spring-dev-environment-checkpoint.pdf](https://drive.google.com/file/d/1_Tpbow6CzedxZpKRqYCoewM947QQBsHx/view?usp=sharing)**


## Section 1: Initial Setup


#### Tomcat Version 


##### **- New version of Tomcat 10 was released to support Jakarta EE 9
- Renamed packages: javax.\* to jakarta.\*
- This is a breaking change for Java EE apps
- Spring 5 currently does not support the new package renaming Jakarta EE 9
- As a result, Spring 5 does not currently work on Tomcat 10
- **Use Tomcat 9 for your Spring 5 apps**➤ [java - Tomcat: How to find out running Tomcat version? - Stack Overflow](https://stackoverflow.com/questions/14925073/tomcat-how-to-find-out-running-tomcat-version)**


#### Additional


##### **1. Download Spring MVC source code for this training class - [Download](https://drive.google.com/file/d/1iyeTgY0A4N_qduo2_-5thUI9Og0ZHOGx/view?usp=share_link)
2. Download latest Spring JAR files from Spring website - [JFrog (spring.io)](https://repo.spring.io/ui/native/release/org/springframework/spring/)**


## Section 2: Spring MVC Configuration


##### **Part 0: 1. Change the perspective of the IDE Window > Perspective > Other > Java EE
2. Open a new project > Select Dynamic Web Project > Enter Finish![](https://lh3.googleusercontent.com/ddhMYdppVQ4H_GrQuTM6Uz6b_lUnru76SEJ2LI9fVEok58ofTs20BnU5spaao0P9VmoTyYyBCJ8MC4G2GQtseEOlIEQG9Zgpc0l5ePiBSa0Dxot-ZwXqB6rz5SkWOX5aRxJ2XFxKLI7gzZ_dADR9av4)**Copy and paste contents in lib folder**3. Copy the jar files from Spring Framework located inside lib folder and paste them at _/spring-mvc-demo/src/main/webapp/WEB-INF/lib_
4. Copy the jar files from MVC Starter Project located [_spring-mvc-config-files\\spring-mvc\\starter-files\\spring-mvc-demo\\lib_](https://drive.google.com/drive/folders/1IjTumjdod03hH_Evjfc8Cc6cwj0EzIXO?usp=share_link) and paste them at _/spring-mvc-demo/src/main/webapp/WEB-INF/lib_**Copy and paste two xml files (**_web.xml_ ****and _spring-mvc-demo-servlet.xml_**) in web-inf folder**5. Copy the two xml files from MVC Starter Project located [__spring-mvc-config-files\\spring-mvc\\starter-files\\spring-mvc-demo\\config__](https://drive.google.com/drive/folders/1IjTumjdod03hH_Evjfc8Cc6cwj0EzIXO?usp=share_link) and paste them in your project at _/spring-mvc-demo/src/main/webapp/WEB-INF/lib_**


### Spring MVC Configuration Process - Part 1


##### **Add configurations to file: WEB-INF/web.xml1. Configure Spring MVC Dispatcher Servlet
2. Set up URL mappings to Spring MVC Dispatcher Servlet**


### Spring MVC Configuration Process - Part 2


##### **Add configurations to file: WEB-INF/spring-mvc-demo-servlet.xml1. Add support for Spring component scanning, don't forget to change the component scanning base package as per your project.
2. Add support for conversion, formatting and validation
3. Configure Spring MVC View Resolver**


#### Step 1: Configure Spring DispatcherServlet


##### **&lt;web-app>&lt;servlet>&lt;servlet-name>dispatcher&lt;/servlet-name>&lt;servlet-class>org.springframework.web.servlet.DispatcherServlet&lt;/servlet-class>&lt;init-param>&lt;param-name>contextConfigLocation&lt;/param-name>&lt;param-value>/WEB-INF/spring-mvc-demo-servlet.xml&lt;/param-value>&lt;/init-param>&lt;load-on-startup>1&lt;/load-on-startup>&lt;/servlet>&lt;/web-app>**


#### Step 2: Set up URL mappings to Spring MVC Dispatcher Servlet


##### **&lt;web-app>&lt;servlet>&lt;servlet-name>dispatcher&lt;/servlet-name>&lt;servlet-class>org.springframework.web.servlet.DispatcherServlet&lt;/servlet-class>...&lt;/servlet>&lt;servlet-mapping>&lt;servlet-name>dispatcher&lt;/servlet-name>&lt;url-pattern>/&lt;/url-pattern>&lt;/servlet-mapping>&lt;/web-app>File: web.xml**


#### Step 3: Add support for Spring component scanning


##### **&lt;beans>&lt;!-- Step 3: Add support for component scanning -->&lt;context:component-scan base-package="com.luv2code.springdemo" />&lt;/beans>File: spring-mvc-demo-servlet.xmlwww.luv2code.com**


#### Step 4: Add support for conversion, formatting and validation


##### **&lt;beans>&lt;!-- Step 3: Add support for component scanning -->&lt;context:component-scan base-package="com.luv2code.springdemo" />&lt;!-- Step 4: Add support for conversion, formatting and validation support -->&lt;mvc:annotation-driven/>&lt;/beans>File: spring-mvc-demo-servlet.xmlwww.luv2code.com**


#### Step 5: Configure Spring MVC View Resolver


##### **&lt;beans>&lt;!-- Step 3: Add support for component scanning -->&lt;context:component-scan base-package="com.luv2code.springdemo" />&lt;!-- Step 4: Add support for conversion, formatting and validation support -->&lt;mvc:annotation-driven/>&lt;!-- Step 5: Define Spring MVC view resolver -->&lt;beanclass="org.springframework.web.servlet.view.InternalResourceViewResolver">&lt;property name="prefix" value="/WEB-INF/view/" />&lt;property name="suffix" value=".jsp" />&lt;/bean>&lt;/beans>[What does the InternalResourceViewResolver do in Spring MVC? - Java Code Geeks - 2023](https://www.javacodegeeks.com/2017/08/internalresourceviewresolver-spring-mvc.html)**


### Spring MVC Configuration Process - Part 3 (Additional)


##### **1. Add Additional folder or files as per the requirement of the project. Such as Create a View folder to store the view pages(html pages).
2.**


## Section 3: Java Spring (MVC) Configuration Files


##### **Each version of a service is defined in a .yaml file, which gives the name of the service and version. You can Typically, you create a directory for each service, which contains the service's YAML files and associated source code. Optional application-level configuration files (dispatch.yaml, cron.yaml, index.yaml, and queue.yaml) are included in the top level app directory. The example below shows three services. In service1 and service2, the source files are at the same level as the YAML file. In service3, there are YAML files for two versions.![](https://lh3.googleusercontent.com/tLdsQl0Nh00sOp70w4Gg-B02RBIXgGUtqpnze1GPsveNwYCmQpimS5Kk7vR5c_ts6RHu07YaDNt3hhPaUArEN6MqqaxM7P-UQ3WqfHnLQCv9RIN10svaV031oL03nN41XJ7KuwmaPOBkiThawMjf55I)For small, simple projects, all the app's files can live in one directory:![](https://lh3.googleusercontent.com/DjJf9UsTrAZQBFzzPHZw-SKRbnTV7DUibevwcjkqWUsIpuQzVhtq78rYJm5Q252fMvU6GoeNNPHuE1gYoTxr5ezGSWUy8fGkOfXPb-oxrtz5W7i64wHX1Mt84kai5-3wu5PI7r8B0tiZ0ToJStwSl_4)**Every YAML file must include a version parameter**. To define the default service, you can explicitly include the parameter **service: default** or leave the service parameter out of the file.**


### The default service


##### **Every application has a single default service. You can define the default service in the appengine-web.xml with the setting service: default, but it isn't necessary to do this. All configuration parameters relevant to services can apply to the default service.**


### Optional configuration files


##### **These configuration files control optional features that apply to all the services in an app:- [dispatch.yaml](https://cloud.google.com/appengine/docs/legacy/standard/java/reference/dispatch-yaml) overrides routing default rules by sending incoming requests to a specific service based on the path or hostname in the URL.
- [queue.yaml](https://cloud.google.com/appengine/docs/legacy/standard/java/config/queueref) configures both push queues and pull queues.
- [index.yaml](https://cloud.google.com/appengine/docs/legacy/standard/java/configuring-datastore-indexes-with-index-yaml) specifies which indexes your app needs if using Datastore queries.
- [cron.yaml](https://cloud.google.com/appengine/docs/legacy/standard/java/config/cronref) configures regularly scheduled tasks that operate at defined times or regular intervals.To deploy updates of these configuration files to App Engine, run the following command from the directory where they are located:**


### The Deployment Descriptor: **web.xml**


##### **Java web applications use a deployment descriptor file to determine how URLs map to servlets, which URLs require authentication, and other information. This file is named web.xml, and resides in the app's WAR under the WEB-INF/ directory. web.xml is part of the servlet standard for web applications.**


#### Servlets and Servlet Mapping


##### **To map a URL to a servlet, you declare the servlet with the &lt;servlet> element, then define a mapping from a URL path to a servlet declaration with the &lt;servlet-mapping> element. In depth details from here**:** [**web.xml: Servlets and URL paths | Google cloud**](https://cloud.google.com/appengine/docs/legacy/standard/java/config/webxml#routing)Read more about web.xml: [The Deployment Descriptor: web.xml  |  App Engine standard environment for Java 8  |  Google Cloud](https://cloud.google.com/appengine/docs/legacy/standard/java/config/webxml)**An Simple Example:** [**Deployment Descriptor: web.xml file - W3schools**](https://www.w3schools.blog/deployment-descriptor-web-xml-file)**


### **web.xml** Deployment Descriptor Elements


##### **Read: [A web.xml Deployment Descriptor Elements (oracle.com)](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#WBAPP502)- [web.xml Namespace Declaration and Schema Location](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#CIHFAIDA)
- [icon](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1070114)
- [display-name](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1043406)
- [description](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023813)
- [distributable](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1044010)
- [context-param](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023821)
- [filter](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1039711)
- [filter-mapping](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1039712)
- [listener](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1039713)
- [servlet](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1022718)
- [servlet-mapping](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023837)
- [session-config](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023849)
- [mime-mapping](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023915)
- [welcome-file-list](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1026979)
- [error-page](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023942)
- [jsp-config](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1071164)
- [resource-env-ref](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1046316)
- [resource-ref](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023962)
- [security-constraint](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023046)
- [login-config](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1023261)
- [security-role](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1025309)
- [env-entry](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1025194)
- [ejb-ref](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1024081)
- [ejb-local-ref](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1046334)
- [web-app](https://docs.oracle.com/cd/E21764_01/web.1111/e13712/web_xml.htm#i1069725)**


## Query: 


##### **- How does the web.xml work? => _When a request comes it is matched with the url pattern in the servlet mapping attribute. When a match is found , control goes to the associated servlet class._
- spring-mvc-demo-servlet.xml works? => **


## FAQ: configure the Spring Dispatcher Servlet using all Java


##### **How to configure the Spring Dispatcher Servlet using all Java Code (no xml)? => [103-faq-how-to-configure-the-spring-dispatcher-servlet-using-all-java-code-no-xml.pdf](https://drive.google.com/file/d/16PO21sRWg4HJDfuWe1CAdICdcl2CjQoX/view?usp=share_link)**


# Chapter 3: Spring MVC


##### ** [04-spring-mvc-configuration-overview.pdf](https://drive.google.com/file/d/1pqvu-vD2lCA7A6E4klwrkmfs-JI1QTsS/view?usp=share_link)A Spring MVC is a Java framework which is used to build web applications. It follows the Model-View-Controller design pattern. It implements all the basic features of a core spring framework like Inversion of Control, Dependency Injection.A Spring MVC provides an elegant solution to use MVC in spring framework by the help of **DispatcherServlet**. Here, **DispatcherServlet** is a class that receives the incoming request and maps it to the right resource such as controllers, models, and views.![](https://lh6.googleusercontent.com/R1kSoUoZvfQg5FrlphfsgnkRiLQmhtGyiu53bYz2TI6Nwo8qBB0zRyQxKbwCednAu7ISfatvWsiZe6G0f52khj6AHUSOtzxbWp9lm5BRJTdEfYKOoJWci9dMcY3-454p4MiEGnbfejYkFCaN5V7HyF4)Figure: Spring Web Model-View-Controller- **Model** - A model contains the data of the application. A data can be a single object or a collection of objects.

  - Model: contains your data

  - Store/retrieve data via backend systems

    -  database, web service, etc…
    - Use a Spring bean if you like

  - Place your data in the model

    - Data can be any Java object/collection

- **Controller** - A controller contains the business logic of an application. Here, the @Controller annotation is used to mark the class as the controller.

  - Code created by developer

  - Contains your business logic

    -  Handle the request
    - Store/retrieve data (db, web service...)
    -  Place data in model

  - Send to appropriate view template

- **View** - A view represents the provided information in a particular format. Generally, JSP+JSTL is used to create a view page. Although spring also supports other view technologies such as Apache Velocity, Thymeleaf and FreeMarker.

  - Spring MVC is flexible

    - Supports many view templates

  - Most common is JSP + JSTL

  - Developer creates a page

    - Displays data

  - Other view templates supported

    - Thymeleaf, Groovy
    - Velocity, Freemarker, etc...

- **Front Controller** - In Spring Web MVC, the DispatcherServlet class works as the front controller. It is responsible for managing the flow of the Spring MVC application. Already developed by Spring Dev Team. 

  - Front controller known as DispatcherServlet

    -  Part of the Spring Framework
    - Already developed by Spring Dev Team

  - You will create,

    - You will createModel objects (orange)
    -  View templates (dark green) 
    - Controller classes (yellow)**


### Understanding the flow of Spring Web MVC


##### **![Spring MVC Tutorial](https://lh4.googleusercontent.com/wzMN-Wce2mUF9c8PYqLgiJ4vNBw-lv1JOpgEEom0K6f_h7a15LNunUJk7DZM9mLUwL0oB0_w-v179AWSBIjVxV8HOLaTK6reNw0KwBe5_dYzDa1NoNO-PB-JZuHzyAoIlP5SR9R_aHmR5fQArEnIusU)- As displayed in the figure, all the incoming requests are intercepted by the DispatcherServlet that works as the front controller.
- The DispatcherServlet gets an entry of handler mapping from the XML file and forwards the request to the controller.
- The controller returns an object of ModelAndView.
- The DispatcherServlet checks the entry of the view resolver in the XML file and invokes the specified view component.**


### Spring: Data Binding


## FAQ


##### **@Controller inherits @Component, how!!! => <https://stackoverflow.com/questions/7761513/is-there-something-like-annotation-inheritance-in-java>**


## Part 1. Spring MVC - Creating a Spring Home Controller and View - 


### Creating a Spring Home Controller and View - [05-spring-mvc-home-controller-overview.pdf](https://drive.google.com/open?id=1HmKWwlLWVpilf_pSOEEYdMtS665RID8I&usp=drive_copy)


##### **package com.diptopaul.springdemo.mvc;import org.springframework.stereotype.Controller;import org.springframework.web.bind.annotation.RequestMapping;|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| package com.diptopaul.springdemo.mvc; import org.springframework.stereotype.Controller; import org.springframework.web.bind.annotation.RequestMapping; @Controller public class HomeController { @RequestMapping("/") public String showPage() { // this method is only returning the view page name as a string. Internally Spring will add suffixes and prefixes using this name and then spring will find the page from the view folder and then show the page to the user. return "main-menu"; } } |FAQ:[ HELP! My Spring MVC Controller is not working. What to do?](https://drive.google.com/open?id=16SWZrcwLSPOB_btUf_HxCgN0tVX-ZHFR&usp=drive_copy)FAQ: [HELP! - Can't Start Tomcat - Ports are in Use!](https://drive.google.com/open?id=18ITVMOUgm1Nj7lk737rwoAv9-AcMzk8d&usp=drive_copy)AFAQ: HELP! - Can’t Start Tomcat - One or more ports are invalid - [Solution](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.aizx2wgjop2k)FAQ: [How Does Component Scan Work - Your Package Names are Different!](https://drive.google.com/file/d/1pL9skkdTTdV8i5WlSmJ3y5gFYfSoCd8b/view?usp=share_link)**


### Reading HTML Form Data Overview - [06-spring-mvc-hello-world-form-and-model-overview.pdf](https://drive.google.com/open?id=10uTx4ELEFYVc63C2ljcEfakOjqAyWTO-&usp=drive_copy)


##### **|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| package com.diptopaul.springdemo.mvc; import org.springframework.stereotype.Controller; import org.springframework.web.bind.annotation.RequestMapping; @Controller public class HomeController { @RequestMapping("/") public String showPage() { // this method is only returning the view page name as a string. Internally Spring will add suffixes and prefixes using this name and then show the page to the user. return "main-menu"; } @RequestMapping("/showForm") public String showForm() { return "helloworld-form";// the actual form html page that will receive input } @RequestMapping("/processForm") public String processForm() { return "helloworld"; // the actual page that will use the input received from the form } } |**


### Adding Data to the Spring Model - [Model, ModelMap, and ModelAndView in Spring MVC | Baeldung](https://www.baeldung.com/spring-mvc-model-model-map-model-view)


##### **[07-spring-mvc-adding-data-to-model-overview.pdf](https://drive.google.com/open?id=18KDTc9TYa6BcmZAFSpr2G4eEwpNJjEV5&usp=drive_copy)\| [OvwVid](https://youtu.be/gk4zkRgS0HU?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [CodeVid1](https://youtu.be/DEordvvsLRs?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [CodeVid2](https://youtu.be/qLPXD2OMkRU?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)**What is a Model and Why is it used for?**In Spring MVC, the Model is an Interface which works as a container that contains the data of the application.**Simply put, the model can supply attributes used for rendering views.**To provide a view with usable data, we simply add this data to its Model object. And the object of HttpServletRequest reads the information provided by the user and passes it to the Model interface.**


#### Spring MVC Model Methods and Syntax


##### **Read and Check,1. [Spring MVC - Model Interface - GeeksforGeeks](https://www.geeksforgeeks.org/spring-mvc-model-interface/) \*\*
2. [Spring MVC Model Interface - javatpoint](https://www.javatpoint.com/spring-mvc-model-interface)**Passing Model to your Controller Method**,|                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @RequestMapping("/processFormVersionTwo") public String letsShoutDude(HttpServletRequest request, Model model) { // read the request parameter from the HTML form String theName = request.getParameter("studentName"); // convert the data to all caps theName = theName.toUpperCase(); // create the message String result = "Yo! " + theName; // add message to the model model.addAttribute("message", result);// return "helloworld"; } |**View Template - JSP**|                                                                                            |
| ------------------------------------------------------------------------------------------ |
| &lt;html>&lt;body> Hello World of Spring! ... The message: ${message} &lt;/body>&lt;/html> |FAQ: [How to use CSS, JavaScript and Images in Spring MVC Web App](https://drive.google.com/file/d/1WNMvJ7QTTED8JggEYOJK7nInXmQMKnAi/view?usp=share_link) FAQ: [Deploying To Tomcat using WAR files](https://drive.google.com/open?id=1-1PSxUHArGqrmSo6JlA4dqKUiZSKJiYz&usp=drive_copy) **


## Part 2. Spring MVC - Request Param and Request Mapping


### Binding Request Params


##### **[08-spring-mvc-binding-request-params-overview.pdf](https://drive.google.com/open?id=1axsL6r4UhsWfQRW5QmYQorA01q0Va8aS&usp=drive_copy) \| [OvwVid](https://youtu.be/3ic0ff-k0I0?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [CodeVid1](https://youtu.be/9wKB8FAMO6E?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)Instead of using **HttpServletRequest**|                                                                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @RequestMapping("/processFormVersionTwo") public String letsShoutDude(HttpServletRequest request, Model model) { // read the request parameter from the HTML form String theName = request.getParameter("studentName"); ... } |Bind variable using **@RequestParam** Annotation|                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @RequestMapping("/processFormVersionTwo") public String letsShoutDude(@RequestParam("studentName") String theName, Model model) { // now we can use the variable: theName } |**


### Controller Level Request Mapping


##### **[09-spring-mvc-request-mapping-for-controller-overview.pdf](https://drive.google.com/open?id=1iEU35kmmWNq-x_iRjbLj-IEVWGrQzx7n&usp=drive_copy) \| [OvwVid](https://youtu.be/5zIqSlzTN3A?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [CodeVid1](https://youtu.be/sCC5LAcIdWE?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [CodeVid2](https://youtu.be/29CcTt5DTls?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)Why do we need this?Imagine two different controller classes have the same RequestMapping path (consider “/funny”) for their respective RequestMethod, if we request for the resource with “/funny” path, it will produce an Ambiguous mapping error. Controller Level Request Mapping can solve this issue by having a different path name for the use of Request Mapping for the Controller class.Controller Request Mapping|                                                                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Controller@RequestMapping("/funny") class FunnyController {  @RequestMapping("/showForm") // => /funny/showForm public String showForm() { ... }  @RequestMapping("/processForm")// => /funny/processForm public String process(HttpServletRequest request, Model model) { ... } } |FAQ: [How does "processForm" work for "/hello"?](https://drive.google.com/open?id=1SGJYgBn4eSkPO-9Yd5SXYDY7vsYSBSHz&usp=drive_copy)**


## Part 3. Spring MVC - Form Tags and **Data Binding**


##### **Spring MVC Data Binding with @ModelAttribute annotation works as two way data binding.**


### Spring MVC Form Library


##### **[10-spring-mvc-form-tags-overview.pdf](https://drive.google.com/open?id=13Ef4vKkb5TQz9P-Gil9ck6puCgc1BuDn&usp=drive_copy) [ovwVid](https://youtu.be/JamIk-q-kYo?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)Understand more about Spring MVC Form tag and its library: 1. [Spring MVC Form Tag - JavaTPoint](https://www.javatpoint.com/spring-mvc-form-tag-library#:~:text=The%20Spring%20MVC%20form%20tags,and%20also%20retrieve%20from%20it.)
2. [Spring MVC JSP Form Tags Tutorial (javaguides.net)](https://www.javaguides.net/2018/10/spring-mvc-jsp-form-tags-tutorial.html)Data Binding- Spring MVC Form Tags can make use of data binding
- Automatically setting / retrieving data from a Java object / beanSpring MVC Form Tags|                  |                       |
| ---------------- | --------------------- |
| Form Tag         |  Description          |
| form:form        | main form container   |
| form:input       | text field            |
| form:textarea    | multi-line text field |
| form:checkbox    | check box             |
| form:radiobutton | radio buttons         |
| form:select      | drop down list        |
| more ....        |                       |How To Reference Spring MVC Form Tags- Specify the Spring namespace at beginning of JSP file|                                                                                    |
| ---------------------------------------------------------------------------------- |
| &lt;%@ taglib prefix="form" uri="http&#x3A;//www.springframework.org/tags/form" %> |**


### List of tags in Spring MVC Form Library


##### **- Form Tag: Covered above.
- [Text Fields](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.9s7rc9n4nnak)
- [Drop-Down Lists - Overview](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.dwuno1onelxw) | FAQ: Use properties file to load country options 
- [Radio Buttons - Overview](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.nqv0fafcgexq) | FAQ: How to populate radio buttons with items from Java class?
- [Checkboxes - Overview](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.2h5r2o50xls5)**


#### Text Fields


##### **[11-form-tags-textfield-overview.pdf](https://drive.google.com/open?id=1eCqo7ZT7F8CquNStl8Temyh5yQMj-2Mj&usp=drive_copy) [ovwVid](https://youtu.be/llt9sF-u96k?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [codeVid1 codeVid2](https://youtu.be/y0vSSrezpks?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H) [codeVid3](https://youtu.be/nkT-I4Ux6LI?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)|                                                                                                                                                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;form:form action="processForm" modelAttribute="student"> firstName: &lt;form:input path="firstName"/> &lt;input type="submit" value="submit"/> &lt;!--only the input that will bind need to have the form prefix, this one is normal html input tag--> &lt;/form:form> |**AFAQ**- How will spring read the value from form and set the value to student object?

  - In the &lt;form:input path="firstName"/> tag, path attribute having the value “firstName” indicates that it has a data binding relationship with the corresponding spring variable. The question is, **how do they work internally?** Internally spring knows the student object is added to the model object as a modelAttribute (already done in controller class), this object is named as “student”. Now spring needs to find out what setter method it needs to call to set the user provided value inside from the form. The special attribute named **path** inside the form:input tag comes into play this time. Spring will take the path attribute value (in this case “firstName”) , convert it to [PascalCase](https://www.theserverside.com/definition/Pascal-case) (=>FirstName) and then add “set” as prefix. Thus it can call the setFirstName() setter method and set the input value to the student object's firstName variable.

    - set + firstName => setFirstName  => setFirstName (“theInputValueProvided by the user”)Development process: Step by step1. Create a Student class => 
2. Create a Student controller class
3. Create HTML form (JSP file)
4. Create form processing code => form processing controller method
5. Create confirmation pageRead the [Baeldung Article](https://www.baeldung.com/spring-mvc-form-tutorial) for more clarity.**Step 1**: Student class📂 Student.class|                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| package com.diptopaul.springdemo.mvc; public class Student { private String firstName; private String lastName;  public Student() {  }  public String getFirstName() { return firstName; } public void setFirstName(String firstName) { this.firstName = firstName; } public String getLastName() { return lastName; } public void setLastName(String lastName) { this.lastName = lastName; } } |**Step 2**: Student controller class📂 StudentController.class|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| package com.diptopaul.springdemo.mvc; import org.springframework.stereotype.Controller; import org.springframework.ui.Model; import org.springframework.web.bind.annotation.RequestMapping; @Controller @RequestMapping("/student") public class StudentController {  @RequestMapping("/showForm") public String showForm(Model theModel) { //create a object Student theStudent = new Student(); //add the object in the Model theModel.addAttribute("student", theStudent); return "student-form"; } } |**Explanation**: @RequestMapping("/showForm")public String showForm(Model model) {Student theStudent = new Student ();// this will work, maybe they consider the default bean name(here customer) of the Student object as the target bean of the form.//model.addAttribute(theStudent );// this will not work, the target object (according to the form) for bean name customer is not available. Maybe this works as like having a user defined bean id, just like we did with @Component("tennisCoach")//model.addAttribute("weird", theStudent);//if we change "weird" to "customer" (target name mentioned at jsp form) it will work.model.addAttribute("customer", theStudent);return "customer-form";}Note: Now consider,  the student object is added to the model as a model object. Initially all the values will be empty in the target bean. Since form and the model object is binded. Form can get the values from the model object using the path attribute, which will help us to know the getter and setter method. Incase of setting values, when submit is performed spring will call the setter method and will make the changes in the object model.One thing to notice here is, we did not have to explicitly add all the data from the html tag here, for example: adding firstName to the Student object, (then adding the student object to the model). Spring will update the data to the student object, as the form and student attribute of the model are binded. All we explicitly need to do here is add the Student object to the model object.**Step 3**: JSP html student form📂 view/student-form.jsp|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%@ taglib prefix="form"uri="http&#x3A;//www.springframework.org/tags/form"%> &lt;%@ page language="java" contentType="text/html; charset=ISO-8859-1"     pageEncoding="ISO-8859-1"%> &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Student Information Form&lt;/title> &lt;/head> &lt;body> &lt;h1>Fill up the student information form&lt;/h1> &lt;form:form action="processForm" modelAttribute="student"> Firtname: &lt;form:input path="firtName"/> &lt;br>&lt;br> Lastname: &lt;form:input path="lastName"/> &lt;br>&lt;br> &lt;input type="submit" value="submit"/> &lt;/form:form> &lt;/body> &lt;/html> |First – notice that we're including a tag library into our JSP page – the form taglib – to help with defining our form.Next – the &lt;form:form> tag plays an important role here; it’s very similar to the regular HTML &lt;form> tag but [the modelAttribute attribute](https://www.baeldung.com/spring-mvc-form-tutorial#:~:text=the%20modelAttribute%20attribute%20is%20the%20key%20which%20specifies%20a%20name%20of%20the%20model%20object%20that%20backs%20this%20form) is the key which specifies a name of the model object that backs this form:&lt;form:form action="processForm" modelAttribute="student">This will correspond to the @ModelAttribute later on in the controller.Next – each input field is using yet another useful tag from the Spring Form taglib – form: prefix. Each of these fields specifies a path attribute – this must correspond to a getter/setter of the model attribute (in this case, the Student class). When the page is loaded, the input fields are populated by Spring, which calls the getter of each field bound to an input field. When the form is submitted, the setters are called to save the values of the form to the object.Finally – when the form is submitted, the POST handler in the controller is invoked and the form is automatically bound to the student argument that we passed in.**Step 4:** form processing code: adding process control method etc📂 StudentController.java (updated)|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| package com.diptopaul.springdemo.mvc; @Controller @RequestMapping("/student") public class StudentController {  @RequestMapping("/showForm") public String showForm(Model theModel) { //create a student object Student theStudent = new Student();  //add the student object as an attribute in the Model theModel.addAttribute("student", theStudent); return "student-form"; }  @RequestMapping("/processForm")//processing form after submission //@ModelAttribute annotation binds form data to the object, explanation: since the form has the same modelAttribute name(here "student") as the controller Model object's attribute, any changes in the form that will change the student object will also reflect the change in the modelAttribute of the Model here in controller. public String processForm(@ModelAttribute("student") Student theStudent) { System.out.println("Full name: " + theStudent.getFirstName()+" " + theStudent.getLastName()); return "student-confirmation"; } }To access our form backing object, we need to inject it via the @ModelAttribute annotation.An &lt;em>@ModelAttribute &lt;/em>on a method argument indicates the argument will be retrieved from the model. If not present in the model, the argument will be instantiated first and then added to the model.[What is Model as a parameter in the Controller method? (Spring forum at Coderanch)](https://coderanch.com/t/695520/frameworks/Model-parameter-Controller-method)[java - How does Spring MVC controller method parameter work? - Stack Overflow](https://stackoverflow.com/questions/8372957/how-does-spring-mvc-controller-method-parameter-work) |**Step 5:** JSP html confirmation page📂 view/student-confirmation.jsp|                                                                                                                                                                                                                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%@ page language="java" contentType="text/html; charset=ISO-8859-1"     pageEncoding="ISO-8859-1"%> &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Confirmation of student form submission&lt;/title> &lt;/head> &lt;body> &lt;h1>Form Submitted&lt;/h1> The Student is Confirmed: ${student.firstName} ${student.lastName} &lt;/body> &lt;/html> |**AFAQ**- How is Spring jsp able to access private members of an object, here the _firstName_ and _lastName_ variable?

  - [****java - How Can Spring/Hibernate Access Private Members? - Stack Overflow****](https://stackoverflow.com/questions/4127365/how-can-spring-hibernate-access-private-members)
  - [****how java jaxb works? - Stack Overflow****](https://stackoverflow.com/questions/3391256/how-java-jaxb-works)**


#### Drop-Down Lists - Overview


##### ** [12-form-tags-dropdown-overview.pdf](https://drive.google.com/open?id=123lLXDQ481w62Z5hOZpGB6tFGuDFiCTh&usp=drive_copy) [ovwVid](https://www.youtube.com/watch?v=2ffhPUfhCL8&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=94&ab_channel=freeCodeCampBengali) [codeVid1 codeVid2](https://youtu.be/NWTwVTPjdX0?list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H)Usual plain HTML dropdown (select tag and option tag)  example:|                                                                                                                                                                                                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| &lt;form action="#">   &lt;label for="country">Choose a country:&lt;/label>   &lt;select name="country" id="country">     &lt;option value="India">India&lt;/option>     &lt;option value="Bangladesh" label="Bangladesh">&lt;/option>     &lt;option value="Germany">Germany&lt;/option>   &lt;/select>   &lt;br>&lt;br>   &lt;input type="submit" value="Submit"> &lt;/form> |Browser output:![](https://lh6.googleusercontent.com/N29oGB-oIiRkHrnItxi2BHL4CdGZvyT2njubxIWh50kHq18ZEO1lRe1FAV2cJYn_depM_uzJ2_PczLZDm5TwagTRSszMWIq678DtxERJ678RJXMZ72q3RHZAYQEUxircBZWCTSaA5dKR87oQU-KfYE0)**MVC form Drop-Down example**:|                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;form action="#" modelAttribute="student">   &lt;label for="country">Choose a country:&lt;/label>   &lt;form:select name="country" path="country">     &lt;form:option value="India" label="India">&lt;/option>     &lt;form:option value="Bangladesh" label="Bangladesh">&lt;/option>     &lt;form:option value="Germany" label="Germany">&lt;/option>   &lt;/form:select>   &lt;br>&lt;br>   &lt;input type="submit" value="Submit"> &lt;/form> |Development process: Step by step6. Update the Student jsp html form => add dropdown html support
7. Update the Student class => Adding getter/setter for new property (country)
8. Update the student form Confirmation page Note: We had no need to update the controller class, as any specific data addition or change in the form will be taken care of by spring, as they are binded. Also Referring to the note of [Text-Fields](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.9s7rc9n4nnak) Step 2. **Step 6**: Update the Student jsp html form => add dropdown html support📂 student-form.jsp|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%-- To enable the spring form support add the following line --%>  &lt;%@ taglib prefix="form" uri="http&#x3A;//www.springframework.org/tags/form"%>   &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Student Information Form&lt;/title> &lt;/head> &lt;body> &lt;h1>Fill up the student information form&lt;/h1> &lt;form:form action="processForm" modelAttribute="student"> Firstname: &lt;form:input path="firstName"/> &lt;br>&lt;br> Lastname: &lt;form:input path="lastName"/> &lt;br>&lt;br>  &lt;!--\[Start] Step 6: Adding drop-down support--> Country: &lt;form:select path="country"> &lt;form:option value="Bangladesh" label="Bangladesh">&lt;/form:option> &lt;form:option value="India" label="India">&lt;/form:option> &lt;form:option value="Germany" label="Germany">&lt;/form:option> &lt;/form:select> &lt;br>&lt;br> &lt;!--\[End] Step 6--> &lt;input type="submit" value="submit"/>  &lt;/form:form> &lt;/body> &lt;/html> |**Step 7**: Update the Student class => Adding getter/setter for new property (country)📂 Student.class|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| package com.diptopaul.springdemo.mvc; import java.util.LinkedHashMap; public class Student { private String firstName; private String lastName;  //\[Start] Step 7.1 (Drop-down): Adding country attribute and getter setter code private String country; //\[HalfEnd] Step 7.1  public Student() {  }  public String getFirstName() { return firstName; } public void setFirstName(String firstName) { this.firstName = firstName; } public String getLastName() { return lastName; } public void setLastName(String lastName) { this.lastName = lastName; } //\[Again-Start] Step 7.2 (Drop-down): Adding country attribute and getter setter code public String getCountry() { return country; } public void setCountry(String country) { this.country = country; } //\[End] Step 7.2 //\[Start] Step Extra Part 3 (Drop-down): Adding countryOptions in the Drop down avoiding hard coding the option public LinkedHashMap&lt;String, String> getCountryOptions() { return countryOptions; } //\[End] Step Extra P3 } |**Step 8:** Update the student form Confirmation page📂 student-confirmation.jsp|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%@ page language="java" contentType="text/html; charset=ISO-8859-1"     pageEncoding="ISO-8859-1"%> &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Confirmation of student form submission&lt;/title> &lt;/head> &lt;body> &lt;h1>Form Submitted&lt;/h1> The Student is Confirmed &lt;br> &lt;br> Name: ${student.firstName} ${student.lastName} &lt;br> &lt;br> &lt;!--\[Start] Step 8: Adding country taken from drop-down--> Country: ${student.country} &lt;!--\[End] Step 8: Adding country taken from drop-down--> &lt;/body> &lt;/html> |
|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |**Extra Step**: Reading the Country Option from the Java class, avoiding hard coded html📂 Student.class|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| package com.diptopaul.springdemo.mvc; import java.util.LinkedHashMap; public class Student { private String firstName; private String lastName;  //\[Start] Step 7.1 (Drop-down): Adding country attribute and getter setter code private String country; //\[HalfEnd] Step 7.1  //\[Start] Step Extra Part 1 (Drop-down): Adding countryOptions in the Drop down avoiding hard coding the option private LinkedHashMap&lt;String, String> countryOptions; //\[End] Step Extra Part 1  public Student() {  //\[Start] Step Extra Part 2 (Drop-down): Adding countryOptions in the Drop down avoiding hard coding the option countryOptions = new LinkedHashMap&lt;>(); countryOptions.put("BD", "Bangladesh"); countryOptions.put("IN", "India"); countryOptions.put("DE", "Germany"); countryOptions.put("USA", "United States of America"); //\[End] Step Extra Part 2 }  public String getFirstName() { return firstName; } public void setFirstName(String firstName) { this.firstName = firstName; } public String getLastName() { return lastName; } public void setLastName(String lastName) { this.lastName = lastName; } //\[Again-Start] Step 7.2 (Drop-down): Adding country attribute and getter setter code public String getCountry() { return country; } public void setCountry(String country) { this.country = country; } //\[End] Step 7.2 //\[Start] Step Extra Part 3 (Drop-down): Adding countryOptions in the Drop down avoiding hard coding the option public LinkedHashMap&lt;String, String> getCountryOptions() { return countryOptions; } //\[End] Step Extra P3 } |📂 student-form.jsp|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%-- To enable the Spring MVC form support add the following line --%>  &lt;%@ taglib prefix="form" uri="http&#x3A;//www.springframework.org/tags/form"%>   &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Student Information Form&lt;/title> &lt;/head> &lt;body> &lt;h1>Fill up the student information form&lt;/h1> &lt;form:form action="processForm" modelAttribute="student"> Firstname: &lt;form:input path="firstName"/> &lt;br>&lt;br> Lastname: &lt;form:input path="lastName"/> &lt;br>&lt;br>  &lt;!--\[Start] Step 6: Adding drop-down support--> Country: &lt;form:select path="country"> &lt;!-- &lt;form:option value="Bangladesh" label="Bangladesh">&lt;/form:option> &lt;form:option value="India" label="India">&lt;/form:option> &lt;form:option value="Germany" label="Germany">&lt;/form:option> --> &lt;!--\[Start] Step Extra (Drop-down) : Adding non hard coded drop-down support--> &lt;form:options items="${student.countryOptions}"/> &lt;!--\[End] Extra Step-->  &lt;/form:select> &lt;br>&lt;br> &lt;!--\[End] Step 6--> &lt;input type="submit" value="submit"/>  &lt;/form:form> &lt;/body> &lt;/html> |**FAQ**: - Use properties file to load country options

  - [133-faq-use-properties-file-to-load-country-options.pdf](https://drive.google.com/file/d/1YQtMC59f85ASNBk_b-uoiSklPDAybQnB/view?usp=share_link)**


#### Radio Buttons - Overview 


##### **[13-form-tags-radio-overview.pdf](https://drive.google.com/open?id=1csFcZzcX-b5Ye-JhowAb2WRRV5SHXcyY&usp=drive_copy) [ovwVid](https://www.youtube.com/watch?v=X3LervKywPw&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=97&ab_channel=freeCodeCampBengali) [codeVid1 ](https://www.youtube.com/watch?v=SOG9-YY5YUU&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=98&ab_channel=freeCodeCampBengali)Usual plain HTML radio button(input tag with type radio)  example:|                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;form action="#">   &lt;p>Please select your favorite Web language:&lt;/p>   &lt;input type="radio" id="html" name="fav_language" value="HTML">   &lt;label for="html">HTML&lt;/label>&lt;br>   &lt;input type="radio" id="css" name="fav_language" value="CSS">   CSS&lt;br>   &lt;input type="radio" id="javascript" name="fav_language" value="JavaScript">JavaScript   &lt;br>&lt;br>   &lt;input type="submit" value="Submit"> &lt;/form> |
|                                                                                                                                                                                                                                                                                                                                                                                                                                                   |Browser output:![](https://lh5.googleusercontent.com/_A5EUmI3q0ayMDxD_3Q02zhqhsr64WNNUVavQyAJLeFodT-7A36hsePraArCFnY9TRgQKbMNkNz0CI63DHC8t984u5BfiBah3uGihvZmvVf2MGRQ12KRjdSIuHvFB0FpH3hybSP3sABZWgxQbV44k3k)**MVC form Radio button(radio tag)  example**:|                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;form:form action="processForm" modelAttribute="student"> Favorite Language: &lt;br> Java &lt;form:radiobutton path="favoriteLanguage" value="Java"/>  C++ &lt;form:radiobutton path="favoriteLanguage" value="C++"/> &lt;br> &lt;br> &lt;input type="submit" value="submit"/> &lt;/form:form> |Development process: Step by step9. Update the Student jsp html form => add radio button html support
10. Update the Student class => Adding getter/setter for new property (radio programming language)
11. Update the student form Confirmation page for Radio**Step 9:**|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **&lt;body> ****&lt;h1>Fill up the student information form&lt;/h1> ****&lt;form:form action="processForm" modelAttribute="student"> ****Firstname: &lt;form:input path="firstName"/> ****&lt;br>&lt;br> ****Lastname: &lt;form:input path="lastName"/> ****&lt;br>&lt;br> ****&lt;!--\[Start] Step 9: Adding radio button support for favorite language--> ****Favorite Language: ****&lt;br> ****Java &lt;form:radiobutton path="favoriteLanguage" value="Java"/>  ****C++ &lt;form:radiobutton path="favoriteLanguage" value="C++"/> ****PHP &lt;form:radiobutton path="favoriteLanguage" value="PHP"/>  ****Python &lt;form:radiobutton path="favoriteLanguage" value="Python"/> ****&lt;br> &lt;br> ****&lt;!--\[End] Step 9--> **** ****&lt;input type="submit" value="submit"/> ****&lt;/form:form> &lt;/body>** |**Step 10: Refer to the full code****Step 11: Refer to the full code****FAQ**: - How to populate radio buttons with items from Java class? 

  - [136-faq-how-to-populate-radiobuttons-with-items-from-java-class.pdf](https://drive.google.com/file/d/1qsmvoSkcLz5Z52lePErbKrIwZRJ-1PVh/view?usp=share_link)**


#### Checkboxes - Overview: 


##### **Implementation is similar to the Radio button, except that we need an array attribute in the Student bean definition and need special tag to loop through the array when we display it.[14-form-tags-checkbox-overview.pdf](https://drive.google.com/open?id=1Tkwqq5K942hjoWqHLjvKoF9Ubyc5zIry&usp=drive_copy) \| [ovwVid](https://www.youtube.com/watch?v=mM5BlFeAD7E&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=99&ab_channel=freeCodeCampBengali) \| [codeVid1 ](https://www.youtube.com/watch?v=2wOWZegwcBU&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=100&ab_channel=freeCodeCampBengali)\| [codeVid2](https://www.youtube.com/watch?v=bWshma0fEBo&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=101&ab_channel=freeCodeCampBengali)**Usual plain HTML checkbox**(**_input tag with type checkbox_**)  example:|                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;form action="/action_page.php">   &lt;input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">   &lt;label for="vehicle1"> I have a bike&lt;/label>&lt;br>   &lt;input type="checkbox" id="vehicle2" name="vehicle2" value="Car">   I have a car&lt;br>   &lt;input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">   I have a boat&lt;br>&lt;br>   &lt;input type="submit" value="Submit"> &lt;/form> |**Browser output**:![](https://lh4.googleusercontent.com/sn2Ycs9W2c04ZqtPSc8mVkSGmUUR5SEd_AQMRHBEmL3sS-T7tRj1GGPm90ns8MCT9c8ZBz3U44SNcDBnnAlb9DUTpcgHU0zm5TgphtzeRaeKnBC_IfH9obRah6tFHWM2hnzvRYWfJDaxW83pegWWZ0k)**MVC form Checkboxes example**:|                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **&lt;form:form action="processForm" modelAttribute="student">********Favorite OS:********&lt;br>********Linux &lt;form:checkbox path="operatingSystems" value="Linux" />****Mac OS &lt;form:checkbox path="operatingSystems" value="Mac OS" />****MS Windows &lt;form:checkbox path="operatingSystems" value="MS Windows"/>********&lt;br> &lt;br>********&lt;input type="submit" value="submit"/>****&lt;/form:form>** |Development process: Step by step12. Update the Student jsp html form => add checkbox html support
13. Update the Student class => Adding getter/setter for new property (variable operatingSystems for checkBox)
14. Update the student form Confirmation page for checkBox**Step 12:** same as MVC form Checkboxes example **given above.****Step 13:**|                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| //(Checkbox): Adding favoriteOS attribute and getter setter code private String\[] operatingSystems; public Student() {  //codes here } public String\[] getOperatingSystems() { return operatingSystems; } //on submit spring will call this method since it is binded with operatingSystem attribute public void setOperatingSystems(String\[] operatingSystems) { this.operatingSystems = operatingSystems; } |**Step 14:** Using JSTL tag|                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| &lt;!-- to enable support for jstl tags --> &lt;%@ taglib uri = "http&#x3A;//java.sun.com/jsp/jstl/core" prefix = "c" %> &lt;!DOCTYPE html> &lt;html> &lt;head>  ... &lt;/head> &lt;body> Operating System: &lt;ul> &lt;c:forEach var="item" items="${student.operatingSystems}"> &lt;li>${item}&lt;/li> &lt;/c:forEach> &lt;/ul> &lt;/body> &lt;html> |**


## FAQ


##### ****AFAQ**1. [What is @ModelAttribute in Spring MVC? - Stack Overflow](https://stackoverflow.com/questions/3423262/what-is-modelattribute-in-spring-mvc) - Read most of the answer
2. [How Spring processes @ModelAttribute?](https://www.codelooru.com/2010/11/how-does-modelattribute-work.html#:~:text=The%20way%20Spring,to%20the%20Model.)
3. [Difference between modelAttribute and commandName attributes in form tag in spring? - Stack Overflow](https://stackoverflow.com/questions/21495616/difference-between-modelattribute-and-commandname-attributes-in-form-tag-in-spri)**


## Part 4. Spring MVC Form Validation - Applying Built-In Validation Rules


### Form validation overview


##### **[15-form-validation-overview.pdf](https://drive.google.com/open?id=1mgk6Frk2Y-pytphBCVbylQJmFTY9JHzn&usp=drive_copy) [ovwVid](https://www.youtube.com/watch?v=rzkNYQ51R18&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=102&ab_channel=freeCodeCampBengali)Java’s Standard Bean Validation API- Java’s Standard Bean Validation API - <http://www.beanvalidation.org>
- Defines a metadata model and API for entity validation
- Not tied to either the web tier or the persistence tier
- Available for server-side apps and also client-side JavaFX/Swing appsSpring and Validation- Spring version 4 and higher supports Bean Validation API
- Preferred method for validation when building Spring apps
- Simply add Validation JARs to our projectValidation Annotations|                 |                                                                                     |
| --------------- | ----------------------------------------------------------------------------------- |
| Annotation      | Description                                                                         |
| @NotNull        | Checks that the annotated value is not null  \[implements the **required feature**] |
| @Min            | Must be a number >= value \[**validates numbers**]                                  |
| @Max            | Must be a number &lt;= value \[**validate numbers**]                                |
| @Size           | Size must match the given size \[**validates length**]                              |
| @Pattern        | Must match a regular expression pattern                                             |
| @Future / @Past | Date must be in future or past of given date                                        |
| Others          | \[**custom validation**]                                                            |Our Road Map1. set up our development environment
2. required field
3. validate number range: min, max
4. validate using regular expression (regexp)
5. custom validation**


#### Form Validation Dev Environment Overview


##### **[16-form-validation-dev-environment-overview.pdf](https://drive.google.com/open?id=1Oa1-I6j8NUMMpapGbbGWTVSutWjKWqNc&usp=drive_copy) [ovwVid](https://www.youtube.com/watch?v=WnLpiX75OI8&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=103&ab_channel=freeCodeCampBengali) [3 Installing Validation Files - YouTube](https://www.youtube.com/watch?v=SiCYdIj9IbM&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=104&ab_channel=freeCodeCampBengali)Hibernate Validator - <http://www.hibernate.org/validator>- The Hibernate team built this to allow developers to express and validate application constraints.
- They have other projects such as the ORM project (tied with the database)Hibernate Validator Version?- Hibernate Validator 7 is based on Jakarta EE 9
- Jakarta EE 9 is the rebranded version of Java EE(latest version Java EE 8, Aug 2017). javax.\* packages are renamed to jakarta.\* . Jakarta EE does not replace Java EE. Support for both is still available.
- Spring 5 is still based on some components of Java EE (javax.\*). Spring may use Jakarta EE components in the future, but no news yet.
- As a result, Spring 5 is not compatible with Hibernate Validator 7Two releases of Hibernate Validator- Hibernate Validator 7 is for Jakarta EE 9 projects
- **Hibernate Validator 6.2** is compatible with **Spring 5**. Hibernate Validator 6.2 has the SAME features as Hibernate Validator 7.In Summary- If you are using **Spring 5** .... then use **Hibernate Validator 6.x**
- If you are using **Jakarta EE 9** ... then use **Hibernate Validator 7.x**
- More details on Hibernate Validator release - <https://in.relation.to/hibernate-validator>Development Process ([3 Installing Validation Files - YouTube](https://www.youtube.com/watch?v=SiCYdIj9IbM&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=104&ab_channel=freeCodeCampBengali))1. Download Validation JAR files from [Hibernate Validator website](https://hibernate.org/validator/) > Releases > Select release version > Then download.

2. Add JAR files to project 

   1. Copy the **3 jar files** from the **dist** folder of downloaded project **hibernate-validator-6.2.5.Final or suitable project.** Then paste the jar files to the **lib** (webapp > WEB-INF > lib) ****folder of your project.
   2. Now copy the **jar files** from the **dist > lib > required** folder and do the same thing.**


### Applying Built-In Validation Rules


### Form Validation Required Overview (Built-In)


##### **[17-form-validation-required-overview.pdf](https://drive.google.com/open?id=11TYJsNU21OrzqNr_5oQiKbA-uT_46zNh&usp=drive_copy) [4 Checking for Required Fields Overview - YouTube](https://www.youtube.com/watch?v=pEuJLt7yEZo&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=105&ab_channel=freeCodeCampBengali)\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**Special Note about BindingResult Parameter Order:**When performing Spring MVC validation, the location of the BindingResult parameter is very important. In the method signature, **the BindingResult parameter must appear immediately after the model attribute**. If you place it in any other location, Spring MVC validation will not work as desired. In fact, your validation rules will be ignored.       @RequestMapping("/processForm")        public String processForm(                @Valid @ModelAttribute("customer") Customer theCustomer,                BindingResult theBindingResult) {            ...                    }Here is the relevant section from the Spring Reference Manual\---**_Defining @RequestMapping methods_**_@RequestMapping handler methods have a flexible signature and can choose from a range of supported controller method arguments and return values.__...__The Errors or BindingResult parameters have to follow the model object that is being__bound immediately ...__Source:_ [_https://docs.spring.io/spring/docs/current/spring-framework-reference/web.html#mvc-ann-methods_](https://docs.spring.io/spring/docs/current/spring-framework-reference/web.html#mvc-ann-methods)\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**


#### Development Process - [17-form-validation-required-overview.pdf](https://drive.google.com/open?id=11TYJsNU21OrzqNr_5oQiKbA-uT_46zNh&usp=drive_copy)


##### **1. Add validation rule to Customer class - [6 Add Validation Rule to Customer Class - YouTube](https://www.youtube.com/watch?v=RxI1wWFBSv4&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=103&ab_channel=freeCodeCampBengali)
2. Display error messages on HTML form - [7 Display Validation Error Messages on HTML Form - YouTube](https://www.youtube.com/watch?v=yyk1VxvS5P0&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=103&ab_channel=freeCodeCampBengali)
3. Perform validation in the Controller class [Part 1](https://www.youtube.com/watch?v=ZOsEgjYJacg&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=104&ab_channel=freeCodeCampBengali) [Part 2](https://www.youtube.com/watch?v=M_rC1t_7AfU&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=109&ab_channel=freeCodeCampBengali)
4. Update confirmation page - [10 Update Confirmation Page - YouTube](https://www.youtube.com/watch?v=X7Ak0tAfRik&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=110&ab_channel=freeCodeCampBengali)Extra Steps:5. Test the Validation Rule for Required Fields - [11 Test the Validation Rule for Required Fields - YouTube](https://www.youtube.com/watch?v=dVHQtg29YLY&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=111&ab_channel=freeCodeCampBengali)
6. Add Pre-processing Code with @InitBinder [18-form-validation-init-binder-trim-overview.pdf](https://drive.google.com/open?id=1pqaSqkKUtGiOP9TMlaB48KrlpWxBnkK9&usp=drive_copy) [@InitBinderCodeVid - YouTube](https://www.youtube.com/watch?v=wgqHHRwSPQ4&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=113&ab_channel=freeCodeCampBengali)**Step 1:**|                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| public class Customer { private String firstName; @NotNull(message="is required") @Size(min=1, message="is required") private String lastName; // getter/setter methods } |**Step 2:**|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%@ taglib uri="http&#x3A;//www.springframework.org/tags/form"     prefix="form"%> &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Insert title here&lt;/title> &lt;/head> &lt;body> &lt;form:form modelAttribute="customer" action="processForm"> First name: &lt;form:input path="firstName">&lt;/form:input> &lt;br> &lt;br> Last Name: &lt;form:input path="lastName">&lt;/form:input> &lt;form:errors path="\*" cssClass="error">&lt;/form:errors> &lt;br> &lt;br> &lt;input type="submit" value="submit">&lt;/input> &lt;/form:form> &lt;/body> &lt;/html> |When we submit the form with an empty **lastName** , it will add an span and return the form as below,|                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;body> &lt;form id="customer" action="processForm" method="post"> First name: &lt;input id="firstName" name="firstName" type="text" value=""> &lt;br> &lt;br> Last Name: &lt;input id="lastName" name="lastName" type="text" value="">            &lt;%-- Associated errors to lastName field displayed --%> &lt;span id="customer.errors" class="error">is required&lt;/span> &lt;br> &lt;br> &lt;input type="submit" value="submit"> &lt;/form> &lt;/body> |**AFAQ:** How does Spring enable the error tag to be visible when an error is found? - Answer given at the bottom of Step 3.**Step 3:**|                                                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **@Controller @RequestMapping("/customer") public class CustomerController { ****@RequestMapping("/processForm") ****public String processForm(@ModelAttribute("customer") Customer customer) { ****return "customer-confirmation"; ****} }** |The control method processForm will be called after submit, @Valid enables the validation check on the customer object which is now binded with the Model object customer.********|                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------- |
| **public String processForm(@Valid @ModelAttribute("customer") Customer customer) { ****return "customer-confirmation"; }** |After the validation check, spring needs to save the result somewhere. We will have a BindingResult type parameter theBindingResult, Spring will inject? the validation result to this object.|                                                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **@RequestMapping("/processForm") public String processForm(@Valid @ModelAttribute("customer") Customer customer, BindingResult theBindingResult)) { ****return "customer-confirmation"; }** |As a result we can use the theBindingResult inside the method to check whether there is any error in the result and perform operation accordingly.|                                                                                                                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **public class CustomerController { @RequestMapping("/processForm") ****public String processForm(@Valid @ModelAttribute("customer") Customer customer, BindingResult theBindingResult) { ****if(theBindingResult.hasErrors()) { ****return "customer-form"; ****} ****return "customer-confirmation"; ****} }** |AFAQ: How does Spring enable the error tag to be visible when an error is found? - Binding and validation errors are registered in the model. The tag retrieves these errors from the model for display purposes. If the tag is nested inside a form:form tag the effective error key or path is the combination of the modelAttribute attribute in the form:form tag and the path you specify. In your case the modelAttribute is not explicit. Referring to the jsp code of step 2,

  - if you enter &lt;form:errors path="lastName">, only errors bound to customer.lastName path are displayed => 1 message
  - if you enter &lt;form:errors path="\*">, errors bound to the customer and its child paths are displayed => more messages. [Source](https://docs.spring.io/spring-framework/docs/3.0.x/spring-framework-reference/html/view.html#view-jsp-formtaglib-errorstag:~:text=What%20if%20we,to%20the%20fields%3A)
  - To check put the following in the Customer class as a new member attribute of the class with validation rules,|                                                                                                          |
| -------------------------------------------------------------------------------------------------------- |
| @NotNull(message="is required") @Size(min=2, message = "is required") private String dummyAttForErrTest; |Also use add a new error tag to display all the errors, |                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;form:form modelAttribute="customer" action="processForm"> First name: &lt;form:input path="firstName">&lt;/form:input> &lt;br> &lt;br> Last Name: &lt;form:input path="lastName">&lt;/form:input> &lt;form:errors path="lastName" cssClass="error">&lt;/form:errors> &lt;br> &lt;br> &lt;% //to display all the errors %> &lt;form:errors path="\*" cssClass="error">&lt;/form:errors> &lt;br> &lt;br> &lt;input type="submit" value="submit">&lt;/input> &lt;/form:form> |**Step 4:**&lt;body>Customer is confirmed.&lt;br>Name: ${customer.firstName} ${customer.lastName}&lt;/body>**


##### Advance Validation


##### ****Update:** you can use @NotBlank for handlin whitespaced input **Extra Step 5:** [11 Test the Validation Rule for Required Fields - YouTube](https://www.youtube.com/watch?v=dVHQtg29YLY&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=111&ab_channel=freeCodeCampBengali)If the user inputs white spaces in the lastName’s input field it wont show any error and will take the input. Weird, Right!!! Solution? **We need Advance validation rules.******![](https://lh3.googleusercontent.com/CjGN2hDe1NpGYMNpAKMQ7bqsF6ckS0t7HeKXOdvSEusQAyIMqt9DZ87UhLryPO2sGPj9-GO5Eq8C-LdXxIGA8k4jKzDFjI-_aF6Xxyw4BrwFG5F2kUDZwCBd6_bMPW4PDh-nd-7ZqZ913hfIrx78OCU)******Extra Step 6:** Add Pre-processing Code with @InitBinder - Overview - [18-form-validation-init-binder-trim-overview.pdf](https://drive.google.com/open?id=1pqaSqkKUtGiOP9TMlaB48KrlpWxBnkK9&usp=drive_copy)  [InitBinderOvvwVid](https://www.youtube.com/watch?v=oQfbCLI5tLc&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=112&ab_channel=freeCodeCampBengali) [@InitBinderCodeVid](https://www.youtube.com/watch?v=wgqHHRwSPQ4&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=113&ab_channel=freeCodeCampBengali)- @InitBinder annotation works as a pre-processor
- It will pre-process each web request to our controller
- **Method annotated with @InitBinder is executed**
- We will use this to trim Strings
- Remove leading and trailing white space
- If String only has white spaces ... trim it to null
- Will resolve our validation problem ... whew :-)**Register Custom Editor in Controller:**CustomerController.java|                                                                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @InitBinder//1 public void initBinder(WebDataBinder dataBinder) {StringTrimmerEditor stringTrimmerEditor = new StringTrimmerEditor(true);//2 dataBinder.registerCustomEditor(String.class, stringTrimmerEditor);//3} |1. Methods annotated with @InitBinder will be called by the Spring framework to initialize the WebDataBinder. Spring will Inject the WebDataBinder into the method. 
2. Create a StringTrimmerEditor instance. The boolean flag indicates if you want to have an empty string returned as null (use true), or if an empty string should remain an empty string (use false).
3. Register the StringTimmerEditor to the binder for all fields of type String.Now all excess whitespace will be trimmed automatically when the values are taken from the &lt;input> fields and put in the form data object.![](https://lh3.googleusercontent.com/Am5sGP7WVhqrievWBFc0WFwoWE7BOCqdOAfSejE-6CNRzUaKQZVQmT5NqJOp0pl2NaR5vcP6hUiVs0lX7QamLMVWG9c81vXCMAiEdICaC25et-2m6pSsCceYEWKSDJ1eIbzKtaqQ0jd6tvXw5CVz6QU)Explanation: [Using StringTrimmerEditor with Thymeleaf - Wim Deblauwe](https://www.wimdeblauwe.com/blog/2021/01/25/using-stringtrimmereditor-with-thymeleaf/)**


### Form Validation - Validating Number Ranges


#### Validating Number Ranges


##### **[19-form-validation-range-overview.pdf](https://drive.google.com/open?id=1nzBWt8m_c7HU5x_craRv-McC8PcFQsE-&usp=drive_copy) [1 Validating a Number Range Overview - YouTube](https://www.youtube.com/watch?v=hi21bfU08gY&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=114&ab_channel=freeCodeCampBengali)Validating a Number Range - [1 Validating a Number Range Overview - YouTube](https://www.youtube.com/watch?v=hi21bfU08gY&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=115&ab_channel=freeCodeCampBengali) \| [VidCode](https://www.youtube.com/watch?v=K3qDxivArfI&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=115&ab_channel=freeCodeCampBengali)Development Process1. Add validation rule to Customer class
2. Display error messages on HTML form
3. Perform validation in the Controller class
4. Update confirmation page**Step 1**: Add validation rule to Customer class|                                                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| public class Customer { // adding range of 0 - 10 @Min(value=0, message="must be greater than or equal to zero") @Max(value=10, message="must be less than or equal to 10") private int freePasses; // getter/setter methods } |**Step 2**: Display error messages on HTML formview/customer-form.jsp&lt;form:form modelAttribute="customer" action="processForm">Free passes: &lt;form:input path="freePasses">&lt;/form:input>&lt;form:errors path="freePasses" cssClass="error">&lt;/form:errors>&lt;br> &lt;br>&lt;input type="submit" value="submit">&lt;/input>&lt;/form:form>**Step 3**: Perform validation in the Controller class, nothing to update, it will be same as we did in Required validation**Step 4:** Update confirmation page, same like the others**


##### Integer Field and Handling String input for Integer Fields


##### **How to make Integer Field Required: freePasses [5 How to make Integer Field Required freePasses - YouTube](https://www.youtube.com/watch?v=i8pSfUaTclA&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=120&ab_channel=freeCodeCampBengali) |                                                                                                                                                                                                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| public class Customer {//required validation added @NotNull(message="is required, null") // adding range of 0 - 10 @Min(value=0, message="must be greater than or equal to zero") @Max(value=10, message="must be less than or equal to 10") private int freePasses; // getter/setter methods } |But **there is an issue**, if you try to put an empty or non int string you will see errors. For an empty string with spaces, the preprocessor initBinder will convert it to null but since int can not have null, it will also produce an error. Currently, we will deal with non int string errors. We need to add regex to handle it.![](https://lh6.googleusercontent.com/SfGQaM2C3CDTysdPtCWp6dvLpbeLd6FjaDkmC07MkmlNC59YrLpyrHGD8c9GCcJYaiy4VKxohGsMOfXTUtUGWJulRqwkRIB-QncPRRdYBscpomUIIF4ZlbcUUZWg1X_URAJfbkz5hfMQ6OTQUa-oCHQ)We need a solution. To make our We can refactor the ****int freePasses to **Integer freePasses** That will handle String input for Integer Fields. Note: **Integer** can hold **null.**How to Handle String input for Integer Fields - Deep Dive [8 How to Handle String input for Integer Fields Deep Dive - YouTube](https://www.youtube.com/watch?v=qfabAVcgdQo&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=121&ab_channel=freeCodeCampBengali)If we try to provide non int input for Integer freePasses input it will cause an error, but this error is long and complex for the user. We need a custom error message.![](https://lh4.googleusercontent.com/bzgJ-e30l9YiQdLWG5O_O8sNImBC4yLTEcUa_7yzlt5r_y-mIB0NWp7v88mgpOCNLDP0ihMZPTjaihzhCvXClRRYfDclQrZFT-mZU7ASsazanNIWyNa61kChPnBpT0zfZ6UTa0Zlt4Mf_2eSHJ1pua0) Now if we print the Binding results in the console we see this,![](https://lh3.googleusercontent.com/Xw9WcOSYw5g_DKP3uPzF4R_ouH_V4_doR5lwCwwa5iS1wusnVUTr3gSpHOinmWFuEmbUCPuRzdf0IaUKGqcr7ZRWX2VfJ-mUHa3Jln_iMbbYl3-pYu10l8vjOO6B_XiytCNL10_0BhCxmoTJ2VmQPLM)The console output message is here,|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| org.springframework.validation.BeanPropertyBindingResult: 1 errorsField error in object 'customer' on field 'freePasses': rejected value \[adadadadadad]; codes \[typeMismatch.customer.freePasses,typeMismatch.freePasses,typeMismatch.java.lang.Integer,typeMismatch]; arguments \[org.springframework.context.support.DefaultMessageSourceResolvable: codes \[customer.freePasses,freePasses]; arguments \[]; default message \[freePasses]]; default message \[Failed to convert property value of type 'java.lang.String' to required type 'java.lang.Integer' for property 'freePasses'; nested exception is java.lang.NumberFormatException: For input string: "adadadadadad"] |So to set our own custom error message for the field freePass, we have to define our custom message in typeMismatch.customer.freePasses = “our custom message”.One thing to note, If you assign typeMismatch.freePasses = “our custom message” ; your custom message will be applicable for any typeMismatch on any field with the name freePasses from any Model Attribute.How to Handle String input for Integer Fields - Custom Message [6 How to Handle String input for Integer Fields Custom Message - YouTube](https://www.youtube.com/watch?v=shbgRsA787s&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=120&ab_channel=freeCodeCampBengali)Development Process:1. Create Custom Error Message

   1. src/resource/messages.properties 

2. Load Custom message resource in spring config file

   1. WebContent/WEB-INF/spring-mvc-demo-servlet.xmlStep 1:Formate: Error Type.SpringModelAttributeName.fieldName = ourCustomMessage typeMismatch.customer.freePasses =Invalid numberHow to Handle String input for Integer Fields - Configure Resource Bundle  [7 How to Handle String input for Integer Fields Configure Resource Bundle - YouTube](https://www.youtube.com/watch?v=ybPFP9rMi7M&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=120&ab_channel=freeCodeCampBengali)FAQ: How to make Integer field required and handle Strings: freePasses - [161-FA~1.PDF](https://drive.google.com/file/d/1_nrCbqIDoCiqsI2oAx_-DuPQPj6bvwAA/view?usp=share_link)**


#### Form Validation - Regular Expressions


##### **[20-form-validation-regex-overview.pdf](https://drive.google.com/open?id=1hPbBGvLyMkco6B5-eAhM8t3cEw7QxucF&usp=drive_copy) \| [3 Applying Regular Expressions Overview - YouTube](https://www.youtube.com/watch?v=I-QtF1JBs10&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=117&ab_channel=freeCodeCampBengali) [VidCode](https://www.youtube.com/watch?v=mH8jwDRLgzY&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=118&ab_channel=freeCodeCampBengali)Development Process:1. Add validation rule to Customer class
2. Display error messages on HTML form
3. Update confirmation pageStep 1:import javax.validation.constraints.Pattern;public class Customer {@Pattern(regexp="^\[a-zA-Z0-9]{5}", message="only 5 chars/digits")private String postalCode;// getter/setter methods}**


### Form Validation - Creating Custom Validation Rules (Advanced)


##### **Custom Form Validation - Overview[21-form-validation-custom-overview.pdf](https://drive.google.com/open?id=1Q-1DcWLMwyJnMluYUCr8c7tj7QwFrU4w&usp=drive_copy) [22-spring-mvc-crud-project-overview.pdf](https://drive.google.com/file/d/1XxTAQc2PouY4uN-jXHAXIkoqTcpajAkd/view?usp=share_link)[1 Custom Form Validation Overview Part 1 - YouTube](https://www.youtube.com/watch?v=c3jTW5bsJ0E&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=122&ab_channel=freeCodeCampBengali) [2 Custom Form Validation Overview Part 2 - YouTube](https://www.youtube.com/watch?v=ypUQeQuBbhE&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=123&ab_channel=freeCodeCampBengali)✤ So far, we’ve used predefined validation rules: **@Min, @Max**, ...✤ For custom validation ... we will create a Custom Java Annotation✤ **@CourseCode**@CourseCode(value="LUV", message="must start with LUV")private String courseCode;Development Process1. Create custom validation rule

   1. Create @CourseCode annotation
   2. Create CourseCodeConstraintValidator

2. Add validation rule to Customer class

3. Display error messages on HTML form

4. Update confirmation page**


#### Creating a Custom Java Annotation - [Part1 ](https://www.youtube.com/watch?v=NIMDcbYYWvk&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=124&ab_channel=freeCodeCampBengali) [Part2](https://www.youtube.com/watch?v=EYi7mZ1ZAYc&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=125&ab_channel=freeCodeCampBengali)


##### ****Step 1a**: Create @CourseCode annotation|                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Constraint(validatedBy = CourseCodeConstraintValidator.class) @Target( { ElementType.METHOD, ElementType.FIELD } ) @Retention(RetentionPolicy.RUNTIME) public @interface CourseCode { // define default course code public String value() default "LUV"; // define default error message public String message() default "must start with LUV"; //add codes for groups//add codes for//add anything else } |**


#### Developing the ConstraintValidator - [5 Developing the ConstraintValidator - YouTube](https://www.youtube.com/watch?v=i6831gCYo1E&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=126&ab_channel=freeCodeCampBengali)


##### ****Step 1b**:|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| import javax.validation.ConstraintValidator; import javax.validation.ConstraintValidatorContext; public class CourseCodeConstraintValidator implements ConstraintValidator&lt;CourseCode, String> { private String coursePrefix; @Override public void initialize(CourseCode theCourseCode) { coursePrefix = theCourseCode.value(); } @Override public boolean isValid(String theCode, ConstraintValidatorContext theConstraintValidatorContext) {  boolean result;  if (theCode != null) { result = theCode.startsWith(coursePrefix); } else { result = true; }  return result; } } |[spring - What is the use of groups and payload in custom Annotation In Java? - Stack Overflow](https://stackoverflow.com/questions/64493818/what-is-the-use-of-groups-and-payload-in-custom-annotation-in-java)Adding Validation Rule to the Entity and Form - [6 Adding Validation Rule to the Entity and Form - YouTube](https://www.youtube.com/watch?v=ccpwahf7ir4&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=127&ab_channel=freeCodeCampBengali)Testing the Custom Validation Rule - [7 Testing the Custom Validation Rule - YouTube](https://www.youtube.com/watch?v=YINpbi96p3E&list=PLon9KQO-XVcvPTumBz0HuTVQBeKHG0_1H&index=128&ab_channel=freeCodeCampBengali)**FAQ**: - Spring MVC Custom Validation - Possible to validate with multiple strings? - [169-faq-spring-mvc-custom-validation-possible-to-validate-with-multiple-strings.pdf](https://drive.google.com/file/d/1nr11wAfY1sXJG_JflAy6x7UD_L0KqEFX/view?usp=share_link)

  - The question is trying to say, is it possible to have more than one course prefix(eg: value={"TOPS", "LUV"}) to validate the input?@CourseCode(value={"TOPS", "LUV"}, message="must start with TOPS or LUV")private String courseCode;**


# Questions to deal with


##### **1. [Query: How does the web.xml and spring-mvc-demo-servlet.xml works?](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.4nti7w6ikete)
2. Query: How does Spring server call the Controller methods on their own?Hibernate**


# Chapter 1: Introduction to Hibernate


## Hibernate Overview -[01-hibernate-overview.pdf](https://drive.google.com/file/d/1q2BGVs1PO35L5RpfJz4LIT8BsAZDUDMA/view?usp=share_link)


##### ****What is Hibernate?**- A framework for persisting / saving Java objects in a database. [www.hibernate.org](http://www.hibernate.org)![](https://lh6.googleusercontent.com/5O9YF9JqSIglvv6Kccxvn962Dmx7hK7sAkqRCvhVsnbFpM9yU4yjb1_NaY5MEyAdKrPXRHsCrjz1VVIZKIyazlfI43ppg5zaXx6J7xlT5oRM2wROTQuZGgf6PpI26FhxbZeKqZHz9ZzyCYKv5xrmsvc)**Benefits of Hibernate**- Hibernate handles all of the low-level SQL
- Minimizes the amount of JDBC code you have to develop
- Hibernate provides the Object-to-Relational Mapping (ORM)**Object-To-Relational Mapping (ORM)**- The developer defines mapping between Java class and database table![](https://lh3.googleusercontent.com/_GbYgqZWjWwNlop9D2Xei_7DNrHpZHdbW2swo4WRSv6_NGaDEa6pZE9CbLasaGBIELG8-IsVaOBgnQ8aCdF4elCr_XPc-Uqirhv2nR0m-WPUvUJFvZ7bEa-M3fDvsboMOHRYPKsbgZWWE_lbC4kt4rw)**Saving a Java Object with Hibernate**|                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| // create Java object Student theStudent = new Student("John", "Doe", "john@luv2code.com"); // save it to database int theId = (Integer) session.save(theStudent); |**Retrieving a Java Object with Hibernate**|                                                                                                                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| // create Java object Student theStudent = new Student("John", "Doe", "john@luv2code.com"); // save it to database int theId = (Integer) session.save(theStudent); // now retrieve from database using the primary key Student myStudent = session.get(Student.class, theId); |**Querying for Java Objects**|                                                                                             |
| ------------------------------------------------------------------------------------------- |
| Query query = session.createQuery("from Student"); List&lt;Student> students= query.list(); |**


## Hibernate and JDBC - [02-hibernate-and-jdbc.pdf](https://drive.google.com/file/d/1bAAqFiO1nvLvcnun6yx4szDc5s-B-_fX/view?usp=share_link)


##### **- Hibernate uses JDBC for all database communications![](https://lh6.googleusercontent.com/AiieolinDPrSL7Znvvfwk2Oepn4tUNZTJxrbEEqoeyrkviGEqAAefZKUbcZqdbRxIyNRjfDYPjwSbe9_lfeMNaFNsziKbPySSm0yDha_ndu6wL-5WfmtJuU37PKiE0RLm7jqcU1NNs3dzLpgdYdJ5cc)**


# Chapter 2: Setting Up Hibernate Development Environment


##### **Before proceeding with developing application with hibernate, make sure you have installed,1. Java 8 or higher, Hibernate 5.2 Requires Java 8
2. You Must Have the Java Development Kit (JDK) Installed
3. (Extra) In order to run the examples in this course, you will need to have Java 8 installed.**


## Hibernate Development Environment Overview


##### **[03_hibernate_setup_dev_environment_overview.pdf](https://drive.google.com/file/d/1GEVxd8bF6rltS1JZQkGqjfaOFwgI55Qw/view?usp=share_link)\| [2 Vid](https://www.youtube.com/watch?v=aDvzxEhB-kI&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=3&ab_channel=freeCodeCampBengali)**Software Required**:1. Java Integrated Development Environment (IDE)
2. Database Server
3. Hibernate JAR files and JDBC Driver**Steps to follow to set up**:1. Install an Java Integrated Development Environment (IDE) - [04-hibernate-tutorial-install-eclipse-on-windows.pdf](https://drive.google.com/file/d/19KAxjGvFmg-EoBJSPkGtDt_mo8_frViW/view?usp=share_link)

2. A Database Server - MySQL

   1. Installing MySQL on MS Windows - [05-install_mysql.pdf](https://drive.google.com/file/d/1O9r9fpTL_MQmdpSK2BMjRt-euR6ZjKdP/view?usp=share_link)\| [InstallingMySQLVid](https://www.youtube.com/watch?v=0Lh1NZ_MLks&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=5&ab_channel=freeCodeCampBengali)

      1. [MySQL :: Developer Zone](https://dev.mysql.com/) > [MySQL Community Downloads](https://dev.mysql.com/downloads/) >[ MySQL Community Server](https://dev.mysql.com/downloads/mysql/) > [MySQL MSI Installer](https://dev.mysql.com/downloads/windows/installer/) > Download the web community version \[Windows (x86, 32-bit), MSI Installer (mysql-installer-**web**-community-8.0.32.0.msi)]

   2. Installing the MySQL Database on Mac -

      1. Official MySQL Installation instructions ****- ****<http://dev.mysql.com/doc/refman/5.7/en/osx-installation.html>

3. Setting/Adding Up a Database Table - [06_hibernate_setup_sample_data.pdf](https://drive.google.com/file/d/1v9eVwB9PTvhcx3cW7VoBkXI0YYacOigq/view?usp=share_link)\| [Video](https://www.youtube.com/watch?v=JghD0Fe2bc4&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=5&ab_channel=freeCodeCampBengali)

   1. Use mysql and run the two scripts inside [5.1 hibernate-sql-scripts-and-starter-files](https://drive.google.com/drive/folders/1W0hAMliNrR3AEl_aY3bTCis7NULBMoEJ?usp=share_link) to create a new table.

4. Setting up Hibernate and MySQL JDBC Driver in Eclipse - [07-setup-hibernate-in-eclipse.pdf](https://drive.google.com/file/d/1UNe96kdDe7L386pgnXPbCyFS6lddW0kG/view?usp=share_link)\| [Video](https://www.youtube.com/watch?v=nGlObYPEpZo&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=6&ab_channel=freeCodeCampBengali)

   1. Create Eclipse Project - Java Project (not Dynamic web project)

   2. Download Hibernate Files

      1. Go to [Your relational data. Objectively. - Hibernate ORM](https://hibernate.org/orm/) > [Releases](https://hibernate.org/orm/releases/) > Select the desired one (5.6 right now) > Download the Zip

   3. Download MySQL JDBC Driver

      1. Go to [MySQL :: Developer Zone](https://dev.mysql.com/) > [MySQL Downloads](https://dev.mysql.com/downloads/) » [Connector/J](https://dev.mysql.com/downloads/connector/j/) > Select Platform Independence as OS > Download the Zip

   4. Add Hibernate JAR files and MySQL JDBC Driver JAR files to Eclipse Project ... Build Path. [6 Setting up Hibernate in Eclipse - YouTube](https://www.youtube.com/watch?v=nGlObYPEpZo&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=6&ab_channel=freeCodeCampBengali)

      1. Create a “**lib”** folder in the Eclipse project

      2. From Hibernate project copy all files from dist>lib > required paste them to eclipse projects “**lib”** folder

      3. From MySQL copy all files from docs paste them to eclipse projects “**lib”** folder

      4. Select the project > right click > select  properties > java build path > select Libraries> select classpath> Add Jars > (a popup will appear) > select the files, you just pasted inside the current projects **lib** folder > press apply ![](https://lh4.googleusercontent.com/75B3ewhN37u-1jU3A73YGx-5TKpSu8zppaLlF1Qt2Y_08YDe2ES0j4ZERe7TVvon3P18jkhtVNFU_-0VREccPHjUNbFL8ncM2wyGFAl8dd49GRQ9oaFXERumSewMdgOzyL-lP6NVEIdBso4Ut7JkbCA)

      5. After completion of installation, a new folder named “Reference Libraries” will be added. 

         1. ![](https://lh6.googleusercontent.com/K9jMKiRvC0wx93MiBp9cnTUO7GZBoVcd2Jre9OsZ0I2ry8xghkhhCkGRFR6tH-Tij_q7b3-kxaTf2glM7SzFSAzdqKzhs5lb5pHTnFZaLUvK42WJvdq6xJELNd04Irf50yXB2z5VPsoBKzxjLi1UFkI)

      6. Some packages are still missing in the latest updates, they introduce alternatives. However, if you still need them add the jars. For example, the JPA api package is not available in the required folder, you can download it or you can find it inside the provided folder of the latest version.

5. Testing Your JDBC Connection - [08-test-jdbc-connection.pdf](https://drive.google.com/file/d/1LlD6gnGeYlEa02h10ssGoWLRlAsioAn2/view?usp=share_link)\| [7 Testing Your JDBC Connection - YouTube](https://www.youtube.com/watch?v=kRJ00LGhZ7Q&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=7&ab_channel=freeCodeCampBengali)**Step 3:** Setting/Adding Up a Database Table [06_hibernate_setup_sample_data.pdf](https://drive.google.com/file/d/1v9eVwB9PTvhcx3cW7VoBkXI0YYacOigq/view?usp=share_link)\| [Video](https://www.youtube.com/watch?v=JghD0Fe2bc4&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=5&ab_channel=freeCodeCampBengali) \| [sql-scripts](https://drive.google.com/drive/folders/1W0hAMliNrR3AEl_aY3bTCis7NULBMoEJ?usp=share_link)**Creating an USER**:**In the simplest form, the syntax for CREATE USER command is as below:**CREATE USER \[IF NOT EXISTS] '{username}'@'{hostname}' IDENTIFIED BY '{passwordString}';📂 01-create-user.sql|                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CREATE USER 'hbstudent'@'localhost' IDENTIFIED BY 'hbstudent'; GRANT ALL PRIVILEGES ON \* . \* TO 'hbstudent'@'localhost'; -- The asterisks in this command refer to the database and table (respectively), another example mydb.\* , where the second star refers to all the tables.\-- resetting the native root password, if the system did not replace it already ALTER USER 'hbstudent'@'localhost' IDENTIFIED WITH mysql_native_password BY 'hbstudent'; |Explanation: [MySQL: Grant all privileges on database](https://stackoverflow.com/questions/5016505/mysql-grant-all-privileges-on-database#:~:text=Therefore%2C%20the%20first,databases%20and%20tables.) ; [How to Reset the Root Password](https://dev.mysql.com/doc/refman/5.7/en/resetting-permissions.html#:~:text=it%20to%20stop.-,Create%20a%20text%20file%20containing%20the%20password%2Dassignment%20statement%20on%20a,USER%20%27root%27%40%27localhost%27%20IDENTIFIED%20BY%20%27MyNewPass%27%3B,-Save%20the%20file) ;📂 02-student-tracker.sql|                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CREATE DATABASE IF NOT EXISTS \`hb_student_tracker\`; USE \`hb_student_tracker\`; -- -- Table structure for table \`student\` -- DROP TABLE IF EXISTS \`student\`; CREATE TABLE \`student\` (   \`id\` int(11) NOT NULL AUTO_INCREMENT,   \`first_name\` varchar(45) DEFAULT NULL,   \`last_name\` varchar(45) DEFAULT NULL,   \`email\` varchar(45) DEFAULT NULL,   PRIMARY KEY (\`id\`) ) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=latin1; |**Step 5**: Testing the JDBC connection, [7 Testing Your JDBC Connection - YouTube](https://www.youtube.com/watch?v=kRJ00LGhZ7Q&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=7&ab_channel=freeCodeCampBengali)|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| public class TestJdbc { public static void main(String\[] args) { // TODO Auto-generated method stub String jdbcUrl = "jdbc:mysql://localhost:3306/hb_student_tracker"; //String jdbcUrl = "jdbc:mysql://localhost:3306/hb_student_tracker?useSSL=false&serverTimezone=UTC"; String user = "hbstudent"; String password = "hbstudent"; try { System.out.println("Connecting to the database: " + jdbcUrl); Connection myConn = DriverManager.getConnection(jdbcUrl,user,password); System.out.println("Connection Successful"); } catch(Exception exc){ exc.printStackTrace(); } } } |**


# Chapter 3: Hibernate Development and CRUD


##### **Hibernate Development Process Overview [09-hibernate-dev-process.pdf](https://drive.google.com/file/d/1-LC9mnXYoaHoZVjOWQbD4VNsfeSxmCLe/view?usp=share_link)\| [ovvwVid](https://www.youtube.com/watch?v=jEc70A8FDEc&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=8&ab_channel=freeCodeCampBengali) [configVid](https://www.youtube.com/watch?v=s7tY1EB0Xso&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=9&ab_channel=freeCodeCampBengali) [annotationVid1](https://www.youtube.com/watch?v=VXlTRAQ9Ii8&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=12&ab_channel=freeCodeCampBengali)To Do List:1. Add Hibernate Configuration file
2. Annotate Java Class
3. Develop Java Code to perform database operations - Hibernate CRUD**


## Hibernate Configuration with Annotations


##### **[10-hibernate-config.pdf](https://drive.google.com/file/d/1mUxcWUJvhjC4NhW1FhoqW-e0A4M4mWMQ/view?usp=sharing) [Video](https://www.youtube.com/watch?v=s7tY1EB0Xso&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=9&ab_channel=freeCodeCampBengali)Creating the Hibernate Configuration File - - Copy the config file from the starter and paste it to the eclipse project.Config files tell the hibernate how to connect to the database.![](https://lh4.googleusercontent.com/m6hpy_Hb-23sOAsYmGEcCSjtQ2BN4pcO8QOSKIuG6INVXOUL4ODSw46DLaZwZIFtCOVhslA4Axip3QgsoZGq65TpYI7pyIgrArBTly8ukqrVU4-___FVqrIM1lZSN7l2uhT6qbe-UYA45c7YVoZhNu4)Config file - [Hibernate - Configuration (tutorialspoint.com)](https://www.tutorialspoint.com/hibernate/hibernate_configuration.htm) \| [Hibernate Configuration - javatpoint](https://www.javatpoint.com/hibernate-configuration)|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;!DOCTYPE hibernate-configuration PUBLIC         "-//Hibernate/Hibernate Configuration DTD 3.0//EN"         "http&#x3A;//www.hibernate.org/dtd/hibernate-configuration-3.0.dtd"> &lt;hibernate-configuration>     &lt;session-factory>         &lt;!-- JDBC Database connection settings -->         &lt;property name="connection.driver_class">com.mysql.cj.jdbc.Driver&lt;/property>         &lt;property name="connection.url">jdbc:mysql://localhost:3306/hb_student_tracker?useSSL=false&amp;amp;serverTimezone=UTC&lt;/property>         &lt;property name="connection.username">hbstudent&lt;/property>         &lt;property name="connection.password">hbstudent&lt;/property>         &lt;!-- JDBC connection pool settings ... using built-in test pool -->         &lt;property name="connection.pool_size">1&lt;/property>         &lt;!-- Select our SQL dialect -->         &lt;property name="dialect">org.hibernate.dialect.MySQLDialect&lt;/property>         &lt;!-- Echo the SQL to stdout -->         &lt;property name="show_sql">true&lt;/property> &lt;!-- Set the current session context --> &lt;property name="current_session_context_class">thread&lt;/property>       &lt;/session-factory> &lt;/hibernate-configuration> |Explanation:1.  &lt;session-factory> -

2. "connection.pool_size" - Connection Pool

3. "dialect" - SQL Dialect

   1. [SQL Dialect](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.vjtcp6xa8779)

4. &lt;property name="show_sql">true&lt;/property>

   1. [Hibernate show real SQL \[duplicate\] - java](https://stackoverflow.com/questions/2536829/hibernate-show-real-sql)
   2. [java - How to print a query string with parameter values when using Hibernate - Stack Overflow](https://stackoverflow.com/questions/1710476/how-to-print-a-query-string-with-parameter-values-when-using-hibernate)Connection with the database will be established with the config file in place. Now, we need to map the class and fields to the database table and columns respectively.**


## Hibernate ORM Annotations 


##### **[11-hibernate-annotations.pdf](https://drive.google.com/file/d/17f91FFAHiEy0Gz15YGoo23jY6VgCL3QH/view?usp=share_link)Object-to-Relational Mapping (ORM): ![](https://lh3.googleusercontent.com/lWRSAbdA5wMxBrh7EKRqjj2OHtM-szAETXKaGtsOCZl3BN1VXkmEaQo5GcofZ1nm4OQ2HS8_bqgxk1VOt78sCp5ki5MXpVvdWlfcNbmdtxgUaeEm36c9vpLT9BauIFbpGIbOnCVpEpjugXu-MrjTjT8)Two Options for Mapping- Option 1: XML config file (legacy)
- Option 2: Java Annotations (modern, preferred)**Option 2: Java Annotations |** [annotationVid1](https://www.youtube.com/watch?v=VXlTRAQ9Ii8&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=12&ab_channel=freeCodeCampBengali) **,** [annoCodeVid2](https://www.youtube.com/watch?v=oCrVaMOjrp8&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=11&ab_channel=freeCodeCampBengali)- Step 1: Map class to database table
- Step 2: Map fields to database columns
- Extra: Add necessary class fields and methods.**Step 1**: Map class to database table|                                                                |
| -------------------------------------------------------------- |
| @Entity  @Table(name="student") public class Student {  ...  } |![](https://lh5.googleusercontent.com/aL5uwnE8bqsfVgrbbf5Ipe6o5kLiTfADk8OeU5H7aCyLD33h7c-vyyAeyk4VfQqnHOaVKx3vyVjyXGNbalffBzzmM92gdEZQXt5b3d_V8ag_VsOgjX7RxjkrWlZ__KQtSRJszlaMf61iwOYDAEMBVyY)**FAQ**- HEADS UP - FOR JAVA 9 USERS
- HEADS UP - JAVA 9 USERS - Eclipse Generate toString() fails
- javax.persistence.Entity Package errors > add the jar.**Step 2**: Map fields to database columns | |                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| import javax.persistence.\*;@Entity @Table(name="student") public class Student { @Id @Column(name="id") private int id; @Column(name="first_name") private String firstName; ... } |![](https://lh6.googleusercontent.com/szbS339t-E71Vv77WT3Bfm7htcD7LOltAR6kgL-DUKNIs1PJCYZopjbb6GKri-IT0DnYpJtM2Ijmqzjgry2DxbaBhffgONenY5RnEkpHfJKupn_GgzcbhMijJSDGsh7MtoaOmccOA2cXoGzIJx0gz5Q)**FAQ:**- FAQ: Why are we using JPA Annotation instead of Hibernate?
- FAQ: Can Hibernate generate database tables based on the Java code?**Hibernate Annotations** :1. @Entity 
2. @Table: use to make a table and change the table details
3. @Id:  
4. @GeneratedValue - 
5. @Column: to change the details of columns. If you don't pass the name argument, then the column name will be the same as the field name in the entity class.
6. @Transient: Tells hibernate not to save this field. Suppose our student class had a field named city and if we wanted hibernate not to save it we would use @Transient. 
7. @Temporal 
8. @Lob tells hibernate that it is a large object, not a simple object. Example: blob, clob
9. @OneToOne, @OneToMany, @ManyToMany , @JoinColumn etcFull code:|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| @Entity @Table(name="student") public class Student {  @Id @Column(name="id") private Integer id;  @Column(name="first_name") private String first_name; @Column(name="last_name") private String last_name; @Column(name="email") private String email; public Student(String first_name, String last_name, String email) { super(); this.first_name = first_name; this.last_name = last_name; this.email = email; } public Integer getId() { return id; } public void setId(Integer id) { this.id = id; } public String getFirst_name() { return first_name; } public void setFirst_name(String first_name) { this.first_name = first_name; } public String getLast_name() { return last_name; } public void setLast_name(String last_name) { this.last_name = last_name; } public String getEmail() { return email; } public void setEmail(String email) { this.email = email; } @Override public String toString() { return "student \[id=" + id + ", first_name=" + first_name + ", last_name=" + last_name + ", email=" + email + "]"; } } |**


## Hibernate Crud


##### **[What is Hibernate caching? Introduction of first-level & second-level cache | by Darshan Dalwadi | Jan, 2021 | Medium | The Startup](https://medium.com/swlh/what-is-hibernate-caching-introduction-of-level-1-level-2-cache-8ea7339a5052)**


### Creating and Saving Java Objects in the Database 


##### **[12-hibernate-save.pdf](https://drive.google.com/file/d/1SETojBkAsnGIB9cmagvy0vHKUrp4fHmu/view?usp=share_link)- Creating and Saving Java Objects - [Part 1 ](https://www.youtube.com/watch?v=NOAD7B-SqfU&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=12&pp=sAQB)

  1. Creating SessionFactory
  2. Create Session
  3. Create Object
  4. Begin Transaction
  5. Save the object
  6. Close the Transaction

- Creating and Saving Java Objects - [Part 2](https://www.youtube.com/watch?v=hYT4LTAgzgY&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=13&ab_channel=freeCodeCampBengali)|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| public class CreateStudentDemo { public static void main( String\[] args )     { /\* Part 1: Setting up the configuration \*/     System.out.println( "Project Started" );     Configuration cfg = new Configuration();cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Student.class);//Point 1    SessionFactory factory = cfg.buildSessionFactory();     System.out.println( factory );         //Create Session     Session session = factory.getCurrentSession();         /\* Part 2: Saving the object to the database \*/     try {     //create object         System.out.println( "Creating new student object" );         Student student1 = new Student("Sanjida","Arno","sanj@gmail.com");         System.out.println(student1);        /\*Block 1: Starts\*/         //begin a transaction         session.beginTransaction();                 //saving the object         System.out.println( "Saving the new student object" );         session.save(student1);                 //commit a transaction         session.getTransaction().commit();         /\*Block 1: ends\*/         //closing the session         session.close();         System.out.println("Done");     }finally {     factory.close();     }     } } |
|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |Point 1 => you can try an alternative approach remove this .addAnnotatedClass(Student.class); and then adding a &lt;mapping class="com.diptopaul.hibernate.demo.entity.Student">&lt;/mapping> in the cfg file instead. Also you can [add multiple entity classes](https://copyprogramming.com/howto/add-annotated-class-in-hibernate-by-adding-all-classes-in-some-package-java) just like .addAnnotatedClass(Flight.class).addAnnotatedClass(Sky.class).addAnnotatedClass(Person.class)Block 1=> Alternative Approach|                                                                                    |
| ---------------------------------------------------------------------------------- |
| Transaction tx  = session.beginTransaction(); session.save(student1); tx.commit(); |Topic to Read further:1. [Sessions and transactions| JBoss.org Content Archive (Read Only)](https://developer.jboss.org/docs/DOC-13951)
2.
3.FAQ:1. Once you run the code if you see an **_Error: Exception in thread "main" java.lang.NoClassDefFoundError: javax/xml/bind/JAXBException_**

   1. This happens because of Java 9 and higher. 

   2. Java 9 and higher has removed java.xml.bind from its default classpath. That's why we get the class not found exception.  We have to explicitly add JAR files to the build path.

   3. you need additional JAR files.

      1. [javax.activation-1.2.0.jar](http://search.maven.org/remotecontent?filepath=com/sun/activation/javax.activation/1.2.0/javax.activation-1.2.0.jar)
      2. [jaxb-api-2.3.0.jar](http://search.maven.org/remotecontent?filepath=javax/xml/bind/jaxb-api/2.3.0/jaxb-api-2.3.0.jar)
      3. [jaxb-core-2.3.0.jar](http://search.maven.org/remotecontent?filepath=com/sun/xml/bind/jaxb-core/2.3.0/jaxb-core-2.3.0.jar)
      4. [jaxb-impl-2.3.0.jar](http://search.maven.org/remotecontent?filepath=com/sun/xml/bind/jaxb-impl/2.3.0/jaxb-impl-2.3.0.jar)

2. Exception in thread "main" java.lang.NoClassDefFoundError: javax/transaction/SystemException

   1. Add the jar dist\\lib\\provided\\jboss-transaction-api_1.2_spec-1.0.0.Final.jar

3. [Does committing a transaction closes session? (Object Relational Mapping forum at Coderanch)](https://www.coderanch.com/t/428509/databases/committing-transaction-closes-session) \| [Should I use session.close() after each Hibernate Search? - Hibernate Search - Hibernate](https://discourse.hibernate.org/t/should-i-use-session-close-after-each-hibernate-search/1473/2)**


#### Primary Keys -[13-hibernate-primary-keys.pdf](https://drive.google.com/file/d/1D_BKBNeavfSLgY_hyLPJzXAjYNS3A1JL/view?usp=share_link)\|


##### **- Primary Keys - Overview -  [3 Primary Keys Overview - YouTube](https://www.youtube.com/watch?v=QtWNAThQzlY&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=14&ab_channel=freeCodeCampBengali)

- 05:54

- Primary Keys - Write Some Code - [4 Primary Keys Write Some Code - YouTube](https://www.youtube.com/watch?v=d23tgelr1mU&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=15&ab_channel=freeCodeCampBengali)

- 07:11

- Primary Keys - Changing the Starting Index - [5 Primary Keys Changing the Starting Index - YouTube](https://www.youtube.com/watch?v=f9Kl--zwtoQ&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=16&ab_channel=freeCodeCampBengali)

  1. ALTER TABLE hb_student_tracker student AUTO_INCREMENT= 3000;
  2. Then try to insert or try to save using hibernateNeed to read: [JPA + Hibernate - Primary Key, @Id and @GeneratedValue Examples (logicbig.com)](https://www.logicbig.com/tutorials/java-ee-tutorial/jpa/jpa-primary-key.html)**


#### Frequent Errors:


##### **1.  GenerationTarget encountered exception accepting command : Error executing DDL create table student address (address Id integer not null, city varchar(50), street varchar(100), primary key (address_Id)) type=MyISAM via JDBC Statement

   1. Solution: Changing the Dialect in Xml cfg file to org.hibernate.dialect.MySQL8Dialect

2. Hibernate : No CurrentSessionContext configured

   1.  Solution: Define this in cfg: &lt;property name="current_session_context_class">thread&lt;/property>**


### Reading Objects with Hibernate - [14-hibernate-read.pdf](https://drive.google.com/open?id=17yTYgWpdL1Gq_jD5Mph8hQD45lg1ATsx&usp=drive_copy)


##### **- Reading Objects with Hibernate - [14-hibernate-read.pdf](https://drive.google.com/open?id=17yTYgWpdL1Gq_jD5Mph8hQD45lg1ATsx&usp=drive_copy) \| [6 Reading Objects with Hibernate - YouTube](https://www.youtube.com/watch?v=RfhfGrA0Fnk&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=17&ab_channel=freeCodeCampBengali)Retrieving a Java Object with Hibernate // create Java objectStudent theStudent = new Student(“Daffy”, “Duck”, “daffy@luv2code.com");// save it to databasesession.save(theStudent);//… Create a new session to read an item from dbsession = factory.getCurrentSession();session.beginTransaction();// now retrieve/read from database using the primary keyStudent myStudent =session.get(Student.class, theStudent.getId());//Commit the transaction and close the sessionsession.getTransaction().commit();**


### Querying Objects with Hibernate [15-hibernate-query.pdf](https://drive.google.com/file/d/1knvGv1J7p8S3XhPJTMj1BH-o4_FeQ23m/view?usp=share_link)


##### **- Querying Objects with Hibernate - Overview [7 Querying Objects with Hibernate Overview - YouTube](https://www.youtube.com/watch?v=O1Ls42WP-6k&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=18&ab_channel=freeCodeCampBengali)
- 03:30
- [Special Note about Deprecated Method in Hibernate 5.2](https://drive.google.com/file/d/1kqOJkRkVnDOG4pzmlAbgAMA_CxK-pbt2/view?usp=share_link)
- 00:07
- Querying Objects with Hibernate - Write Some Code - Part 1 [9 Querying Objects with Hibernate Write Some Code Part 1 - YouTube](https://www.youtube.com/watch?v=_BQu5JQXt2Q&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=19&ab_channel=freeCodeCampBengali)
- 06:56
- Querying Objects with Hibernate - Write Some Code - [Part 2](https://www.youtube.com/watch?v=hm-GTtHWYoY&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=20&ab_channel=freeCodeCampBengali)
- 06:59
- FAQ: [How To View Hibernate SQL Parameter Values](https://drive.google.com/open?id=1Cw2Vaq4oR0JkXwIRJn2AD1AEPD5wqXph&usp=drive_copy)
- 02:04
- FAQ: [how-to-read-dates-with-hibernate.pdf](https://drive.google.com/open?id=1RijUiW7xTUDnnrjxD6eNt0Y7_Jtja69E&usp=drive_copy)Pending: [how-to-read-dates-with-hibernate.pdf](https://drive.google.com/open?id=1RijUiW7xTUDnnrjxD6eNt0Y7_Jtja69E&usp=drive_copy)**


#### Revise [SQL](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.wrhaoomrg4gj)


#### Take a Look in HQL


##### **- [Hibernate - Query Language (tutorialspoint.com)](https://www.tutorialspoint.com/hibernate/hibernate_query_language.htm)

- [Hibernate - Native SQL (tutorialspoint.com)](https://www.tutorialspoint.com/hibernate/hibernate_native_sql.htm) - more like traditional SQL in hibernate methods.

- How to set parameter inside hibernate query string - [HQL (Hibernate Query Language) Tutorial with Examples - javatpoint](https://www.javatpoint.com/hql)

  - Transaction tx=session.beginTransaction();  
  - Query q=session.createQuery("update User set name=:n where id=:i");  
  - q.setParameter("n","Udit Kumar");  
  - q.setParameter("i",111);  **


### Updating Objects with Hibernate [16-hibernate-update.pdf](https://drive.google.com/open?id=1hNhxpJpLZwBH-FJv3x5L6EWuMJP3kTR5&usp=drive_copy)


##### **- Updating Objects with Hibernate - Overview [12 Updating Objects with Hibernate Overview - YouTub](https://www.youtube.com/watch?v=8JiVxWHkEgs&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=21&ab_channel=freeCodeCampBengali)
- Updating Objects with Hibernate - Write Some Code [13 Updating Objects with Hibernate Write Some Code - YouTube](https://www.youtube.com/watch?v=1ac7H4gYtr4&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=22&ab_channel=freeCodeCampBengali)
- 07:57**


### Deleting Objects with Hibernate [17-hibernate-delete.pdf](https://drive.google.com/file/d/1PLIHAyC0iMQ3c0WABypj-7WB736bYp4Y/view?usp=share_link)


##### **- Deleting Objects with Hibernate - Overview [14 Deleting Objects with Hibernate Overview - YouTube](https://www.youtube.com/watch?v=Sjkliy33g0A&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=23&ab_channel=freeCodeCampBengali)
- 02:45
- Deleting Objects with Hibernate - Write Some Code [15 Deleting Objects with Hibernate Write Some Code - YouTube](https://www.youtube.com/watch?v=qq9oZEP16J0&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=24&ab_channel=freeCodeCampBengali)
- 06:33
- Practice Activity #8 - Hibernate Development
- 00:30
- FAQ: How to read Dates with Hibernate
- 02:35**


# Chapter 4: Hibernate Terms


##### **1. Hibernate Session - [Object States in Hibernate’s Session | Baeldung](https://www.baeldung.com/hibernate-session-object-states#:~:text=The%20Session%20interface%20is%20the,operations%2C%20and%20then%20close%20it.)**


# Chapter 5: Hibernate Advance


##### **[18-hibernate-advanced-mappings-overview.pdf](https://drive.google.com/file/d/1bCEVgL_ppfwL9Imvb1twGJRa0iYx85MT/view?usp=share_link)**


## Hibernate Advanced Mappings 


##### **2 lectures • 8min- Advanced Mappings Overview
- Preview02:56
- Database Concepts
- 05:15If there is **ManyToOne** or **ManyToMany** or **ManyToSomething** relationship then we can **not do cascade delete**.**


## Hibernate Advanced Mappings - @OneToOne


##### **Constraint Clause: [CONSTRAINT clause (oracle.com)](https://docs.oracle.com/javadb/10.8.3.0/ref/rrefsqlj13590.html#:~:text=A%20CONSTRAINT%20clause%20is%20an,Constraint%20names%20are%20optional.&text=Column%2Dlevel%20constraints%20refer%20to,name%20(except%20check%20constraints).) \| [CONSTRAINT Clause - Microsoft Support](https://support.microsoft.com/en-us/office/constraint-clause-e5241593-139a-4eb7-ad30-61026873191e)**


### @OneToOne Uni- Directional


##### **[19-hibernate-one-to-one-uni-overview-part-1.pdf](https://drive.google.com/open?id=1jSx7soHrswRmGacJ0JMRVFEd66m5q0hQ&usp=drive_copy)  [20-hibernate-one-to-one-uni-overview-part-2.pdf](https://drive.google.com/open?id=19R8sk7VEnuRyeYE0584MrkMFDD7VREaK&usp=drive_copy) [21-hibernate-one-to-one-uni-overview-part-3.pdf](https://drive.google.com/open?id=1ZRnIt2biqV3uP7_Rj0m0qcfEBGC3JbDr&usp=drive_copy)[22-hibernate-one-to-one-uni.pdf](https://drive.google.com/open?id=1Ql59ZxnscdyabTwsPtg414LpNG4kTQ5S&usp=drive_copy)- [1 @OneToOne Overview Part 1 - YouTube](https://www.youtube.com/watch?v=Znp2J8FPqhQ&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=27&ab_channel=freeCodeCampBengali)
- [2 @OneToOne Overview Part 2 - YouTube](https://www.youtube.com/watch?v=hGtFYf_05VI&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=28&ab_channel=freeCodeCampBengali)
- [3 @OneToOne - Overview - Part 3](https://www.youtube.com/watch?v=U_lfInBXjl0&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=29&ab_channel=freeCodeCampBengali)**Development Process: One-to-One (Step-By-Step)**1. Prep Work - Define database tables

   1. [4 @OneToOne Run Database Scripts - YouTube](https://www.youtube.com/watch?v=49R7e-ej7rA&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=30&ab_channel=freeCodeCampBengali)

   2. [5 @OneToOne Write Some Code Prep Work - YouTube](https://www.youtube.com/watch?v=Apv_q8ykeL8&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=31&ab_channel=freeCodeCampBengali)

      1. Start a new project
      2. Add Config file with new db name
      3. Test the jdbc connection.

2. Create InstructorDetail class 

   1. [6 @OneToOne Write Some Code Create InstructorDetail class - YouTube](https://www.youtube.com/watch?v=JKrWg2UpWXQ&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=32&ab_channel=freeCodeCampBengali)

3. Create Instructor class

   1. [7 @OneToOne Write Some Code Create Instructor class - YouTube](https://www.youtube.com/watch?v=NKZoDYiQC8k&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=33&ab_channel=freeCodeCampBengali)

4. Create Main App

   1. [8 @OneToOne Write Some Code Build Main App Part 1 - YouTube](https://www.youtube.com/watch?v=AZSfNplxOPA&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=34&ab_channel=freeCodeCampBengali)
   2. [9 @OneToOne Write Some Code Build Main App Part 2 - YouTube](https://www.youtube.com/watch?v=CXET2OpxN6Q&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=35&ab_channel=freeCodeCampBengali)**Step 1:** Prep Work - Define database tablestable: instructor_detailFile: create-db.sqlCREATE TABLE \`instructor_detail\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`youtube_channel\` varchar(128) DEFAULT NULL,\`hobby\` varchar(45) DEFAULT NULL,PRIMARY KEY (\`id\`));table: instructorFile: create-db.sqlCREATE TABLE \`instructor\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`first_name\` varchar(45) DEFAULT NULL,\`last_name\` varchar(45) DEFAULT NULL,\`email\` varchar(45) DEFAULT NULL,\`instructor_detail_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),CONSTRAINT \`FK_DETAIL\` FOREIGN KEY (\`instructor_detail_id\`)REFERENCES \`instructor_detail\` (\`id\`)...);Constraint Clause: [CONSTRAINT clause (oracle.com)](https://docs.oracle.com/javadb/10.8.3.0/ref/rrefsqlj13590.html#:~:text=A%20CONSTRAINT%20clause%20is%20an,Constraint%20names%20are%20optional.&text=Column%2Dlevel%20constraints%20refer%20to,name%20(except%20check%20constraints).) \| [CONSTRAINT Clause - Microsoft Support](https://support.microsoft.com/en-us/office/constraint-clause-e5241593-139a-4eb7-ad30-61026873191e)![](https://lh3.googleusercontent.com/Zvs8ar5wHmK-mJcUgWSIXOd9L-UYECdth8a8t8h6w4qKEdDv1pVv3JxtAi8RbGWSl0zp_nU_ZpyLivsrgoppQ1aUo_0kDHjInXyvFV0b3iqtjn7JqpqgvUe5cEXkAirRrDx7A1FOoND_j6RrOr09aRE)**Step 2**: Create InstructorDetail class@Entity@Table(name="instructor_detail")public class InstructorDetail {@Id@GeneratedValue(strategy=GenerationType.IDENTITY)@Column(name="id")private int id;@Column(name="youtube_channel")private String youtubeChannel;@Column(name="hobby")private String hobby;// constructors// getters / setters}**Step 3**: Create Instructor class@Entity@Table(name="instructor")public class Instructor {@Id@GeneratedValue(strategy=GenerationType.IDENTITY)@Column(name="id")private int id;@Column(name="first_name")private String firstName;@Column(name="last_name")private String lastName;@Column(name="email")private String email;@OneToOne@JoinColumn(name=“instructor_detail_id")private InstructorDetail instructorDetail;...// constructors, getters / setters}@OneToOne mapping![](https://lh5.googleusercontent.com/xUpSweuSNw7PpIYEJ5PgZOzO2HHwF50Tf4uS78iKIxqLL7s2BNi8LeoG4sfFVMiF9eeYi1yuDfXbt7AmnTioViyT8dr7zEIIIa3NLklE0ty3UgBDlgXIjnCDGozNHnTbXh_9I__pr0DuLKKXIEwP1Gc)![](https://lh4.googleusercontent.com/YrQF7USFINyYeMhFllJno65FUbyGYxF8kIRhureAkJO5lgsuLSlBIjGf7SGeB1qBfiHhDpsHAJ5S8tVW7G3E4H6GUAf_IkXjtJBJyfVm9CPh5P6QQZWFH2hTlTrXgxFPNrH2nwLqof-tePogOUqFlM0)Now the question is If we make any changes in the foreign key table, how is it going to affect the referred field? For example if we delete the referred field or if we delete the foreign key table, what action will be performed?We can Cascade operations by defining cascade types. More about [Cascade](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.bxy12egc0zak).**Updated**:@Entity@Table(name="instructor")public class Instructor {...@OneToOne(cascade=CascadeType.ALL)@JoinColumn(name="instructor_detail_id")private InstructorDetail instructorDetail;...// constructors, getters / setters}Note: By default, no operations are cascaded. **Step 4**: Create Main Apppublic static void main(String\[] args) {...// create the objectsInstructor tempInstructor = new Instructor("Chad", "Darby", "darby@luv2code.com");InstructorDetail tempInstructorDetail =new InstructorDetail(“http&#x3A;//www.luv2code.com/youtube", "Luv 2 code!!!");// associate the objectstempInstructor.setInstructorDetail(tempInstructorDetail);// start a transactionsession.beginTransaction();session.save(tempInstructor);// commit transactionsession.getTransaction().commit();...}**


#### Entity Lifecycle ( Delete an Entity)


##### **- [10 @OneToOne Delete an Entity - YouTube](https://www.youtube.com/watch?v=0Vv6HEEQ3AM&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=36&ab_channel=freeCodeCampBengali)//begin a transaction         session.beginTransaction();                 //get the instructor using the primary key/ id         int insId = 1;         Instructor tempIns = session.get(Instructor.class, insId);         System.out.println("Found Instructor: " + tempIns);                 //delete the instructor         if(tempIns!=null) {         System.out.println("Deleting Instructor: " + tempIns);         // Note: this will also delete its associated "details" object, because of CascadeType.ALL         session.delete(tempIns);         }                 // commit transaction         session.getTransaction().commit();**


### @OneToOne - Cascade


##### **[21-hibernate-cascade.pdf](https://drive.google.com/open?id=1ZRnIt2biqV3uP7_Rj0m0qcfEBGC3JbDr&usp=drive_copy)[2 @OneToOne Overview Part 2 - YouTube](https://www.youtube.com/watch?v=hGtFYf_05VI&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=29&ab_channel=freeCodeCampBengali)**


### @OneToOne - Entity Lifecycle


##### **[20-hibernate-one-to-one-uni-overview-part-2.pdf](https://drive.google.com/file/d/19R8sk7VEnuRyeYE0584MrkMFDD7VREaK/view?usp=sharing)**Clarification of terms**In [UML](https://docs.oracle.com/cd/A97335_02/apps.102/bc4j/developing_bc_projects/Glossary.htm#UML) terms, An entity is a domain-specific noun, such as a customer, order, or item. Entity class defines what property the entities will have. And Instances of Entity class is called Entity object. [Glossary (oracle.com)](https://docs.oracle.com/cd/A97335_02/apps.102/bc4j/developing_bc_projects/Glossary.htm#entity). **Sometimes by saying entities some people refer to a collection of entity instances.**[Are entities (in an Entity relationship diagram) correspond to rows in a table, or are they distinctly named tables? - Quora](https://www.quora.com/Are-entities-in-an-Entity-relationship-diagram-correspond-to-rows-in-a-table-or-are-they-distinctly-named-tables)**Transient** The lifecycle state of a newly instantiated entity object is called transient. The entity hasn’t been persisted yet, so it doesn’t represent any database record. (Now, for better understanding read the Persistent or Managed state, then come back)Your persistence context doesn’t know about your newly instantiated object. As long as your entity object is in the lifecycle state transient, you can think of it as a basic Java object without any connection to the database and any JPA-specific functionality.Author author = new Author();author.setFirstName("Thorben");author.setLastName("Janssen");To change the state of Transient to Managed state we use hibernate session’s save/get etc method or JPA entity manager’s persist/save etc method.**Persistent or Managed State**Student student1 = new Student("Sanji","Cute","[arno@gmail.com](mailto:arno@gmail.com)"); // (1)         System.out.println(student1);                 //begin a transaction         session.beginTransaction();                 //saving the object         System.out.println( "Saving the new student object" );         session.save(student1); // (2)         student1.setFirstName("Arno");// Will this work? (3)              //commit a transaction         session.getTransaction().commit(); // (4)- (1) > Right now object is in Transient State
- (2) > Object is in Persistent or Managed state, The current student is saved in the heap cache. It will be visible to the db after execution of the commit method. If you perform a detach method to the object at this point after step 2, the value already being saved in the cache will still be seen in the db. 
- (3) > This will work, just after using the save method, the Student entity object gets attached to the current persistence context. As a result it went to the JPA entity lifecycle (Hibernate lifecycle) managed/persistent state. That means that the persistence provider, e.g. Hibernate, will detect any changes on the objects and generate the required SQL INSERT or UPDATE statements when it flushes the persistence context.
- (4) After committing, the object student1 goes to Detached state. Any changes to the object will only affect the object itself not the db. We can also detach it before the commit method by using detach method, see detail in detach state example.There are different ways to get an entity to the lifecycle state managed:1. You can call the EntityManager.persist method of JPA  or  with a new entity object. em.persist(student1);// similar to save method2. You can load an entity object from the database using the EntityManager.find method

   1. Student student = em.find(Student.class, ‘5’); // Similar to hibernate get method

3. You can merge a detached entity by calling the EntityManager.merge method or update it by calling the update method on your Hibernate Session.

   1. em.merge(student1);

4. Use the Hibernate Save or **Get** or Load method etc.session.beginTransaction();int studentId = 2;Student tempStudent = session.get(Student.class, studentId); // went to the managed statetempStudent.setFirstName("Kurup"); // any changes will reflect to the database after commitsession.getTransaction().commit();1.**Detached State:**An entity that was previously managed but is no longer attached to the current persistence context is in the lifecycle state detached.An entity gets detached when you close the persistence context. That typically happens after a request gets processed. Then the database transaction gets committed, the persistence context gets closed, and the entity object gets returned to the caller. The caller then retrieves an entity object in the lifecycle state detached.Detaching an entity from Sessionsession.close();_//or_session.evict(entity);You can also programmatically detach an entity by calling the _detach_ method on the _EntityManager_.em.detach(author);Student student1 = new Student("Sanji","Cute","arno@gmail.com"); // (1)         System.out.println(student1);                 //begin a transaction         session.beginTransaction();                 //saving the object         System.out.println( "Saving the new student object" );         session.save(student1); // (2)          student1.setFirstName("Arno");// Will this work? (3)      session.detach(student1); (4)         //commit a transaction         session.getTransaction().commit(); // (5)System.out.println(student1); // (6)- (1) > Right now object is in Transient State
- (2) > Object is in Persistent or Managed state, The current student is saved in the heap cache. It will be visible to the db after execution of the commit method. If you perform a detach method to the object at this point after step 2, the value already being saved in the cache will still be seen in the db. 
- (3) and (4) > This will not work. Changes made in step (3) are not saved in the heap cache. Thus when we perform detach operation, the object gets detached and as a result any changes that we did in step (3) on the student1 object will not be visible in the db after the execution of the commit method.
- (5) The object student1 is already in the detached state. After committing, any pending changes to the object will only affect the object itself, not the db. See the print in (6)**Reattaching an entity:**session.detach(student1); // student 1 goes to detached state         student1.setFirstName("Afrin");// Will this get reflected on db?         student1.setLastName("Mourni");// Will this ..?         session.merge(student1); // Until this point the line above this would not have gotten reflected on the db, but now after executing merge the object will reattach to the persistence context and thus going to persistent state again. As a result after commit the changes will be reflected in the db.**Removed State:**When you call the remove method on your EntityManager, the mapped database record doesn’t get removed immediately. The entity object only changes its lifecycle state to removed.During the next flush operation, Hibernate will generate an SQL DELETE statement to remove the record from the database table.em.remove(author);Or Hibernate Sessions remove method,session.remove(employee);Full Example:session.beginTransaction();int studentId = 13;Student tempStudent = session.get(Student.class, studentId); (1)session.delete(tempStudent); // (2)\*session.getTransaction().commit(); // (3)- (1) Goes to Managed or Persistent state
- (2)\* Goes to removed state
- (3) after commit execution the hibernate will generate an SQL DELETE statement to remove it completely. And the entity lifecycle will enter the transient state.Other ways to get to the removed state > [Deleting Objects with Hibernate | Baeldung](https://www.baeldung.com/delete-with-hibernate)Sources: [Entity Lifecycle Model in JPA & Hibernate (thorben-janssen.com)](https://thorben-janssen.com/entity-lifecycle-model/#JPA8217s_Persistence_Context), Also Read [Hibernate Entity Lifecycle | Baeldung](https://www.baeldung.com/hibernate-entity-lifecycle)**


### @OneToOne - Bi-Directional 


##### **[23-hibernate-one-to-one-bi-overview.pdf](https://drive.google.com/open?id=1gap5mRk1639Kyvr_6oGiNVMIDln3WhFU&usp=drive_copy)- [11 @OneToOne Bi Directional Overview - YouTube](https://www.youtube.com/watch?v=w4JKADpw8ek&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=37&ab_channel=freeCodeCampBengali)So far we have uni-directional mapping.![](https://lh5.googleusercontent.com/AMSS8bgcXk6CfR9v4mGUQhkKLi_n_MKA00lETPqvlCZBIyDXhHIRS7i9ZQl51E34qwvqWZX58w-SvioBY96OyL6_EH0HEEXN4bk4ie_COsk6LRVniWy-ASP5DWkfsdUtsZs5gdpbK_8wyq0maTiB440)Sometimes we might want to get the associated Instructor whenever we load the InstructorDetails. In some cases it's necessary to have this feature. But we can’t do this with the current uni-directional relationship. We can accomplish this by using bi-directional one to one mapping.![](https://lh6.googleusercontent.com/sNyFO_QO0BjpEOBOlqKst9Rwwhinh0r-c9ls0ZXbm23TvwjWyFbmw236ap5OByO8Wh9Ms31wYMRb6W56BZ4TbIzq1gW9jzLy6hdrpD1mrKiOQC0bjN8UTEBK4rVO_M5egVHBfaXXw9dJxc8NGFhrGAQ)- We can start with InstructorDetail and make it back to the Instructor
- **We can keep the existing database schema. No changes required to the database.**
- Simply update the Java code. Use mappedBy.Development Process: One-to-One (Bi-Directional)Step-By-Step1. No Changes in DB Schema

2. Make updates to InstructorDetail class: [12 @OneToOne Bi Directional Create Relationship - YouTube](https://www.youtube.com/watch?v=AoX2yoerE3o&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=38&ab_channel=freeCodeCampBengali)

   1. Add new field to reference Instructor
   2. Add getter/setter methods for Instructor
   3. Add @OneToOne annotation with mappedBy argument

3. Create Main App

   1. [13 @OneToOne Bi Directional Develop Main App - YouTube](https://www.youtube.com/watch?v=CdihDrhKSDk&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=39&ab_channel=freeCodeCampBengali)More on mappedBy- mappedBy tells Hibernate
- Look at the instructorDetail property in the Instructor class
- Use information from the Instructor class @JoinColumn
- To help find associated instructorStep 2: update InstructorDetail class/\*CREATE TABLE \`instructor_detail\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`youtube_channel\` varchar(128) DEFAULT NULL,\`hobby\` varchar(45) DEFAULT NULL,PRIMARY KEY (\`id\`));\*/@Entity@Table(name="instructor_detail")**public** **class** InstructorDetail {@Id@GeneratedValue(strategy=GenerationType.**_IDENTITY_**)@Column(name="id")**private** **int** id;@Column(name="youtube_channel")**private** String youtubeChannel;@Column(name="hobby")**private** String hobby;//new field@OneToOne(mappedBy="instructorDetail", cascade={CascadeType.**_DETACH_**,CascadeType.**_MERGE_**,CascadeType.**_PERSIST_**,CascadeType.**_REFRESH_**})// if instructorDetail gets deleted its associated Instructor will remain saved, since cascadeType remove is not provided//@OneToOne(mappedBy="instructorDetail", cascade=CascadeType.ALL)//instructorDetail is a variable of InsDetail class inside Instructor class**private** Instructor instructor;//getter setterStep 3:[14 @OneToOne Refactoring and Exception Handling - YouTube](https://www.youtube.com/watch?v=OCtnAKkhEcw&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=40&ab_channel=freeCodeCampBengali)**


#### Delete in Bidirectional


##### **[15 @OneToOne Bi Directional Cascade Delete - YouTube](https://www.youtube.com/watch?v=kaT8hGmkXRo&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=41&ab_channel=freeCodeCampBengali)OneToOne Bi Directional Delete Only InstructorDetail:[16 @OneToOne Bi Directional Delete Only InstructorDetail Part 1 - YouTube](https://www.youtube.com/watch?v=nwK5q2MWh2M&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=42&ab_channel=freeCodeCampBengali)[17 @OneToOne Bi Directional Delete Only InstructorDetail Part 2 - YouTube](https://www.youtube.com/watch?v=KSFX32W6K0Y&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=44&ab_channel=freeCodeCampBengali)Steps: 1. Change cascadeType to cascade={CascadeType.**_DETACH_**,CascadeType.**_MERGE_**,CascadeType.**_PERSIST_**,CascadeType.**_REFRESH_**})
2. In the main app, you will encounter an error: deleted object would be re-saved by cascade, if you try to delete at this point. The solution to error is to remove the associated object reference, thus breaking the bidirectional link. tempInstructorDetail.getInstructor().setInstructorDetail(null);
3.**


## Hibernate Advanced Mappings - @OneToMany


### @OneToMany - Bi-Directional


##### **[24-hibernate-one-to-many-overview.pdf](https://drive.google.com/open?id=10jL3SmitvDKG68L9kWHpxyNHMgQqHrWA&usp=drive_copy)10 lectures • 43min- [1 @OneToMany Bi Directional Overview Part 1 - YouTube](https://www.youtube.com/watch?v=418aW7_h-cw&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=44)
- Preview 04:13
- @OneToMany - Bi-Directional Overview - Part 2
- Preview 03:41
- @OneToMany - Bi-Directional - Database Prep Work
- 04:36
- @OneToMany - Bi-Directional - Create Course Mapping
- 05:01
- @OneToMany - Bi-Directional - Define Course Relationship
- 03:06
- @OneToMany - Bi-Directional - Update Instructor
- 04:54
- @OneToMany - Bi-Directional - Add Instructor to Database
- 04:39
- @OneToMany - Bi-Directional - Create Courses for Instructor
- 05:04
- @OneToMany - Bi-Directional - Retrieve Instructor Courses
- 03:40
- [10 @OneToMany Bi Directional Delete a Course - YouTube](https://www.youtube.com/watch?v=a3idBcklVA8&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=54)
- 04:24[Spring Data JPA One to Many Bidirectional Mapping (javaguides.net)](https://www.javaguides.net/2022/02/spring-data-jpa-one-to-many-bidirectional-mapping.html)Bi-directional in One-to-Many will have Many-to-One relationship as well,One-to-Many Mapping- An instructor can have many coursesMany-to-One Mapping- Many courses can have one instructor
- Inverse / opposite of One-to-ManyReal-World Project Requirement- If you delete an instructor, DO NOT delete the courses

- If you delete a course, DO NOT delete the instructor

  - Do not apply cascading deletes!![](https://lh4.googleusercontent.com/Uk_15EwgVQ-NY7ZpzcTnfCdPDc0exxsTOmBrAChcs4KgJraZ2thEUJyu_ffFZI7Au_iS0w7iew8g0JoANgzcG5N8R9ordFT0-Yvh83OquQzWhmLXsQJOlGYmAooXFW3KmKpr-jXJojBtN93V9-6HGsQ)**Development Process: One-to-Many**Step-By-Step1. Prep Work - Define database tables

2. Create Course class

   1. Add support for Cascading 

      1. Do not apply cascading deletes!

3. Update Instructor class

   1. Add support for Cascading 

      1. Do not apply cascading deletes!

   2. Add convenience methods for bi-directional

4. Create Main App**Step 1**: Prep Work - Define database tablesDROP schema if exists \`hb-03-one-to-many\`;CREATE SCHEMA \`hb-03-one-to-many\`;use \`hb-03-one-to-many\`;SET FOREIGN_KEY_CHECKS =0;DROP TABLE IF EXISTS \`instructor_detail\`;CREATE TABLE \`instructor_detail\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`youtube_channel\` varchar(128) DEFAULT NULL,\`hobby\` varchar(45) DEFAULT NULL,PRIMARY KEY (\`id\`)) ENGINE=InnoDB auto_increment=1 default charset=latin1;DROP TABLE IF EXISTS \`instructor\`;CREATE TABLE \`instructor\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`first_name\` varchar(45) DEFAULT NULL,\`last_name\` varchar(45) DEFAULT NULL,\`email\` varchar(45) DEFAULT NULL,\`instructor_detail_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),CONSTRAINT \`FK_DETAIL\` FOREIGN KEY (\`instructor_detail_id\`)REFERENCES \`instructor_detail\` (\`id\`) ON DELETE NO ACTION ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;SET FOREIGN_KEY_CHECKS = 1;DROP TABLE IF EXISTS \`course\`;CREATE TABLE \`course\`(\`id\` int(11) NOT NULL auto_increment,\`title\` varchar(128) DEFAULT NULL,\`instructor_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),UNIQUE KEY \`TITLE_UNIQUE\` (\`title\`),KEY \`FK_INSTRUCTOR_idx\` (\`instructor_id\`),constraint \`FK_INSTRUCTOR\` FOREIGN KEY (\`instructor_id\`) references \`instructor\` (\`id\`)ON DELETE NO ACTION ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;**Step 2**: Create Course class1. Add support for Cascading 

   1. Do not apply cascading deletes!@Entity@Table(name="course")**public** **class** Course {@Id@GeneratedValue(strategy=GenerationType.**_IDENTITY_**)@Column(name="id")**private** **int** id;@Column(name="title")**private** String title;@ManyToOne(cascade= {CascadeType.**_DETACH_**, CascadeType.**_MERGE_**, CascadeType.**_PERSIST_**, CascadeType.**_REFRESH_**})// cascading delete is not applied@JoinColumn(name="instructor_id")**private** Instructor instructor;// add constructor// add getter setter}**Step 3**: Update Instructor class2. Add convenience methods for bi-directional

3. Add support for Cascading 

   1. Do not apply cascading deletes!@Entity@Table(name="instructor")**public** **class** Instructor {@Id@GeneratedValue(strategy=GenerationType.**_IDENTITY_**)@Column(name="id")**private** **int** id;@Column(name="first_name")**private** String firstName;@Column(name="last_name")**private** String lastName;@Column(name="email")**private** String email;@OneToOne(cascade=CascadeType.**_ALL_**)@JoinColumn(name="instructor_detail_id")//name of the fk column in the db**private** InstructorDetail instructorDetail;@OneToMany(mappedBy="instructor", cascade= {CascadeType.**_DETACH_**, CascadeType.**_MERGE_**, CascadeType.**_PERSIST_**, CascadeType.**_REFRESH_**})**private** List&lt;Course> courses;//Q: How do we add data in the course list field? By calling the convenience method add and passing a course argument./\*\* (mappedBy="instructor") >> Refers to “instructor” property in “Course” class\* mappedBy tells Hibernate\* • Look at the instructor property in the Course class\* • Use information from the Course class @JoinColumn\* • To help find associated courses\*/// add constructor// add getter setter//add convenience methods for bi-directional relationship**public** **void** add(Course tempCourse) {**if** (courses == **null**) {courses = **new** ArrayList&lt;>();}courses.add(tempCourse);tempCourse.setInstructor(**this**);}}}**Step 4**: Create Main App1. **CreateInstructorDemo****public** **class** CreateInstructorDemo{**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**);//Point 1   SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );       //Create Session    Session session = factory.getCurrentSession();       /\* Part 2: Saving the object to the database \*/    **try** {    //create object        System.**_out_**.println( "Creating new student object" );        // create the objects        Instructor tempInstructor = **new** Instructor("Paul", "Alan", "alany@lharverd.edu");        InstructorDetail tempInstructorDetail =  **new** InstructorDetail("http&#x3A;//www.youtube.com", "CS Teaching!!!");        // associate the objects        tempInstructor.setInstructorDetail(tempInstructorDetail);        System.**_out_**.println(tempInstructor);        /\*Block 1: Starts\*/        //begin a transaction        session.beginTransaction();               //saving the object        System.**_out_**.println( "Saving the new Instructor object" );        session.save(tempInstructor);               //commit a transaction        session.getTransaction().commit();        /\*Block 1: ends\*/        System.**_out_**.println("Done");    }    **catch**(Exception exc){        exc.printStackTrace();       }    **finally** {        //closing the session, handles the connection leak issue        session.close();        factory.close();       }   }}2. **CreateCourseDemoAssignThemToInstructor****public** **class** CreateCourseDemoAssignThemToInstructor{**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**);//Point 1   SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );       //Create Session    Session session = factory.getCurrentSession();       /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/        //begin a transaction        session.beginTransaction();           //create object        System.**_out_**.println( "Creating new Course object" );        // create the objects        Course tempCourse = **new** Course("Data Structure");        Course tempCourse2 = **new** Course("Algorithm");        System.**_out_**.println(tempCourse);               // Assign the course to an Ins        //get the instructor        **int** insId = 1;        Instructor tempIns = session.get(Instructor.**class**, insId);        tempIns.add(tempCourse);        tempIns.add(tempCourse2);               System.**_out_**.println(tempIns);               session.save(tempCourse);        session.save(tempCourse2);               //commit a transaction        session.getTransaction().commit();        /\*Block 1: ends\*/        System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}3. **GetInstructorCoursesDemo****public** **class** GetInstructorCoursesDemo{**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();    cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**);//Point 1       SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );           //Create Session    Session session = factory.getCurrentSession();    /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/    //begin a transaction    session.beginTransaction();    //get the instructor    **int** insId = 1;    Instructor tempIns = session.get(Instructor.**class**, insId);    System.**_out_**.println(tempIns.getCourses());    //commit a transaction    session.getTransaction().commit();    /\*Block 1: ends\*/    System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}4. DeleteCourseDemo**


### Eager vs Lazy Loading


##### **[25-hibernate-fetch-types-eager-vs-lazy-overview.pdf](https://drive.google.com/open?id=1hGGnOp-stVSh_5r3943oyMmU44-5nLKY&usp=drive_copy)8 lectures • 36min- Eager vs Lazy Loading - Overview - Part 1
- Preview03:17
- Eager vs Lazy Loading - Overview - Part 2
- Preview 05:16
- Eager vs Lazy Loading - Coding - Eager
- 08:08
- Eager vs Lazy Loading - Coding - Lazy
- 04:00
- Eager vs Lazy Loading - Coding - Closing the Session
- 04:07
- Eager vs Lazy Loading - Coding - Resolve Lazy Loading Issue
- 03:21
- Eager vs Lazy Loading - Coding - HQL JOIN FETCH
- 06:37
- FAQ: How to load the courses at a later time in the application?
- 01:05Default Fetch Types|              |                        |
| ------------ | ---------------------- |
| **Mapping**  | **Default Fetch Type** |
| @OneToOne    | FetchType.EAGER        |
| @OneToMany   | FetchType.LAZY         |
| @ManyToOne   | FetchType.EAGER        |
| @ManyToMany  | FetchType.LAZY         |public class EagerLazyDemo {public static void main( String\[] args )    {     //CODES     // cODES     try {     // CODES     Instructor tempIns = session.get(Instructor.class, insId);// line 1     System.out.println("Instructor: " + tempIns);         System.out.println("Courses: " + tempIns.getCourses());// line 3     //commit a transaction     session.getTransaction().commit();     /\*Block 1: ends\*/     System.out.println("Done");     }    }}**Eager output**Hibernate: select instructor0\_.id as id1_1_0\_, instructor0\_.email as email2_1_0\_, instructor0\_.first_name as first_na3_1_0\_, instructor0\_.instructor_detail_id as instruct5_1_0\_, instructor0\_.last_name as last_nam4_1_0\_, courses1\_.instructor_id as instruct3_0_1\_, courses1\_.id as id1_0_1\_, courses1\_.id as id1_0_2\_, courses1\_.instructor_id as instruct3_0_2\_, courses1\_.title as title2_0_2\_, instructor2\_.id as id1_2_3\_, instructor2\_.hobby as hobby2_2_3\_, instructor2\_.youtube_channel as youtube_3_2_3\_ from instructor instructor0\_ left outer join course courses1\_ on instructor0\_.id=courses1\_.instructor_id left outer join instructor_detail instructor2\_ on instructor0\_.instructor_detail_id=instructor2\_.id where instructor0\_.id=?Instructor: Instructor \[id=1, firstName=Paul, lastName=Alan, email=alany@lharverd.edu, instructorDetail=InstructorDetail \[id=1, youtubeChannel=http&#x3A;//www.youtube.com, hobby=CS Teaching!!!]]Courses: \[Course \[id=1, title=SPL, instructor=Instructor \[id=1, firstName=Paul, lastName=Alan, email=alany@lharverd.edu, instructorDetail=InstructorDetail \[id=1, youtubeChannel=http&#x3A;//www.youtube.com, hobby=CS Teaching!!!]]], Course \[id=2, title=Algorithm, instructor=Instructor \[id=1, firstName=Paul, lastName=Alan, email=alany@lharverd.edu, instructorDetail=InstructorDetail \[id=1, youtubeChannel=http&#x3A;//www.youtube.com, hobby=CS Teaching!!!]]]]DoneExplanation: In the output line 1(green) for having eager fetch type in the Instructor entity, whenever we try to fetch the Instructor table(code line 1), the application specifically hibernate will fetch all the associated entity tables from the database and put them in the temporary memory. For that reason, next time whenever a user requests for the course table(at code line 3), hibernate won't fetch the table data from the database , instead it will serve the data from memory.**Lazy output****Hibernate: select instructor0\_.id as id1_1_0\_, instructor0\_.email as email2_1_0\_, instructor0\_.first_name as first_na3_1_0\_, instructor0\_.instructor_detail_id as instruct5_1_0\_, instructor0\_.last_name as last_nam4_1_0\_, instructor1\_.id as id1_2_1\_, instructor1\_.hobby as hobby2_2_1\_, instructor1\_.youtube_channel as youtube_3_2_1\_ from instructor instructor0\_ left outer join instructor_detail instructor1\_ on instructor0\_.instructor_detail_id=instructor1\_.id where instructor0\_.id=?****Instructor: Instructor \[id=1, firstName=Paul, lastName=Alan, email=alany@lharverd.edu, instructorDetail=InstructorDetail \[id=1, youtubeChannel=http&#x3A;//www.youtube.com, hobby=CS Teaching!!!]]****Hibernate: select courses0\_.instructor_id as instruct3_0_0\_, courses0\_.id as id1_0_0\_, courses0\_.id as id1_0_1\_, courses0\_.instructor_id as instruct3_0_1\_, courses0\_.title as title2_0_1\_ from course courses0\_ where courses0\_.instructor_id=?****Courses: \[Course \[id=1, title=SPL, instructor=Instructor \[id=1, firstName=Paul, lastName=Alan, email=alany@lharverd.edu, instructorDetail=InstructorDetail \[id=1, youtubeChannel=http&#x3A;//www.youtube.com, hobby=CS Teaching!!!]]], Course \[id=2, title=Algorithm, instructor=Instructor \[id=1, firstName=Paul, lastName=Alan, email=alany@lharverd.edu, instructorDetail=InstructorDetail \[id=1, youtubeChannel=http&#x3A;//www.youtube.com, hobby=CS Teaching!!!]]]]****Done**Explanation: In the output line 1(green) for having Lazy fetch type in the Instructor entity, whenever we try to fetch the Instructor table(code line 1), the application specifically hibernate will fetch all only the data of instructor table (which includes a instructor detail column) from the database and put them in the temporary memory. However, whenever a user requests for the course table(at code line 3), hibernate will fetch the course table data from the database, since it is not available in the memory.**More about Lazy Loading**- When you lazy load, the data is only retrieved on demand

- However, this requires an open Hibernate session

  - need an connection to database to retrieve data

-  If the Hibernate session is closed

  - And you attempt to retrieve lazy data
  - Hibernate will throw an exception Watch out for this!

- To retrieve lazy data, you will need to open a Hibernate session

- Retrieve lazy data using

  - Option 1: session.get and call appropriate getter method(s)
  - Option 2: Hibernate query with HQLMany other techniques available but the two above are most common**


### @OneToMany - Unidirectional


##### **[26-hibernate-one-to-many-uni-overview.pdf](https://drive.google.com/open?id=1emaCgGQDiDascsZzHVniUOVk3TVwXTKI&usp=drive_copy)9 lectures • 38min- @OneToMany - Uni-Directional - Overview - Part 1
- Preview03:52
- @OneToMany - Uni-Directional - Overview - Part 2
- Preview03:26
- FAQ: @JoinColumn ... where does it find the column?
- 01:03
- @OneToMany - Uni-Directional - Set up database tables
- 04:16
- @OneToMany - Uni-Directional - Create Review Class
- 05:53
- @OneToMany - Uni-Directional - Configure Fetch Type
- 04:43
- @OneToMany - Uni-Directional - Create Course Reviews
- 07:56
- @OneToMany - Uni-Directional - Get Course Reviews
- 03:35
- @OneToMany - Uni-Directional - Delete Course Reviews
- 03:14DROP TABLE IF EXISTS \`review\`;CREATE TABLE \`review\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`comment\` varchar(256) DEFAULT NULL,\`course_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),KEY \`FK_COURSE_ID_idx\` (\`course_id\`),CONSTRAINT \`FK_COURSE\` FOREIGN KEY (\`course_id\`) references \`course\` (\`id\`)ON DELETE CASCADE ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;**Development Process: One-to-Many**Step-By-Step1. Prep Work - Define database tables

2. Create Review class

3. Update Course class

   1. Add convenient method addReview

4. Create Main App**Step 1**: Prep Work - Define database tablesDROP TABLE IF EXISTS \`review\`;CREATE TABLE \`review\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`comment\` varchar(256) DEFAULT NULL,\`course_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),KEY \`FK_COURSE_ID_idx\` (\`course_id\`),CONSTRAINT \`FK_COURSE\` FOREIGN KEY (\`course_id\`) references \`course\` (\`id\`)ON DELETE CASCADE ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;**Step 2:** Create Review class@Entity@Table(name="review")**public** **class** Review {@Id@GeneratedValue(strategy=GenerationType.**_IDENTITY_**)@Column(name="id")**private** **int** id;@Column(name="comment")**private** String comment;}**Step 3**: Update Course class@Entity@Table(name="course")**public** **class** Course {@Id@GeneratedValue(strategy=GenerationType.**_IDENTITY_**)@Column(name="id")**private** **int** id;@Column(name="title")**private** String title;@ManyToOne(cascade= {CascadeType.**_DETACH_**, CascadeType.**_MERGE_**, CascadeType.**_PERSIST_**, CascadeType.**_REFRESH_**})@JoinColumn(name="instructor_id")**private** Instructor instructor;@OneToMany(fetch=FetchType.**_LAZY_**, cascade=CascadeType.**_ALL_**)@JoinColumn(name="course_id")**private** List&lt;Review> reviews;// add convenience methods for adding reviewspublic void addReview(Review tempReview) {if (reviews == null) {reviews = new ArrayList&lt;>();}reviews.add(tempReview);}}Step 4:**public** **class** CreateCoursesReviewDemo_AssignThemToCourses{**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();    cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**).addAnnotatedClass(Review.**class**);//Point 1       SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );           //Create Session    Session session = factory.getCurrentSession();    /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/    //begin a transaction    session.beginTransaction();    //get the instructor    **int** courseId = 1;    Course tempCourse = session.get(Course.**class**, courseId);       //Create Reviews    Review tempReview = **new** Review("SPL is one of the most fundamental course.");    Review tempReview2 = **new** Review("Understanding of SPL will innensly help learning other programming language.");       // Assign the reviews to a course    tempCourse.add(tempReview);    tempCourse.add(tempReview2);    System.**_out_**.println(tempCourse.getReviews());    //commit a transaction    session.getTransaction().commit();    /\*Block 1: ends\*/    System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}GetCoursesReviewDemo    /\* Part 2: Get the review of courses from the database \*/    **try** {    /\*Block 1: Starts\*/    //begin a transaction    session.beginTransaction();    //get the instructor    **int** courseId = 1;    Course tempCourse = session.get(Course.**class**, courseId);    System.**_out_**.println(tempCourse.getReviews());    //commit a transaction    session.getTransaction().commit();    /\*Block 1: ends\*/    System.**_out_**.println("Done");    }**


## Hibernate Advanced Mappings - @ManyToMany


##### **[27-hibernate-many-to-many-overview.pdf](https://drive.google.com/open?id=1IYARulyMKgF8adUMPlQEOVHbKDzCphCv&usp=drive_copy)13 lectures • 56min**


### Overview


##### **[1 @ManyToMany Overview Part 1 - YouTube](https://www.youtube.com/watch?v=vEblVfy_9NY&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=69&ab_channel=freeCodeCampBengali) \| [2 @ManyToMany Overview Part 2 - YouTube](https://www.youtube.com/watch?v=HeScUTRM8OQ&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=70&ab_channel=freeCodeCampBengali)Many-to-Many Mapping- A course can have many students
- A student can have many courses![](https://lh3.googleusercontent.com/IGBCLFg7cfEBdK4OS3ry9o8hzGSQTH7TQrfaOem32HtlwWJ3wraMW1rgU6y_zowLwmCd83oq5NEFEySuc0FYPXP27rYetE76_raLIanlxJ-ZME8Y9oaxAs5Y8KDLFgeIXU8jLekQxZKXrTAjoujVA4A)- Need to track which student is in which course and vice-versa

  - A **Join Table** is used to **keep the track.******![](https://lh4.googleusercontent.com/Pgp-zrdE3om_mIE_Cnp7Rp-_-cnRqM67hR9V0NDFK_dNXSHTTRshKlTNAV7uEncUw6xsLeClnEJYbZOQihNEReDhQRwqMZbUqGFnyE_LdSATcmxGl--f6HiLZzHP9zn4PSaJp7C5NvbZeOclBXCOkqE)******Join Table**A table that provides a mapping between two tables. It has foreign keys for each table to define the mapping relationship.![](https://lh4.googleusercontent.com/zA4L-TkWurVEVqqpUADPQwt0qpgxKG_Nf---4LcHQjCKESQZ2eIGPYqz0Of-XdRXXE6-GR6TQ8fQ95w6ReQIMKjmQRKThffJzbNcKj6pCvaxouo6vWQ8TyEvjz793CYPVpHKXPM74iSZInrFq2-8ftU)![](https://lh4.googleusercontent.com/xfPzjFNzj6eL9Vcf5Fn2qszar2Z8hPSeiAqJ-9tGVtqj9OBRsSJ9tSo_DOtZ8GaEjZ7teiSNKxnuDTTyu_Pp9EUK4Qah9ciPzdAZpOh10q_hSszQrsRdRro7Ed9JJmLlW-6BXtkzN3eKapNZXrauItg)**


### Development Process: Many-to-Many


##### **Step-By-Step1. Prep Work - Define database tables

   1. join table: course_student

2. Update Course class

   1. reference students
   2. Add @ManyToMany annotation
   3. Add @JoinTable

3. Update Student class

   1. reference students
   2. Add @ManyToMany annotation
   3. Add @JoinTable

4. Create Main App- [11 @ManyToMany Get Courses for Student - YouTube](https://www.youtube.com/watch?v=4VczskgQFJQ&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=79&ab_channel=freeCodeCampBengali)
- [12 @ManyToMany Delete a Course - YouTube](https://www.youtube.com/watch?v=1Nq9lHNySNg&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=80&ab_channel=freeCodeCampBengali)**Step 1: Prep Work - Define database tables** [**3 @ManyToMany Set up database tables - YouTube**](https://www.youtube.com/watch?v=Si8PA3tzOMY&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=71&ab_channel=freeCodeCampBengali)DROP schema if exists \`hb-05-many-to-many\`;CREATE SCHEMA \`hb-05-many-to-many\`;use \`hb-05-many-to-many\`;SET FOREIGN_KEY_CHECKS =0;DROP TABLE IF EXISTS \`student\`;CREATE TABLE \`student\` (  \`id\` int(11) NOT NULL AUTO_INCREMENT,  \`first_name\` varchar(45) DEFAULT NULL,  \`last_name\` varchar(45) DEFAULT NULL,  \`email\` varchar(45) DEFAULT NULL,  PRIMARY KEY (\`id\`)) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=latin1;DROP TABLE IF EXISTS \`instructor_detail\`;CREATE TABLE \`instructor_detail\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`youtube_channel\` varchar(128) DEFAULT NULL,\`hobby\` varchar(45) DEFAULT NULL,PRIMARY KEY (\`id\`)) ENGINE=InnoDB auto_increment=1 default charset=latin1;DROP TABLE IF EXISTS \`instructor\`;CREATE TABLE \`instructor\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`first_name\` varchar(45) DEFAULT NULL,\`last_name\` varchar(45) DEFAULT NULL,\`email\` varchar(45) DEFAULT NULL,\`instructor_detail_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),CONSTRAINT \`FK_DETAIL\` FOREIGN KEY (\`instructor_detail_id\`)REFERENCES \`instructor_detail\` (\`id\`) ON DELETE NO ACTION ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;SET FOREIGN_KEY_CHECKS = 1;DROP TABLE IF EXISTS \`course\`;CREATE TABLE \`course\`(\`id\` int(11) NOT NULL auto_increment,\`title\` varchar(128) DEFAULT NULL,\`instructor_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),UNIQUE KEY \`TITLE_UNIQUE\` (\`title\`),KEY \`FK_INSTRUCTOR_idx\` (\`instructor_id\`),constraint \`FK_INSTRUCTOR\` FOREIGN KEY (\`instructor_id\`) references \`instructor\` (\`id\`)ON DELETE NO ACTION ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;DROP TABLE IF EXISTS \`review\`;CREATE TABLE \`review\` (\`id\` int(11) NOT NULL AUTO_INCREMENT,\`comment\` varchar(256) DEFAULT NULL,\`course_id\` int(11) DEFAULT NULL,PRIMARY KEY (\`id\`),KEY \`FK_COURSE_ID_idx\` (\`course_id\`),CONSTRAINT \`FK_COURSE\` FOREIGN KEY (\`course_id\`) references \`course\` (\`id\`)ON DELETE CASCADE ON UPDATE NO ACTION)ENGINE=InnoDB auto_increment=1 default charset=latin1;DROP TABLE IF EXISTS \`course_student\`;CREATE TABLE \`course_student\`(\`course_id\` int(11) NOT NULL,\`student_id\` int(11) NOT NULL,PRIMARY KEY (\`course_id\`, \`student_id\`),CONSTRAINT \`FK_COURSE_05\` FOREIGN KEY (\`course_id\`) REFERENCES \`course\` (\`id\`),CONSTRAINT \`FK_STUDENT\` FOREIGN KEY (\`student_id\`) REFERENCES \`student\` (\`id\`))ENGINE=InnoDB auto_increment=1 default charset=latin1;![](https://lh3.googleusercontent.com/vKHomXuPTTokFkkBOEOpJHN1yvcAiRlOXBWmiq1E4RkklytXOIVKy2eNtsFtrGPKivQeqyu7k7WtjP3Ps1e-Vl4JJOthqPwqHtKqolXgGWFXKXIF8bSQm20V_jpAV53blZpOAqpiDMtXvuddvEv4qK4)**Step 2:** Update Course class =>  [4 @ManyToMany Update Course class - YouTube](https://www.youtube.com/watch?v=OpNMODVFlo4&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=72&ab_channel=freeCodeCampBengali) \| [5 @ManyToMany Configure Course for many to many - YouTube](https://www.youtube.com/watch?v=0HffRM1Yzdc&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=73&ab_channel=freeCodeCampBengali)1. reference students
2. Add @ManyToMany annotation
3. Add @JoinTables@Entity@Table(name="course")public class Course {@ManyToMany@JoinTable(name="course_student",joinColumns=@JoinColumn(name="course_id"),inverseJoinColumns=@JoinColumn(name="student_id"))private List&lt;Student> students;// getter / setters//add convenience methods for adding reviewspublic void addStudent(Student tempStudent) {if (students == null) {students = new ArrayList&lt;>();}students.add(tempStudent);}}**Step 3: Update Student class =>** [6 @ManyToMany Configure Student for many to many - YouTube](https://www.youtube.com/watch?v=HmH2VM_6-Aw&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=74&ab_channel=freeCodeCampBengali)1. reference students
2. Add @ManyToMany annotation
3. Add @JoinTable@Entity@Table(name="student")public class Student {@ManyToMany@JoinTable(name="course_student",joinColumns=@JoinColumn(name="student_id"),inverseJoinColumns=@JoinColumn(name="course_id"))private List&lt;Course> courses;// getter / setters}**More: @JoinTable (In the context of Course class)**@JoinTable tells Hibernate- Look at the course_id column in the course_student table
- For other side (inverse), look at the student_id column in the course_student table
- Use this information to find relationship between course and students****![](https://lh5.googleusercontent.com/Bw-dh9Z57O_9cvdc6gzVEDyXGY7cxmb_iV7BSRMQXd-4kf4pSm_cS3sLPTUyzhabcIPEgfQsV0GGLAZ8hQM34ycMijk_36e_NaFffxVJnB17wYThvttaMOEc3k5IkNtOxHlBMLDFOabebMrf77Gboa8)******More on “inverse”**- In this context, we are defining the relationship in the **Course** class
- The **Student** class is on the “other side” ... so it is considered the “inverse”
- “Inverse” refers to the “other side” of the relationship****![](https://lh6.googleusercontent.com/xI3qoWSRZzw1vuwrNAoUyRQOf2BYb0cQxd18eeZWI19T_qdhpyhMnmwQcIrxHTji-JhiKuYfjQJm0GtJ6mWhAXOvnNlpk1i32v1sHjFGf6d7eNQmOIHL-SI4dTFYEszgXfAhDABiKPjH_6wlPR4m1fw)******Now, In the context of Student class let’s do a similar thing, just going the other way******![](https://lh6.googleusercontent.com/AyvG_gwbElSv0T01GPFbKm5dcxd5Sj0gqOe616pFO8dHkhUW4YdvkPHiJLpZz-88vJ82pqkPCCSi6JudW6lTIsj31SvJCmd-5VsGbEMKFPVYtLPNZ4-qo8nK2pYwnUVBEIobdH26gVh_rMTzNdEIiAU)******Real-World Project Requirement**- If you delete a course, DO NOT delete the students. DO NOT apply cascading deletes!![](https://lh4.googleusercontent.com/0jpjXuCreIslUPtXbPdgzLp9anyeMkiJ7QKG-ciPBwLNJTa0tOtaLqQqLxReLj1NMq8Lc60LSyAalhp8Ub0NUx8E8RPL_9LWbr6_fFY-s4iWkNAM_wGf_z5adRxdvMKOvnvcUiWjNv5SpnZpRf_tFk4)**Step 4:** Create Main App - [7 @ManyToMany Create a Main App - YouTube](https://www.youtube.com/watch?v=hQE0ZVG0MQs&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=75&ab_channel=freeCodeCampBengali)
- [8 @ManyToMany Review the app output - YouTube](https://www.youtube.com/watch?v=1PesbmWm0Do&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=77&ab_channel=freeCodeCampBengali) - Shows hibernate inserting data into Join Table1)**public** **class** AssignCourseToStudentDemo {**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();    cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**).addAnnotatedClass(Review.**class**).addAnnotatedClass(Student.**class**);//Point 1       SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );       //Create Session    Session session = factory.getCurrentSession();       /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/        //begin a transaction        session.beginTransaction();           //get a course        System.**_out_**.println( "Get the Course object" );        // create the objects        **int** courseId = 1;        Course tempCourse = session.get(Course.**class**, courseId);        System.**_out_**.println(tempCourse);               // Assign the course to an Student        //get the instructor        **int** studentId = 1;        Student tempStudent = session.get(Student.**class**, studentId);        // replace this with an add method in the entity        List &lt;Course> tempCourses = tempStudent.getCourses();        tempCourses.add(tempCourse);        tempStudent.setCourses(tempCourses);       //        List &lt;Student> tempStudents = tempCourse.getStudents();//        tempStudents.add(tempStudent);//        tempCourse.setStudents(tempStudents);               session.save(tempStudent);        session.save(tempCourse);               //commit a transaction        session.getTransaction().commit();        /\*Block 1: ends\*/        System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}2) **Add more courses to an Already existing Student:**- [9 @ManyToMany Add more courses for a student - YouTube](https://www.youtube.com/watch?v=7lLHEr_4qG8&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=77&ab_channel=freeCodeCampBengali)
- [10 @ManyToMany Verify Data in Join Table - YouTube](https://www.youtube.com/watch?v=CJ0ccuRZLVE&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=78&ab_channel=freeCodeCampBengali)3) [11 @ManyToMany Get Courses for Student - YouTube](https://www.youtube.com/watch?v=4VczskgQFJQ&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=79&ab_channel=freeCodeCampBengali)**public** **class** GetCoursesOfStudent {**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();    cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**).addAnnotatedClass(Review.**class**).addAnnotatedClass(Student.**class**);//Point 1       SessionFactory factory = cfg.buildSessionFactory();       //Create Session    Session session = factory.getCurrentSession();       /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/        //begin a transaction        session.beginTransaction();           //get a course        System.**_out_**.println( "Get the Course object" );        // create the objects        **int** studentId = 8;        Student tempStudent = session.get(Student.**class**, studentId);        System.**_out_**.println(tempStudent);        System.**_out_**.println();               List &lt;Course> tempCourses = tempStudent.getCourses();        System.**_out_**.println(tempCourses);// show lazy or details               //commit a transaction        session.getTransaction().commit();        /\*Block 1: ends\*/        System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}4) [12 @ManyToMany Delete a Course - YouTube](https://www.youtube.com/watch?v=1Nq9lHNySNg&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=80&ab_channel=freeCodeCampBengali) to check if the student cascade no delete is working.5) [13 @ManyToMany Delete a Student - YouTube](https://www.youtube.com/watch?v=w8Cn6wa6ZxI&list=PLon9KQO-XVctd1ZYrKAq3xFa8HR1iGWZ3&index=81&ab_channel=freeCodeCampBengali) to check if the course cascade no delete is working.6)**public** **class** GetStudentsOfACourse {**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();    cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**).addAnnotatedClass(Review.**class**).addAnnotatedClass(Student.**class**);//Point 1       SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );       //Create Session    Session session = factory.getCurrentSession();       /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/        //begin a transaction        session.beginTransaction();           //get a course        System.**_out_**.println( "Get the Course object" );        // create the objects        **int** courseId = 1;        Course tempCourse = session.get(Course.**class**, courseId);        System.**_out_**.println(tempCourse);               List &lt;Student> tempStudents = tempCourse.getStudents();        System.**_out_**.println(tempStudents);               //commit a transaction        session.getTransaction().commit();        /\*Block 1: ends\*/        System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}7) **public** **class** DeleteCoursesOfStudentDemo{**public** **static** **void** main( String\[] args )   {/\* Part 1: Setting up the configuration \*/    System.**_out_**.println( "Project Started" );    Configuration cfg = **new** Configuration();    cfg.configure("hibernate.cfg.xml").addAnnotatedClass(Instructor.**class**).addAnnotatedClass(InstructorDetail.**class**).addAnnotatedClass(Course.**class**).addAnnotatedClass(Review.**class**).addAnnotatedClass(Student.**class**);//Point 1       SessionFactory factory = cfg.buildSessionFactory();    System.**_out_**.println( factory );       //Create Session    Session session = factory.getCurrentSession();       /\* Part 2: Saving the object to the database \*/    **try** {    /\*Block 1: Starts\*/        //begin a transaction        session.beginTransaction();               // Get the student first        **int** studentId = 1;        Student tempStudent = session.get(Student.**class**, studentId);               List &lt;Course> tempCourses = tempStudent.getCourses();           //Remove the course        System.**_out_**.println( "Removing the Course object" );        **int** courseId = 2;        // get the course objects        Course tempCourse = session.get(Course.**class**, courseId);        **if**(tempCourse!=**null**)        {        tempCourses.remove(tempCourse);        }               tempStudent.setCourses(tempCourses);        session.save(tempStudent);               //commit a transaction        session.getTransaction().commit();        /\*Block 1: ends\*/        System.**_out_**.println("Done");    }**catch**(Exception exc){    exc.printStackTrace();    }    **finally** {    //closing the session, handles the connection leak issue    session.close();    factory.close();    }   }}**Other features**• In the next set of videos, we’ll add support for other features• **Lazy Loading** of students and courses• Cascading to handle cascading saves ... but NOT deletes• If we delete a course, DO NOT delete students• If we delete a student, DO NOT delete coursesDatabase CRUD Web App - Spring MVC and Hibernate Web Project[web-customer-tracker - A CRUD project based on Spring framework and Hibernate. - YouTube](https://www.youtube.com/watch?v=pL1llJVQmRw&ab_channel=DiptoPaul)**


# Project Overview and Demo


##### ****What is this project?**Full working Spring MVC and Hibernate application that connects to a database![](https://lh4.googleusercontent.com/eXCXFO9prOQz5fh8FJqCMUpxuqFYIDGpK8Be-Nn3Ck-ZrGXgh6PpCkZogIMXahnqve_EhlIGnQvbj2cAS1JwdystAILMAlWiuGWNneCdW9irpQsnPH75RATPqEsMofNgU4tviK7juS5LvXJcilMUJkg)**Customer Relationship Management - CRM**1. Set up Database Dev Environment
2. List Customers
3. Add a new Customer
4. Update a Customer
5. Delete a Customer![](https://lh5.googleusercontent.com/w_KHYl3MY81nM_RYj2XG2t6tZwJVony7J2JcidDIOQcWur4n6o8kjlNSaaA_R8c186wosUyWTZnkIpDs2KRp3SysS6ojv0-aCWiEx3dlTTfTiAjdtDuCPF96rarsqfJB8cotDzRQ56wYUN8p1p5tiK0)![](https://lh5.googleusercontent.com/RAbhYDbLFfRgv2gpxcmVVMzMwWkyykDPW8LSiksgELMVidr0KUw2h2a_cNAdSJVjhKgPArTsvUx42BpaBW0cn1Mus_iFe6XmYNZ001B6GtQCd8Vbeyek2331nc0OLLLlhRvEtPNw8zOQNTMXrpbUYcU)**


# Development Process - Step by Step


##### **1. Set up Database Dev Environment

   1. Setup Database Table

      1. Two Database Scripts (Folder: sql-scripts)

         1. 01-create-user.sql - Create a new MySQL user for our application

            1. user id: springstudent
            2. password: springstudent

         2. 02-customer-tracker.sql - Create a new database table: customer

            1. Create then Load table with sample data

      2. Test DB Connection

2. Setup Project IDE Dev Environment

3. List Customers

4. Add a new Customer

5. Update a Customer

6. Delete a Customer**


## Database Dev Environment Setup


### Setup (MYSQL PART) - [6 Set Up Dev Environment Part 1 - YouTube](https://www.youtube.com/watch?v=XVmNsMtVGa4&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=5&ab_channel=freeCodeCampBengali)


##### ****Create a new MySQL user for our application**File: 01-create-user.sqlCREATE USER 'springstudent'@'localhost' IDENTIFIED BY 'springstudent';GRANT ALL PRIVILEGES ON \* . \* TO 'springstudent'@'localhost';\#\# Starting with MySQL 8.0.4, the MySQL team changed the \# default authentication plugin for MySQL server \# from mysql_native_password to caching_sha2_password.\#\# The command below will make the appropriate updates for your user account.\#\# See the MySQL Reference Manual for details: \# https&#x3A;//dev.mysql.com/doc/refman/8.0/en/caching-sha2-pluggable-authentication.html\#ALTER USER 'springstudent'@'localhost' IDENTIFIED WITH mysql_native_password BY 'springstudent';**Create a new database table: customer**File: 02-customer-tracker.sqlCREATE DATABASE  IF NOT EXISTS \`web_customer_tracker\` /\*!40100 DEFAULT CHARACTER SET latin1 \*/;USE \`web_customer_tracker\`;\-- MySQL dump 10.13  Distrib 5.6.13, for osx10.6 (i386)\--\-- Host: 127.0.0.1    Database: web_customer_tracker\-- ------------------------------------------------------\-- Server version 5.6.16/\*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT \*/;/\*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS \*/;/\*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION \*/;/\*!40101 SET NAMES utf8 \*/;/\*!40103 SET @OLD_TIME_ZONE=@@TIME_ZONE \*/;/\*!40103 SET TIME_ZONE='+00:00' \*/;/\*!40014 SET @OLD_UNIQUE_CHECKS=@@UNIQUE_CHECKS, UNIQUE_CHECKS=0 \*/;/\*!40014 SET @OLD_FOREIGN_KEY_CHECKS=@@FOREIGN_KEY_CHECKS, FOREIGN_KEY_CHECKS=0 \*/;/\*!40101 SET @OLD_SQL_MODE=@@SQL_MODE, SQL_MODE='NO_AUTO_VALUE_ON_ZERO' \*/;/\*!40111 SET @OLD_SQL_NOTES=@@SQL_NOTES, SQL_NOTES=0 \*/;\--\-- Table structure for table \`customer\`\--DROP TABLE IF EXISTS \`customer\`;/\*!40101 SET @saved_cs_client     = @@character_set_client \*/;/\*!40101 SET character_set_client = utf8 \*/;CREATE TABLE \`customer\` (  \`id\` int(11) NOT NULL AUTO_INCREMENT,  \`first_name\` varchar(45) DEFAULT NULL,  \`last_name\` varchar(45) DEFAULT NULL,  \`email\` varchar(45) DEFAULT NULL,  PRIMARY KEY (\`id\`)) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=latin1;/\*!40101 SET character_set_client = @saved_cs_client \*/;\--\-- Dumping data for table \`customer\`\--LOCK TABLES \`customer\` WRITE;/\*!40000 ALTER TABLE \`customer\` DISABLE KEYS \*/;INSERT INTO \`customer\` VALUES (1,'Shariar','Shohag','shariar@gmail.com'),(2,'John','Doe','john@yahoo.com'),(3,'Ajay','Roy','ajay@hotmail.com'),(4,'Lionel','Messi','lm10@fcbarcelona.com'),(5,'Bill','Gates','bill@microsoft.com');/\*!40000 ALTER TABLE \`customer\` ENABLE KEYS \*/;UNLOCK TABLES;/\*!40103 SET TIME_ZONE=@OLD_TIME_ZONE \*/;/\*!40101 SET SQL_MODE=@OLD_SQL_MODE \*/;/\*!40014 SET FOREIGN_KEY_CHECKS=@OLD_FOREIGN_KEY_CHECKS \*/;/\*!40014 SET UNIQUE_CHECKS=@OLD_UNIQUE_CHECKS \*/;/\*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT \*/;/\*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS \*/;/\*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION \*/;/\*!40111 SET SQL_NOTES=@OLD_SQL_NOTES \*/;\-- Dump completed on 2016-09-24 21:50:59**FAQ: What does statements like /\*40101 - - -   - - -   - - - \*/  this do?**- [****mysql - What do the statements at the start of a MysqlDump do? - Stack Overflow****](https://stackoverflow.com/questions/15489456/what-do-the-statements-at-the-start-of-a-mysqldump-do)
- [****sql - MySQL syntax: What is this? - Stack Overflow****](https://stackoverflow.com/questions/6265891/mysql-syntax-what-is-this)
- [****mysql - When are we supposed to set default-character-set for the client? - Database Administrators Stack Exchange****](https://dba.stackexchange.com/questions/7841/when-are-we-supposed-to-set-default-character-set-for-the-client)
- Write your answer after reading them**


### Test Database Connection  -  [4 Test Database Connection Part 1 - YouTube](https://www.youtube.com/watch?v=sESBdjKIEn4&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=3&ab_channel=freeCodeCampBengali) \|


##### **[**5 Test Database Connection Part 2 - YouTube**](https://www.youtube.com/watch?v=TL85m71v7UU&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=4&ab_channel=freeCodeCampBengali)- Create new project file named “web-customer-tracker” as Dynamic web project
- Add **jdbc driver** to WEB-INF > lib directory
- To test the db, create a package named “com.diptopaul.testdb”
- Create a servlet inside the package named “TestDbServlet”, uncheck some methods that are created by default before finishing the file creation.File: TestDbServlet.java/\*\* \* Servlet implementation class TestDbServlet \*/@WebServlet("/TestDbServlet")public class TestDbServlet extends HttpServlet {private static final long serialVersionUID = 1L;/\*\* \* @see HttpServlet#doGet(HttpServletRequest request, HttpServletResponse response) \*/protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {// setup connection variablesString user = "springstudent";String pass = "springstudent";String jdbcUrl = "jdbc:mysql://localhost:3306/web_customer_tracker?useSSL=false&serverTimezone=UTC";String driver = "com.mysql.cj.jdbc.Driver";// get connection to databasetry {PrintWriter out = response.getWriter();out.println("Connecting to database: " + jdbcUrl);Class.forName(driver);Connection myConn = DriverManager.getConnection(jdbcUrl, user, pass);out.println("SUCCESS!!!");myConn.close();}catch (Exception exc) {exc.printStackTrace();throw new ServletException(exc);}}}**FAQ**1. What is the use of `Class.forName("...")`?

   1. Pre Java 6 the `DriverManager` class wouldn't have known which JDBC driver you wanted to use, since there are multiple drivers associated with JDBC. So, In previous versions of JDBC, to obtain a connection, you first had to initialize your JDBC driver by calling the method Class.forName. This method required an object of type java.sql.Driver. Each JDBC driver contains one or more classes that implements the interface java.sql.Driver. Thus when calling this method `forName `it automatically loaded the Driver. `Class.forName("...")` was a way of pre-loading the driver classes.Since JDBC 4.0 the DriverManager itself uses ServiceLoader to find drivers on the classpath. Any JDBC 4.0 drivers that are found in your class path are automatically loaded. (However, you must manually load any drivers prior to JDBC 4.0 with the method Class.forName.). In other words, it allows you to use the Driver class without having an explicit import for your class. This allows you to build the project without having to have the Oracle driver in your classpath.  [Establishing a Connection (The Java™ Tutorials > JDBC Database Access > JDBC Basics)](<https://docs.oracle.com/javase/tutorial/jdbc/basics/connecting.html#:~:text=In%20previous%20versions,Class.forName.)>)1. [java - What is the actual use of Class.forName("oracle.jdbc.driver.OracleDriver") while connecting to a database? - Stack Overflow](https://stackoverflow.com/questions/8053095/what-is-the-actual-use-of-class-fornameoracle-jdbc-driver-oracledriver-while)
2. <https://stackoverflow.com/a/21202612/7828981>2. No suitable driver found for jdbc mysql//localhost :3306

   1. Add `Class.forName("full qualified directory of driver class")`**


## Setup Project IDE Dev Environment


### Setup


#### **Setup Dev Environment -** [6 Set Up Dev Environment Part 1 - YouTube](https://www.youtube.com/watch?v=XVmNsMtVGa4&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=5&ab_channel=freeCodeCampBengali) [05-setup-dev-environment.pdf](https://drive.google.com/file/d/1P-gTYjhnIApX1u08FMmot7_y-v8H1532/view?usp=share_link)


##### **1. Already created a project file named “web-customer-tracker” while testing connection. Now do the following steps.

2. Copy starter config files and paste them to web-inf directory

   1. web.xml and spring config ()

3. Copy over JSTL libs and paste them to WEB-INF > lib

4. Copy latest Spring JAR files and paste them to WEB-INF > lib

5. Copy latest Hibernate JAR files and paste them to WEB-INF > lib

   1. Copy the files from Required
   2. Copy the files from the directory optional > c3po**File**: web.xml&lt;?xml version=_"1.0"_ encoding=_"UTF-8"_?>&lt;web-app xmlns:xsi=_"http&#x3A;//www.w3.org/2001/XMLSchema-instance"_ xmlns=_"http&#x3A;//xmlns.jcp.org/xml/ns/javaee"_ xsi:schemaLocation=_"http&#x3A;//xmlns.jcp.org/xml/ns/javaee http&#x3A;//xmlns.jcp.org/xml/ns/javaee/web-app_3_1.xsd"_ id=_"WebApp_ID"_ version=_"3.1"_>  &lt;display-name>spring-mvc-crud-demo&lt;/display-name>  &lt;absolute-ordering />  &lt;welcome-file-list>&lt;welcome-file>index.jsp&lt;/welcome-file>&lt;welcome-file>index.html&lt;/welcome-file>  &lt;/welcome-file-list>  &lt;servlet>&lt;servlet-name>dispatcher&lt;/servlet-name>&lt;servlet-class>org.springframework.web.servlet.DispatcherServlet&lt;/servlet-class>&lt;init-param>   &lt;param-name>contextConfigLocation&lt;/param-name> &lt;param-value>/WEB-INF/spring-mvc-crud-demo-servlet.xml&lt;/param-value>&lt;/init-param>&lt;load-on-startup>1&lt;/load-on-startup>  &lt;/servlet>  &lt;servlet-mapping>&lt;servlet-name>dispatcher&lt;/servlet-name>&lt;url-pattern>/&lt;/url-pattern>  &lt;/servlet-mapping>&lt;/web-app>What does  &lt;absolute-ordering /> do?- [java - What is the difference between Web Fragment Project and Dynamic Web Project? - Stack Overflow](https://stackoverflow.com/questions/25657315/what-is-the-difference-between-web-fragment-project-and-dynamic-web-project)
- [Web fragments - IBM Documentation](https://www.ibm.com/docs/en/was-nd/8.5.5?topic=applications-web-fragments)File: WEB-INF/spring-mvc-crud-demo-servlet.xml&lt;?xml version=_"1.0"_ encoding=_"UTF-8"_?>&lt;beans xmlns=_"http&#x3A;//www.springframework.org/schema/beans"_  xmlns:xsi=_"http&#x3A;//www.w3.org/2001/XMLSchema-instance"_  xmlns:context=_"http&#x3A;//www.springframework.org/schema/context"_xmlns:tx=_"http&#x3A;//www.springframework.org/schema/tx"_  xmlns:mvc=_"http&#x3A;//www.springframework.org/schema/mvc"_  xsi:schemaLocation=_"_        ___http&#x3A;//www.springframework.org/schema/beans_        ___http&#x3A;//www.springframework.org/schema/beans/spring-beans.xsd_        ___http&#x3A;//www.springframework.org/schema/context_        ___http&#x3A;//www.springframework.org/schema/context/spring-context.xsd_        ___http&#x3A;//www.springframework.org/schema/mvc_        ___http&#x3A;//www.springframework.org/schema/mvc/spring-mvc.xsd_        ___http&#x3A;//www.springframework.org/schema/tx_        ___http&#x3A;//www.springframework.org/schema/tx/spring-tx.xsd"_>   &lt;!-- Add support for component scanning -->  &lt;context:component-scan base-package=_"com.luv2code.springdemo"_ />   &lt;!-- Add support for conversion, formatting and validation support -->  &lt;mvc:annotation-driven/>   &lt;!-- Define Spring MVC view resolver -->  &lt;bean    class=_"org.springframework.web.servlet.view.InternalResourceViewResolver"_>        &lt;property name=_"prefix"_ value=_"/WEB-INF/view/"_ />        &lt;property name=_"suffix"_ value=_".jsp"_ />  &lt;/bean> &lt;!-- Step 1: Define Database DataSource / connection pool -->  &lt;bean id=_"myDataSource"_ class=_"com.mchange.v2.c3p0.ComboPooledDataSource"_       destroy-method=_"close"_>     &lt;property name=_"driverClass"_ value=_"com.mysql.cj.jdbc.Driver"_ />     &lt;property name=_"jdbcUrl"_ value=_"jdbc:mysql://localhost:3306/web_customer_tracker?useSSL=false&amp;amp;serverTimezone=UTC"_ />     &lt;property name=_"user"_ value=_"springstudent"_ />     &lt;property name=_"password"_ value=_"springstudent"_ />      &lt;!-- these are connection pool properties for C3P0 -->        &lt;property name=_"initialPoolSize"_ value=_"5"_/>     &lt;property name=_"minPoolSize"_ value=_"5"_ />     &lt;property name=_"maxPoolSize"_ value=_"20"_ />     &lt;property name=_"maxIdleTime"_ value=_"30000"_ />  &lt;/bean>  &lt;!-- Step 2: Setup Hibernate session factory -->  &lt;bean id=_"sessionFactory"_        class=_"org.springframework.orm.hibernate5.LocalSessionFactoryBean"_>        &lt;property name=_"dataSource"_ ref=_"myDataSource"_ />        &lt;property name=_"packagesToScan"_ value=_"com.luv2code.springdemo.entity"_ />        &lt;property name=_"hibernateProperties"_>           &lt;props>              &lt;prop key=_"hibernate.dialect"_>org.hibernate.dialect.MySQLDialect&lt;/prop>              &lt;prop key=_"hibernate.show_sql"_>true&lt;/prop>           &lt;/props>        &lt;/property>   &lt;/bean>   &lt;!-- Step 3: Setup Hibernate transaction manager -->  &lt;bean id=_"myTransactionManager"_         class=_"org.springframework.orm.hibernate5.HibernateTransactionManager"_>     &lt;property name=_"sessionFactory"_ ref=_"sessionFactory"_/>&lt;/bean>&lt;!-- Step 4: Enable configuration of transactional behavior based on annotations -->  &lt;tx:annotation-driven transaction-manager=_"myTransactionManager"_ />   &lt;!-- Add support for reading web resources: css, images, js, etc ... -->  &lt;mvc:resources location=_"/resources/"_ mapping=_"/resources/\*\*"_>&lt;/mvc:resources> &lt;/beans>- Tag [&lt;/props>](https://www.java4coding.com/contents/spring/spring-property-tag)
-  **


#### **Configuration for Spring + Hibernate (Step by Step) -** [8 Set Up Dev Environment Part 2 - YouTube](https://www.youtube.com/watch?v=gWnyA_ipQVc&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=6&ab_channel=freeCodeCampBengali) \| [9 Set Up Dev Environment Part 3 - YouTube](https://www.youtube.com/watch?v=0xKIbgrJNfQ&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=7&ab_channel=freeCodeCampBengali) [04-setup-dev-environment-part-2.pdf](https://drive.google.com/file/d/1Is--qisrrAmGqsho9sFqprSA3O6P39_k/view?usp=share_link)


##### **1. Define database dataSource / connection pool
2. Setup Hibernate session factory
3. Setup Hibernate transaction manager
4. Enable configuration of transactional annotations**Placement of Configurations**Add the following configurations in your Spring MVC configuration fileFor our example: spring-mvc-crud-demo-servlet.xml**Step 1**: Define database dataSource / connection pool&lt;bean id="myDataSource" class="com.mchange.v2.c3p0.ComboPooledDataSource"destroy-method=“close">&lt;property name="driverClass" value="com.mysql.jdbc.Driver" />&lt;property name="jdbcUrl"value="jdbc:mysql://localhost:3306/web_customer_tracker?useSSL=false" />&lt;property name="user" value="springstudent" />&lt;property name="password" value="springstudent" />&lt;!-- these are connection pool properties for C3P0 -->&lt;property name="minPoolSize" value="5" />&lt;property name="maxPoolSize" value="20" />&lt;property name="maxIdleTime" value="30000" />&lt;/bean>**Step 2**: Setup Hibernate session factory&lt;bean id="sessionFactory"class=“org.springframework.orm.hibernate5.LocalSessionFactoryBean">&lt;property name="dataSource" ref="myDataSource" />&lt;property name="packagesToScan" value="com.luv2code.springdemo.entity" />&lt;property name="hibernateProperties">&lt;props>&lt;prop key="hibernate.dialect">org.hibernate.dialect.MySQLDialect&lt;/prop>&lt;prop key="hibernate.show_sql">true&lt;/prop>&lt;/props>&lt;/property>&lt;/bean>**Step 3**: Setup Hibernate transaction manager&lt;bean id="myTransactionManager"class=“org.springframework.orm.hibernate5.HibernateTransactionManager">&lt;property name="sessionFactory" ref="sessionFactory"/>&lt;/bean>**Step 4:** Enable configuration of transactional annotations&lt;tx:annotation-driven transaction-manager="myTransactionManager" />**Full xml Configuration code****


### Test Basic Spring MVC Controller [10 Test Spring MVC Controller Part 1 - YouTube](https://www.youtube.com/watch?v=PHODaACNOss&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=8&ab_channel=freeCodeCampBengali) \| [11 Test Spring MVC Controller Part 2 - YouTube](https://www.youtube.com/watch?v=l6YzfnhZCaY&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=9&ab_channel=freeCodeCampBengali)


##### **![](https://lh5.googleusercontent.com/kg5YjTZSBzyU62wx-SnUcC0RcP8S6AIFWxQtRVJWGTKrwToPoDAJ1vrHmCX-hKPbJWVddFpSMiufPW5DbdVU-g3a793lafVU_tBVu_uMKs6RG23cKcQ0uK6Io8zisAKQK4kzmtuE8ADNtkTPwGZ3fPA)**File**: _CustomerController.java_package com.luv2code.springdemo.controller;import org.springframework.stereotype.Controller;import org.springframework.ui. Model;import org.springframework.web.bind.annotation. Request Mapping;@Controller@RequestMapping("/customer")public class Customer Controller {@RequestMapping("/list")public String listCustomers (Model theModel) {return "list-customers";}}**File**: _WEB-INF > view > list-customers.jsp_&lt;!DOCTYPE html>&lt;html>&lt;head>&lt;title>List Customers&lt;/title>&lt;/head>&lt;body>List Customers - coming soon&lt;/body>&lt;/html>Finally, Run on server then browse <http://localhost:8080/web-customer-tracker/customer/list>**


## Project Development


### Sample App Architecture - [07-mvc_app_architecture.pdf](https://drive.google.com/file/d/18NokO5DZ8QWd8lDYRaQWyM8k4JdKK5lP/view?usp=sharing) [1 List Customers Overview - YouTube](https://www.youtube.com/watch?v=s582J6OKr_s&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=10&ab_channel=freeCodeCampBengali)


##### **Sample App Features - Refresher- List Customers, show a list
- Add a new Customer
- Update a Customer
- Delete a Customer![](https://lh6.googleusercontent.com/e6NTeQPPgLfc-UXuLtBFr8UXBdkW4cKfrXdzwceaK7fO42cWaPhaBP2UkLXJCCh9lq61_18BDQy3jlods8mvZtey4fNtNDfm3GDnOfCcqtkWJ7-pzHC8i_Wis-hQdqjR262y-D-oGlXUyB0WYhF8dRw)**


#### Customer Data Access Object


##### **✤ Responsible for interfacing with the database✤ This is a common design pattern: Data Access Object (DAO)![](https://lh3.googleusercontent.com/5x9pPZ7t4t82WwI_5hxoXLbAE7WyUrq0EnsZK5nBNn9Kmk9n8vg-XrrzUkNrGqX779jzLxg5vCkQwnYT6Q9SLxXSTnQRqUskJ44fjV5djOtGUioI6V3dPsk25NUwGKcoI1v4y6Tp2Ls2jJR2lWQtlXA)**Customer DAO Methods**- saveCustomer(...)
- getCustomer(...)
- getCustomers()
- updateCustomer(...)
- deleteCustomer(...)[08-overview-of-development-process.pdf](https://drive.google.com/file/d/1ovTB2ahKp0QYnieEasBo4Tsdmb638neV/view?usp=sharing)\| [2 List Customers Overview of Development Process - YouTube](https://www.youtube.com/watch?v=SZIMU6oWXIw&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=11&ab_channel=freeCodeCampBengali)**


### List Customers - Dev Process


##### **1. Create Customer.java

2. Create CustomerDAO.java

   1. CustomerDAOImpl.java

3. Create CustomerController.java

4. Create JSP page: list-customers.jsp![](https://lh4.googleusercontent.com/8l663ZEVgH9bzb8vhPjmD_jZb4Bw6f0Or3NylIq5KmhU5oKqFOydxkhaSKbHBhrEG94omPL6kgA6OVJjLk8w4ZM4SY5WRd7ozB7VFDizsPydvBeykRAknNFOPdgBRVBdhiJShqNG97VBXus4HC7IecM)**


#### Create Customer Entity


##### **[09-create-customer-entity.pdf](https://drive.google.com/file/d/1brJFE7yTpyiW7I_aQZVHOab_HEAFSye-/view?usp=sharing)\| [3 List Customers Creating Hibernate Entity Part 1 - YouTube](https://www.youtube.com/watch?v=KsGtKT98nY8&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=11&ab_channel=freeCodeCampBengali) Entity Class: Java class that is mapped to a database table![](https://lh4.googleusercontent.com/uHAfe6NdGz7QEt9TECNrp6Dsvq9JxkxTXOx1dCW2DkSXT01MZ-JG3Xc24rMPnynDKxNoFFoaE-3sWoBsa2n5q5z5yuzjdN6CPdBORWWjelcxiLfDAqVJW4ulzL90jHK2ptrjgbxsh667DNVOCeR0Md4)Step 1: Map class to database table![](https://lh6.googleusercontent.com/TuEKhNiWdyDa-nSuTDTMP4sbyr4lpG9GQPqNsze253Drq7RR4gkUOZr5psBvuztK57aSVPJ3Bwu_E8InbExLhB37wRB5K6P3bnWLeQGJaFrj4FXArD3Oepe6zUNi9VuwQJwdEd8A0z3QQLhiHaA0HwA)Step 2: Map fields to database columns![](https://lh3.googleusercontent.com/G4snpv5_F6MQuLLprvOufS8dx1b1ioTHYbJ7Wjj8-6L-nOiIaZ8mEMBdPPpQmMarXBxNji7D9HrTwgw3OGSa5oYpOsYJMJPQ6u1xyjh2CCNyy-xK7AKx5tzicEBqqDepf9b4vK_l2IakNXfVdTQWJ2E)Add Entity Scanning- Remember our Spring MVC config file?&lt;bean id="sessionFactory"class=“org.springframework.orm.hibernate5.LocalSessionFactoryBean">&lt;property name="dataSource" ref="myDataSource" />&lt;property name="packagesToScan" value="com.luv2code.springdemo.entity" />...&lt;/bean>**Customer Entity Class**@Entity@Table(name="customer")**public** **class** Customer {   @Id  @GeneratedValue(strategy=GenerationType.**_IDENTITY_**)  @Column(name="id")  **private** **int** id;   @Column(name="first_name")  **private** String firstName;   @Column(name="last_name")  **private** String lastName;   @Column(name="email")  **private** String email;  //constructors   // getter and setter   //additional methods}**


#### DAO Layer - Define and Create Data Access Object


##### **[10-define_dao_with_repository_annotation_overview.pdf](https://drive.google.com/file/d/1ZgjZWSC8c5_jtmLDTP4w49A-1k91afSL/view?usp=share_link)![](https://lh6.googleusercontent.com/e6NTeQPPgLfc-UXuLtBFr8UXBdkW4cKfrXdzwceaK7fO42cWaPhaBP2UkLXJCCh9lq61_18BDQy3jlods8mvZtey4fNtNDfm3GDnOfCcqtkWJ7-pzHC8i_Wis-hQdqjR262y-D-oGlXUyB0WYhF8dRw)**Customer Data Access Object(DAO)**✤ For Hibernate, our DAO needs a **Hibernate SessionFactory**![](https://lh5.googleusercontent.com/kI6rex_JIHHS5x_ljt9zJ4gKfUAvqG-k-xizO9kyL67GBwVeFc1HWlavynGyFMshNIAvh2BXKphgLQBSSwg6CvUlmOQ4HkpslwDKTWzq7xcDbhuK6RmjXvB0BUIaOSAl5_7xiTA0k1MJxhU9Fb6ei3M)**Hibernate SessionFactory**✤ Our **Hibernate Session Factory** needs a **Data Source**✤ The data source defines database connection info![](https://lh5.googleusercontent.com/oPDXzLTvNHF3DGZzxKZo7zSEKJDn5jrhcJ7tR9bzLsvAazdRLNtTv_2C-5S9LpUaHFGS-TZdLmNiz-s38X_QPLvZfT65MflbQFQFohKN2mpShRFkWtHNq-yMDusW4f0KvMRQZ8mMKZ8bATBfTf7JWZU)These are all **dependencies**! We will **wire** them together **with Dependency Injection (DI**). First we need to define **Data Source** as a bean, then define **SessionFactory** as a bean. Once these two beans are defined for the use of autowiring in the project’s main source codes, we can define DAO’s for the development and use these dependencies.1. **Data Source**&lt;bean id="myDataSource" class="com.mchange.v2.c3p0.ComboPooledDataSource"destroy-method=“close">&lt;property name="driverClass" value="com.mysql.jdbc.Driver" />&lt;property name="jdbcUrl"value="jdbc:mysql://localhost:3306/web_customer_tracker?useSSL=false" />... user id, password etc ...&lt;/bean>![](https://lh5.googleusercontent.com/oPDXzLTvNHF3DGZzxKZo7zSEKJDn5jrhcJ7tR9bzLsvAazdRLNtTv_2C-5S9LpUaHFGS-TZdLmNiz-s38X_QPLvZfT65MflbQFQFohKN2mpShRFkWtHNq-yMDusW4f0KvMRQZ8mMKZ8bATBfTf7JWZU)2. **Session Factory**&lt;bean id="sessionFactory"class=“org.springframework.orm.hibernate5.LocalSessionFactoryBean">&lt;property name="dataSource" ref="myDataSource" />...&lt;/bean>![](https://lh5.googleusercontent.com/oPDXzLTvNHF3DGZzxKZo7zSEKJDn5jrhcJ7tR9bzLsvAazdRLNtTv_2C-5S9LpUaHFGS-TZdLmNiz-s38X_QPLvZfT65MflbQFQFohKN2mpShRFkWtHNq-yMDusW4f0KvMRQZ8mMKZ8bATBfTf7JWZU)**Create Customer DAO (step by step)**1. Define DAO interface

2. Define DAO implementation

   1. Inject the session factory**Step 1: Define DAO interface** [**7 List Customers Developing Hibernate DAO Write Some Code Part 1 - YouTube**](https://www.youtube.com/watch?v=OUAeBV6jjas&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=17&ab_channel=freeCodeCampBengali)public interface CustomerDAO {public List&lt;Customer> getCustomers();}**Step 2: Define DAO implementation** [**8 List Customers Developing Hibernate DAO Write Some Code Part 2 - YouTube**](https://www.youtube.com/watch?v=wvxsPBmWAEo&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=17&ab_channel=freeCodeCampBengali)public class CustomerDAOImpl implements CustomerDAO {@Autowiredprivate SessionFactory sessionFactory;public List&lt;Customer> getCustomers() {...}}We can further update this with the use of Annotations.**


##### Spring @Transactional


##### **- Spring provides an @Transactional annotation which wraps the next block of code with begin and ending of a transaction.
- Automagically begin and end a transaction for your Hibernate code
- No need for you to explicitly do this in your code
- This Spring magic happens behind the scenes**Flash back - Equivalent Standalone Hibernate code( Alternative )**// start a transactionsession.beginTransaction();// DO YOUR HIBERNATE STUFF HERE// ...// commit transactionsession.getTransaction().commit();**Spring @Transactional Magic****Step 2 (Update 1): Define DAO implementation**public class CustomerDAOImpl implements CustomerDAO {@Autowiredprivate SessionFactory sessionFactory;@Transactional // Bad Practice to put this annotation here, better to move it to Service layer, we will do it laterpublic List&lt;Customer> getCustomers() {// get the current hibernate sessionSession currentSession = sessionFactory.getCurrentSession();// create a queryQuery&lt;Customer> theQuery =currentSession.createQuery("from Customer", Customer.class);// get the result listList&lt;Customer> customers = theQuery.getResultList();return customers;}}**Note**: This code will be updated when the service layer will be added.**Query:** How does @Transactional work?- [java - How does @Transactional influence current session in Hibernate? - Stack Overflow](https://stackoverflow.com/questions/24710620/how-does-transactional-influence-current-session-in-hibernate)
- <https://stackoverflow.com/a/10680753/7828981>
- [Some clarification about Spring @Transactional annotation on a method and why we should use it on service layer and not use it on DAO layer.](https://stackoverflow.com/questions/15300483/some-clarification-about-spring-transactional-annotation-on-a-method#:~:text=First%20of%20all,for%20more%20information.)
-**Specialized Annotation for DAOs**- Spring provides the @Repository annotation**


##### @Repository annotation


##### **- Applied to DAO implementations
- Spring will automatically register the DAO implementation
- thanks to component-scanning
- Spring also provides translation of any JDBC related exceptions**@Repository annotations magic****Step 2 (Update 2): Define DAO implementation**@Repository**public** **class** CustomerDAOImpl **implements** CustomerDAO{   @Autowired  **private** SessionFactory sessionFactory;   @Transactional // Bad Practice to put this annotation here, better to move it to Service layer, we will do it later  @Override  **public** List&lt;Customer> getCustomers() {        // **TODO** Auto-generated method stub        Session currentSession = sessionFactory.getCurrentSession();        List&lt;Customer> customers = currentSession.createQuery("from Customer", Customer.**class**).getResultList();               **return** customers;  } }**Note**: This code will be updated when the service layer will be added.**


#### Create CustomerController


##### ** [11-inject-repository-into-controller.pdf](https://drive.google.com/file/d/1ihkS64_ipk6Jka7LHZKtucrvo2XFUv4k/view?usp=share_link)\| [9 List Customers Injecting DAO into Controller - YouTube](https://www.youtube.com/watch?v=7FsapSUy71U&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=18&ab_channel=freeCodeCampBengali)**File**: **com.dpauld.springdemo.controller/CustomerController.java**public class CustomerController {@AutowiredCustomerDAO customerDAO; // Bad Practice to access DAO layer from controller, better to move it to Service layer and access the service layer object, we will do it later@RequestMapping("/list")public String listCustomers (Model theModel) {//get the customers from daoList&lt;Customer> theCustomers = customerDAO.getCustomers();//add customer to the modeltheModel.addAttribute("customers", theCustomers);return "list-customers";}}**Note**: This code will be updated when the service layer will be added.**


#### Create JSP page: list-customers.jsp 


##### JSP


##### **[12-create-the-jsp-view.pdf](https://drive.google.com/file/d/15kiDdZJw32Xvg4X_SpJTmaCbZfWpXt2_/view?usp=share_link) [10 List Customers Developing JSP View Page - YouTube](https://www.youtube.com/watch?v=SdiBeJkBlnA&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=19&ab_channel=freeCodeCampBengali) \|**File**: **web-inf/view/list-customers.jsp**&lt;%@ taglib uri = _"http&#x3A;//java.sun.com/jsp/jstl/core"_ prefix = _"c"_ %>&lt;!DOCTYPE html>&lt;html>&lt;head>&lt;meta charset=_"ISO-8859-1"_>&lt;title>List Customers&lt;/title>&lt;/head>&lt;body>&lt;!--List Customers - coming soon-->&lt;div class=_"wrapper"_>  &lt;div class=_"header"_>        &lt;h2>CRM - Customer Relationship Manager&lt;/h2>  &lt;/div>&lt;/div>&lt;div class=_"container"_>  &lt;div class=_"content"_>        &lt;table>             &lt;tr>                  &lt;th>First Name&lt;/th>                  &lt;th>Last Name&lt;/th>                  &lt;th>Email&lt;/th>             &lt;/tr>             &lt;!-- added taglib directive to enable jstl tags support -->             &lt;c:forEach var=_"tempCustomer"_ items=_"_${customers}_"_>                  &lt;tr>                        &lt;td>${tempCustomer.firstName}&lt;/td>                        &lt;td>${tempCustomer.lastName}&lt;/td>                        &lt;td>${tempCustomer.email}&lt;/td>                  &lt;/tr>             &lt;/c:forEach>        &lt;/table>  &lt;/div> &lt;/div>&lt;/body>&lt;/html>**


##### CSS


##### ** [13-making-it-pretty-with-css.pdf](https://drive.google.com/file/d/1PcKRZaAgViPb2WFDpFFgxOkeDFek9ruy/view?usp=share_link) [11 Making it Pretty with CSS Overview - YouTube](https://www.youtube.com/watch?v=Hm0n1pwCqj4&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=20&ab_channel=freeCodeCampBengali) \| [12 Making it Pretty with CSS Write Some Code Part 1 - YouTube](https://www.youtube.com/watch?v=T_aqJip49TY&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=21&ab_channel=freeCodeCampBengali) \| [13 Making it Pretty with CSS Write Some Code Part 2 - YouTube](https://www.youtube.com/watch?v=sz9QjXQ02BU&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=22&ab_channel=freeCodeCampBengali)First Version![](https://lh5.googleusercontent.com/hgVT_Co-4g7wdGG-jZxQNxmLgW8YRfJr3QggLT3qnN0kNcnow1k3yEGIjW6UoVx9dbhVeVk51Ljmr1kSQuBnhmz7A4ZJDlHl_LtEAN-dwRhtFp3IpDwZI8wuFy2uHoi8lXqmgBbOn2VO6ArjZTDa_lE)Second Version: Making it pretty with CSS ![](https://lh5.googleusercontent.com/3qZvKLVDRW8pvnBBFJgvuO8qk8B_sN_4Uq9fbY0QXihv6dbaa_D7aICDaE7O3DWCi1zzNZj57yoD8YCpyKvvl0OdKsi9RRD7IrYvBxO4jYngkJlWvkMLZAvsqoQSi8itH_hvqvVXbmvnHPYH7OtSofs)Development Process1. Place CSS in a ‘resources’ directory
2. Configure Spring to serve up ‘resources’ directory
3. Reference CSS in your JSP**Step 1**: Place CSS in ‘resources’ directory![](https://lh5.googleusercontent.com/nJY_xu3NbkU-c8wsjjOB07HJ0l9JIZC63FKqpEKSsT3bw6fkB_PcrYzGwFZXruaa0O4mWSBZLll7f8_mFFvol0uWztMgCsTHlv9q0SQTbd8ZILFibUOzyWiAsrQzbFz8gtY3BkYh0dABIvgP1GU6yu4)or![](https://lh5.googleusercontent.com/veVBCWR1-FazsWjT28IiY7GFaTXiJz9CPitpXYr8YmZ6p3Vv4FCIzHIubvquhKTpGt8qAYZhOKcbiMeRloetZCTNiSqEoaQUTTN62-tyLlq1Wg87vm40a8fG_tRn3IPLNHUw1Zf5ib0cni9ZI9spWM0)**Step 2:** Configure Spring to serve up ‘resources’ directory**File:** spring-mvc-crud-demo-servlet.xml&lt;mvc:resources location=_"/resources/"_ mapping=_"/resources/\*\*"_>&lt;/mvc:resources>The **mvc:resources** element is used to point the location of resources with a specific public URL pattern.For example, the following line will serve all requests for resources coming in with a public URL pattern, like “/resources/\*\*”, by searching in the “/resources/” directory under the root folder in our application:&lt;mvc:resources mapping="/resources/\*\*" location="/resources/" />The **location** attribute of the **mvc:resources** tag defines the base directory location of static resources that you want to serve. The **Mapping** attribute, just indicates the incoming requested path that needs to be mapped to this resources directory.**Step 3**: Reference CSS in your JSP&lt;head>&lt;title>List Customers&lt;/title>&lt;link type=_"text/css"_rel=_"stylesheet"_href=_"_${pageContext.request.contextPath}_/resources/css/style.css"_>&lt;/head>pageContext is a variable implicitly available to the jsp pages. pageContext.request.contextPath returns the directory of project name. In this case returns /web-customer-tracker**Applies for JavaScript, images, pdfs etc…**![](https://lh4.googleusercontent.com/v2W2rYUbw7CgzK9Hi38BuQgi7GSgRkS2t9ADePvsmfvhHTMuOZv-AJHMYG92QiTppHNDj9OFDIr7BLvaVafKqZuixo8TtXdHQGlLpvfi7KhiuWTA34UuzhxMHjuSZzWmA2PpJD1O5-x-fbHIfzBuNr4)**Alternate Directory Structure**![](https://lh3.googleusercontent.com/8Al04yUuukcCk9dT_IvEu97g5b0kQdl04Wu6_BgANjGY9GaZmCqbo5lY8nXSWzJppqdVjX2_j7hWONLa1UGLH9gcRl-L8jnvlVpW8TPDYAE9bEFNfK_qds9tkQStMBt0u7MVDgYUTxvDKyh-Yt7L7IQ)**Configure Spring for Alternate Directory Structure to serve up ‘resources’ directory** **File**: _spring-mvc-crud-demo-servlet.xml_&lt;mvc:resources location=_“/resources_/" mapping=_"/resources/\*\*"_ />&lt;mvc:resources location=_“/images_/" mapping=_"/images/\*\*"_ />&lt;mvc:resources location=_“/js_/" mapping=_"/js/\*\*"_ />&lt;mvc:resources location=_“/pdf_/" mapping=_"/pdf/\*\*"_ />FAQ:1. javax.servlet.jsp.PageContext cannot be resolved to a type

   1. Make sure to Add **servlet-api** dependency and jsp-api dependency, this might solve the issue.

   2. **Alternative** approach

      1. Right click on project and go to properties
      2. Click over Targeted Runtimes
      3.  Check the mark server you are using. For example, "Apache Tomcat v8.0"

   3. Read details about [PageContext](https://agiletribe.purplehillsbooks.com/2016/02/23/httpservletrequest-path-decoding/)

      1. **getContextPath**()
      2. **getPathInfo**()
      3. **getPathTranslated**()
      4. **getQueryString**()
      5. **getRequestURI**()
      6. **getRequestURL**()
      7. **getServletPath**()
      8. Note: the request.getContextPath() is only available from Servlet 2.5 spec.![](https://lh6.googleusercontent.com/404M2XLvI4lQnvzZ-U-f8PCs7DwZT-LObl-xLL5_6tDgJmeMH_cZDDK-TqEdK0Nvym6ddB4roDn86rd2F2v7g1tTxeg00Lz6wNC3lMoQZqa5fxEa_RsfmYIMk-mQx2hLCJkv5zhZtwJoFccQ4qphOQc)**Query**:1. [java - What does this expression language ${pageContext.request.contextPath} exactly do in JSP EL? - Stack Overflow](https://stackoverflow.com/questions/5850336/what-does-this-expression-language-pagecontext-request-contextpath-exactly-do#:~:text=The%20pageContext%20is,on%20your%20part.)
2. [Spring 3 MVC resources and tag &lt;mvc:resources /> - Stack Overflow](https://stackoverflow.com/questions/8195213/spring-3-mvc-resources-and-tag-mvcresources#:~:text=As%20said%20by%20%40Nancom,resources/pdf/index.pdf)* * *A Stack Overflow answer, note: mapping value is **resource** not **resources,** so don't get confused.As said by @Nancom&lt;mvc:resources location="/resources/" mapping="/resource/\*\*"/>So for clarity lets our image is inresources/images/logo.png"The **location** attribute of the **mvc:resources** tag defines the base directory location of static resources that you want to serve. It can be images paths that are available under the `src/main/webapp/resources/images/` directory; you may wonder why we have given only **/resources/** as the location value instead of `src/main/webapp/resources/images/`. This is because we consider the `resources` directory as the base directory for all resources, we can have multiple sub-directories under the resources directory to put our images and other static resource files.The second attribute, **mapping**, just indicates the request path that needs to be mapped to this `resources` directory. In our case, we have assigned `/resource/**` as the mapping value. So, if any web **request starts** with the `/resource` request path, then it will be mapped to the `resources` directory, and the `/**` symbol indicates the recursive look for any resource files underneath the base `resources` directory.So for urls like `http://localhost:8080/webstore/resource/images/logo.png`. So, while serving this web request, Spring MVC will consider `/resource/images/logo.png` as the request path. So, it will try to map `/resource` to the base directory specified by the **location** attribute, `resources`. From this directory, it will try to look for the remaining path of the URL, which is `/images/logo.png`. Since we have the `images` directory under the `resources` directory, Spring can easily locate the image file from the `images` directory.So&lt;mvc:resources location="/resources/" mapping="/resource/\*\*"/>gives us for given \[requests] -> \[resource mapping]:`http://localhost:8080/webstore/resource/images/logo.png` -> searches in `resources/images/logo.png``http://localhost:8080/webstore/resource/images/small/picture.png` -> searches in `resources/images/small/picture.png``http://localhost:8080/webstore/resource/css/main.css` -> searches in `resources/css/main.css``http://localhost:8080/webstore/resource/pdf/index.pdf` -> searches in `resources/pdf/index.pdf`* * *3. Dad**


##### Final Codes


##### **File: **


#### Welcome file


##### **[14-adding-a-welcome-file.pdf](https://drive.google.com/file/d/12h_Wi1hk7Ir0X0WvwOtiD2PXhWN5rUKQ/view?usp=share_link) [14 Adding a Welcome File - YouTube](https://www.youtube.com/watch?v=gIQm8-z4mMY&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=24&ab_channel=freeCodeCampBengali)**Welcome File**<http://localhost:8080/web-customer-tracker>1. Server will look for a welcome file
2. If it doesn’t find one, then you’ll get a 404 :-(![](https://lh4.googleusercontent.com/EHcufcVe9lokWulEbJWEjlhG_h3y_9MMcPhtDo3xtxnrRNiPbt3iVY27tS_4lWQstAk3SMdOYL3wg4liek4Ht72bHI9mL8vhZn6iUBYPG_CVOrOwuhr9QvscrSEvdaMlfd0EZHKBYmO4AFJprz0-M18)3. Welcome files are configured in **web.xml**

   1. By adding a **jsp** or **html** file inside &lt;welcome-file-list> tag.**File**: _web.xml_    &lt;welcome-file-list>&lt;welcome-file>index.jsp&lt;/welcome-file>&lt;welcome-file>index.html&lt;/welcome-file>  &lt;/welcome-file-list>Look for these files **index.jsp** and **index.html** from top down approachLet's have it simple for now**File**:  **webapp/index.jsp**&lt;% response.sendRedirect("customer/list"); %>**


#### Refactor @GetMapping and @PostMapping 


##### **[15-GetMapping-and-PostMapping.pdf](https://drive.google.com/file/d/11gho1gW3zzBlZoBeWBtquSxEl9bQnTlo/view?usp=share_link) [1 Refactor @GetMapping and @PostMapping Overview - YouTube](https://www.youtube.com/watch?v=ZnBx7CXnVxw&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=24&ab_channel=freeCodeCampBengali) [2 Refactor @GetMapping and @PostMapping Write Some Code - YouTube](https://www.youtube.com/watch?v=2UqYKX6j7Zo&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=25&ab_channel=freeCodeCampBengali) HTTP Request / Response![](https://lh4.googleusercontent.com/filWZMoR0p0PmjWmCwhiQ8hjltZslL0S7D0HkgrySrinPyqWbOG5hNeqi5xAT5V9Bv1zAkr7wAzFb6pGWNDhO22WnZW9C-nVCd7uzIWiQVBGPQ_dg-9queq3s8eZrf9mEgTmW8wf2HVWizpqAhds6U4)**Most Commonly Used HTTP Methods**|            |                                   |
| :--------: | :-------------------------------: |
|   Method   |            Description            |
|     GET    | Requests data from given resource |
|    POST    |   Submits data to given resource  |
| others ... |                                   |**Refresher of Spring MVC JSP form Demo**&lt;form:form modelAttribute=_"customer1"_ action=_"processForm"_>  Fill out the form.  &lt;br> &lt;br>        First name: &lt;form:input path=_"firstName"_>&lt;/form:input>        &lt;br> &lt;br>        Last Name: &lt;form:input path=_"lastName"_>&lt;/form:input>        &lt;form:errors path=_"lastName"_ cssClass=_"error"_>&lt;/form:errors>        &lt;br> &lt;br>              Free passes: &lt;form:input path=_"freePasses"_>&lt;/form:input>       &lt;form:errors path=_"freePasses"_ cssClass=_"error"_>&lt;/form:errors>       &lt;br> &lt;br>   &lt;input type=_"submit"_ value=_"submit"_>&lt;/input> &lt;/form:form>Previously in Spring MVC we did not use any method types. Now we will deal with the **post method** and the **get method**.**


##### GET method


##### ****Sending Data with GET method**,&lt;form action="processForm" method="GET" ...>...&lt;/form>- Form data is added to end of URL as name/value pairstheUrl?field1=value1&field2=value2…**Refresher of Spring MVC Controller Demo**@RequestMapping("/processForm")**public** String processForm(@Valid @ModelAttribute("customer1") Customer customer, BindingResult theBindingResult) {  System.**_out_**.println("Binding Results:\\n" + theBindingResult);  **if**(theBindingResult.hasErrors()) {        //System.out.println(customer.getFreePasses());        **return** "customer-form";  }  **return** "customer-confirmation";}Previously in Spring MVC we used RequestMapping to handle **ALL HTTP methods**. Now we want to put constraints on controller mapping so that we can have Specific controller to serve specific types of request methods. **Constrain the Request Mapping - GET and Post**@RequestMapping(path="/processForm", method=RequestMethod.GET)**public** String processForm(...) {...}- This mapping ONLY handles GET method
- Any other HTTP REQUEST method will get rejected**


##### POST method


##### ****Sending Data with POST method**&lt;form action="processForm" method="POST" ...>...&lt;/form>- Form data is passed in the body of HTTP request message![](https://lh6.googleusercontent.com/K6NrsDNxet7bvQ08b0fKPsG-342e7rivRvUMuTV8OUYKTW_e5YvuNLH8Yew4amvrfFgmsOKufP0HRCqnP2ZggaYNu5wGE-HRjcI_RSua8jH6WOywKUIrkSJgcxLMtGK03j8g-G1yZHcM0rMgXMU9JIM)**Short-Cut:** We can also use two special annotations to handle them specifically **@GetMapping** for mapping get request and **@PostMapping** for mapping post request. _\[Added in Spring 4.3]_New Annotations- @GetMapping
- @PostMapping@GetMapping("/processForm")**public** String processForm(...) {...}New annotation: @GetMapping- This mapping ONLY handles GET method
- Any other HTTP REQUEST method will get rejectedTo Handle Post method, we use two approaches similar to the Get method handling.@PostMapping("/submitForm")**public** String submitForm(...) {...}New annotation: @PostMapping- @RequestMapping(path="/processForm", method=RequestMethod.POST)
- Short-cut: @PostMapping("/processForm")**Updated Full Code:**@Controller@RequestMapping("/customer")**public** **class** CustomerController {   @Autowired  CustomerDAO customerDAO;   //@RequestMapping("/list")  @GetMapping("/list") // Refactored, try PostMapping(), you will get an error  **public** String listCustomers (Model theModel) {               //get the customers from dao        List&lt;Customer> theCustomers = customerDAO.getCustomers();               //add customer to the model        theModel.addAttribute("customers", theCustomers);               System.**_out_**.println(theCustomers);               **return** "list-customers";  }}**


##### **Which One between GET and POST?**


##### ****GET**- Good for debugging
- Bookmark or email URL
- Limitations on data length**Post**- Can’t bookmark or email URL
- No limitations on data length
- Can also send binary data**


#### Refactor a Service layer


##### **[16-services-overview.pdf](https://drive.google.com/file/d/1gGepfZ04dMi2Ku_vL7ysQsWc_qVONqyP/view?usp=share_link)[3 Refactor Add a Service Layer Overview - YouTube](https://www.youtube.com/watch?v=gCuC_1kQRmk&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=26&ab_channel=freeCodeCampBengali) [4 Refactor Add a Service Layer Write Some Code Part 1 - YouTube](https://www.youtube.com/watch?v=GpnTu-DGkT0&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=27&ab_channel=freeCodeCampBengali) [5 Refactor Add a Service Layer Write Some Code Part 2 - YouTube](https://www.youtube.com/watch?v=UToTqLleS9A&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=28&ab_channel=freeCodeCampBengali)**Big Picture**![](https://lh6.googleusercontent.com/e6NTeQPPgLfc-UXuLtBFr8UXBdkW4cKfrXdzwceaK7fO42cWaPhaBP2UkLXJCCh9lq61_18BDQy3jlods8mvZtey4fNtNDfm3GDnOfCcqtkWJ7-pzHC8i_Wis-hQdqjR262y-D-oGlXUyB0WYhF8dRw)**Refactor: Add a Service Layer**![](https://lh6.googleusercontent.com/UZHA-6ETfHvdDPrQLd7wywFrH3oXXb2uaSRvD1Ytm7TKkBCW5stuDJRDZwjG4BSczCDDMCCXdr6JsO8pvDYGLtRWHYlAZ3yll0ntcvIkdAN3b0ZAAeT94TTBNwdM4HMnIPu0mks29P8QJpD6FDUzz3M)**Purpose of Service Layer**- **Service Facade** design pattern
- Intermediate layer for custom business logic
- Integrate data from multiple sources (DAO/repositories)**Integrate Multiple Data Sources**Service layer can write custom business logic with multiple data sources by using multiple DAO’s.![](https://lh6.googleusercontent.com/y8xcWcbOksW4139wPj4erv29-dgyPD_yS7Odz4B84uMmIiMOp8iClvYCdInHsIByxW5DxX2S1sTq5cRyM3TkGcVAUo4uLFotsKM-5VrETfbEwy99qq6NvCQsCrBHujsglZnROZcZxf_BKjNL16gyhGA)**Specialized Annotation for Services**- Spring provides the @Service annotation

  - @Service applied to Service implementations

  - Spring will automatically register the Service implementation

    - thanks to component-scanning![](https://lh3.googleusercontent.com/oag5WaduQ2MTgy44fI00WHOKa1FmXLdw-AGQ7DaILcWvwdmDQ_THsFEMJreEQYfhxqQP_636Cz0Ukfx1Ikdml6PhKi_YaVrLLAMBZtnWD0A0fenN4Oa-xcp4GFh0Ymka0X4irk0IUIG-j4Uu2Tlz4dc)**Revised Big Picture**![](https://lh4.googleusercontent.com/xvvpZfeCvXlggO_DmP37kwWg0OZGEsT2G4akThEnsKkBuIpI2unQEgAILFRpoj63Bw5eZDgeSiXOmdbx-hbs58dTaUxu-bSKmae4tf-9zPARurVNWpyENjNqMYFmWFi1eaN7U07XOLzjxH8kXJ1OeuA)Customer Service1. Define Service Interface

2. Define Service implementation

   1. Inject the CustomerDAO

3. Use the Service layer object inside controllers or update  codes of other layers accordinglyCreate a package for the service layer![](https://lh4.googleusercontent.com/m4Hb17qjYfMEkDa1es_STwFCE46DL9ot_zxuJT6bVYTfnBWisMU1duGQk1sxYgZlBb4O4oGz0LO72xekLvfWhXjDZhGlmZ45VkMXAAE5RxI2Fq5dcchDx8beoTXyeRc54Gm959yWCbRdEukIdwZZrcE)**\[Updated Codes]****Step 1**: Define Service interface**public** **interface** CustomerService {  **public** List&lt;Customer> getCustomers();}**Step 2**:Define Service implementation, then Inject the CustomerDAO@Service**public** **class** CustomerServiceImpl **implements** CustomerService{  @Autowired  CustomerDAO customerDAO;  @Transactional // good practice to move transaction annotation in service layer instead of using in DAO layer  @Override  **public** List&lt;Customer> getCustomers() {        // **TODO** Auto-generated method stub        **return** customerDAO.getCustomers();  }}**Step 3:** Use Service layer object inside controllers or update  codes of other layers accordingly**File**: CustomerController.java@Controller@RequestMapping("/customer")**public** **class** CustomerController { //   @Autowired//   CustomerDAO customerDAO; // bad practice   @Autowired  CustomerService customerService;   //@RequestMapping("/list") // removed  @GetMapping("/list") // Refactored, try PostMapping, you will get an error  **public** String listCustomers (Model theModel) {               //get the customers from dao        List&lt;Customer> theCustomers = customerService.getCustomers();               //add customer to the model        theModel.addAttribute("customers", theCustomers);               System.**_out_**.println(theCustomers);               **return** "list-customers";  }}**File**: CustomerDAOImpl.java@Repository**public** **class** CustomerDAOImpl **implements** CustomerDAO{   @Autowired  **private** SessionFactory sessionFactory;   //Removed @Transactional // Bad Practice to put this annotation here, instead of Service layer  @Override  **public** List&lt;Customer> getCustomers() {        // **TODO** Auto-generated method stub        Session currentSession = sessionFactory.getCurrentSession();        List&lt;Customer> customers = currentSession.createQuery("from Customer", Customer.**class**).getResultList();               **return** customers;  } }**FAQ**: 1. @Component vs @Service vs @Repository

   1. [java - What's the difference between @Component, @Repository & @Service annotations in Spring? - Stack Overflow](https://stackoverflow.com/questions/6827752/whats-the-difference-between-component-repository-service-annotations-in)**Query?**1. **How do I separate the DAO @Repository layer and @Service layer that Chad did not do!****


### Add a new Customer


##### **[17-add-customer-overview.pdf](https://drive.google.com/file/d/1qQYkNUaIdMha4Bzx3EyDJSXP8grURsXS/view?usp=share_link)[1 Add Customer Overview - YouTube](https://www.youtube.com/watch?v=oRwm5ie3MKQ&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=29&ab_channel=freeCodeCampBengali) [2 Add Customer Setting up the Add Button Part 1 - YouTube](https://www.youtube.com/watch?v=cAajTXeZ9x4&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=30&ab_channel=freeCodeCampBengali)[3 Add Customer Setting up the Add Button Part 2 - YouTube](https://www.youtube.com/watch?v=z9lq4CUErvk&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=31&ab_channel=freeCodeCampBengali)[4 Add Customer Creating the HTML Form Part 1 - YouTube](https://www.youtube.com/watch?v=iI_kyKtNXSM&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=32&ab_channel=freeCodeCampBengali)[5 Add Customer Creating the HTML Form Part 2 - YouTube](https://www.youtube.com/watch?v=D96GjFwTvJk&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=33&ab_channel=freeCodeCampBengali)[6 Add Customer Creating the HTML Form Part 3 - YouTube](https://www.youtube.com/watch?v=4-m9gQ2GGX4&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=34&ab_channel=freeCodeCampBengali)[7 Add Customer Save to Database Part 1 - YouTube](https://www.youtube.com/watch?v=IBltO4xUmZg&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=35&ab_channel=freeCodeCampBengali)[8 Add Customer Save to Database Part 2 - YouTube](https://www.youtube.com/watch?v=sgibMlovPlM&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=36&ab_channel=freeCodeCampBengali)[9 Sort Customer Data - YouTube](https://www.youtube.com/watch?v=-5ffUhcKCDY&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=37&ab_channel=freeCodeCampBengali)![](https://lh4.googleusercontent.com/NZ9Gv535EgnWBhjI6w8cBhdki7GEQ2Lb3jVPC0djZtEkJUI8JVgCGuto_ZBIiqZCovnb_M4Mmq5HHEE681TrYkS78Cce_J4ojtgLt1LbLzICaaMx9rp8ZDZrG3uHOVCquvXfb483lE-hxqvTaztULUw)Clicking add customer will serve this page,![](https://lh4.googleusercontent.com/ukFMxc2ySBLHGPZZGMr1QT6nY1efm0GGKpv34_csccNjahGhpF4K7fQ4UMF_I0sDNK6LgzQbcfWH5i9rxZVQAx4JGYsGWebTyobj0ToAon06DF1ZDxNB2sxCq9hM6FwT4Y_lfvOGns_FqoUzxxIn3Kc)Big Picture![](https://lh5.googleusercontent.com/L0dYZD3GtGgneoG_sehMFsIyl1CV_3eXW7HQ0YKrh5rT0GCSlRp9LopyuVz-iEzxSzgPKqUrF08rz3g7E-vdprUh4RnNPXbQi5aU8FjsVaCDW-hRSx1OL6wBtUaUgx1LE76we22nN8ygQ5m7TtVSHe8)**


#### Dev Process - Step By Step


##### **1. Update list-customer.jsp

   1. New “Add Customer” button

2. Create HTML form for new customer

   1. Create a HTML form for saving customer
   2. Define a new Controller method to serve the form page

3. Process Form Data to save it

   1. Controller -> Service -> DAO

      1. Update controller

      2. Update Service layer

         1. Update Service Interface
         2. Update the Implementation class 

      3. Update DAO layer

         1. Update DAO Interface
         2. Update the DAO Implementation class - ~~Update list-customer.jsp~~

  - ~~New “Add Customer” button~~

- ~~Create HTML form for new customer~~

  - Create a HTML form for saving customer
  - ~~Define a new Controller method to serve the form page~~

- ~~Process Form Data to save it~~

  - ~~Controller -> Service -> DAO~~**Step 1**:1. “Add Customer” button&lt;body>&lt;!--List Customers - coming soon-->&lt;div class=_"wrapper"_>&lt;/div>&lt;div class=_"container"_>  &lt;div class=_"content"_>        &lt;!-- put new button: add customer -->        &lt;input type=_"button"_ value=_"Add Customer"_        onCLick="window.location.href='showFormForAdd'; return false;"        class=_"add-button"_/>        &lt;table>                &lt;/table>  &lt;/div> &lt;/div>&lt;/body>**Step 2**: Create HTML form for new customer**Part 1**: Create a HTML form for saving customer**File**:/web-customer-tracker/src/main/webapp/WEB-INF/view/customer-form.jsp&lt;%@ page language=_"java"_ contentType=_"text/html; charset=ISO-8859-1"_pageEncoding=_"ISO-8859-1"_%>&lt;%@ taglib uri=_"http&#x3A;//www.springframework.org/tags/form"_prefix=_"form"_%>&lt;!DOCTYPE html>&lt;html>&lt;head>  &lt;meta charset=_"ISO-8859-1"_>  &lt;title>Add a new Customer&lt;/title>  &lt;!-- Reference our style sheet -->  &lt;link type=_"text/css"_ rel=_"stylesheet"_ href=_"_${pageContext.request.contextPath}_/resources/css/style.css"_>  &lt;link type=_"text/css"_ rel=_"stylesheet"_ href=_"_${pageContext.request.contextPath}_/resources/css/add-customer-style.css"_/>&lt;/head>&lt;body>   &lt;div class=_"wrapper"_>        &lt;div class=_"header"_>             &lt;h2>CRM - Customer Relationship Manager&lt;/h2>             &lt;!-- ${pageContext.request.contextPath} -->        &lt;/div>  &lt;/div>  &lt;div class=_"container"_>        &lt;h3>Save customer&lt;/h3>        &lt;form:form modelAttribute=_"customer"_ action=_"saveCustomer"_ method=_"POST"_>             &lt;table>                  &lt;tbody>                        &lt;tr>                             &lt;td>&lt;label>First name:&lt;/label>&lt;/td>                             &lt;td>&lt;form:input path=_"firstName"_ placeholder=_"John"_/>&lt;/td>                        &lt;/tr>                        &lt;tr>                             &lt;td>&lt;label>Last name:&lt;/label>&lt;/td>                             &lt;td>&lt;form:input path=_"lastName"_ placeholder=_"Doe"_>&lt;/form:input>&lt;/td>                        &lt;/tr>                        &lt;tr>                             &lt;td>&lt;label>Email:&lt;/label>&lt;/td>                             &lt;td>&lt;form:input path=_"email"_ placeholder=_"john@gmail.com"_>&lt;/form:input>&lt;/td>                        &lt;/tr>                        &lt;tr>                             &lt;td>&lt;label>&lt;/label>&lt;/td>                             &lt;td>&lt;input type=_"submit"_ value=_"Save"_ class=_"save"_>&lt;/input>&lt;/td>                        &lt;/tr>                  &lt;/tbody>             &lt;/table>        &lt;/form:form>  &lt;/div>  &lt;div style="clear; both">&lt;/div>  &lt;p>        &lt;a href=_"_${pageContext.request.contextPath}_/customer/list"_>Back to List&lt;/a>  &lt;/p>&lt;/body>&lt;/html>**Part 2**: Define a new Controller method to serve the form page**File**: com.dpauld.springdemo.controller/CustomerController.java**public** **class** CustomerController {  @Autowired  CustomerService customerService;   @GetMapping("/list")  **public** String listCustomers (Model theModel) {        // codes        **return** "list-customers";  }   @GetMapping("/showFormForAdd")  **public** String showFormForAdd (Model theModel) {               //create customer object to add as a model attribute to bind the form data        Customer theCustomer = **new** Customer();               theModel.addAttribute("customer", theCustomer);        **return** "customer-form";  }}**Step 3:** Process Form Data to save it**Part 1**: Update Customer controller**File**: com.dpauld.springdemo.controller/CustomerController.java**public** **class** CustomerController {   @Autowired  CustomerService customerService;   @GetMapping("/list")  **public** String listCustomers (Model theModel) {        // codes        **return** "list-customers";  }   @GetMapping("/showFormForAdd")  **public** String showFormForAdd (Model theModel) {        //codes    **return** "customer-form";  }   @PostMapping("/saveCustomer")  **public** String saveCustomer (@ModelAttribute("customer") Customer theCustomer,Model theModel) {        customerService.saveCustomer(theCustomer);               **return** "redirect:/customer/list";  } }**Part 2**: Update DAO layer by updating both interface and implementation**File**: com.dpauld.springdemo.dao/CustomerDAO.java@Repository**public** **class** CustomerDAOImpl **implements** CustomerDAO{   @Autowired  **private** SessionFactory sessionFactory;   //Removed @Transactional // Bad Practice to put this annotation here, instead of Service layer  @Override  **public** List&lt;Customer> getCustomers() {        // **TODO** Auto-generated method stub        Session currentSession = sessionFactory.getCurrentSession();        List&lt;Customer> customers = currentSession.createQuery("from Customer", Customer.**class**).getResultList();               **return** customers;  }   @Override  **public** **void** saveCustomer(Customer theCustomer) {        // **TODO** Auto-generated method stub        Session currentSession = sessionFactory.getCurrentSession();        currentSession.save(theCustomer);  } }**Part 3**: Update Service layer by updating both interface and implementation**File**: com.dpauld.springdemo.service/CustomerService.java@Service**public** **class** CustomerServiceImpl **implements** CustomerService{   @Autowired  CustomerDAO customerDAO;   @Transactional // good practice to move transaction annotation in service layer instead of using in DAO layer  @Override  **public** List&lt;Customer> getCustomers() {        // **TODO** Auto-generated method stub        **return** customerDAO.getCustomers();  }   @Transactional  @Override  **public** **void** saveCustomer(Customer theCustomer) {        // **TODO** Auto-generated method stub        customerDAO.saveCustomer(theCustomer);  } }[**_window.location.href Property_**](https://www.geeksforgeeks.org/difference-between-window-location-href-window-location-replace-and-window-location-assign-in-javascript/)**:**- The **href** property on the location object stores the URL of the current webpage.
- On changing the **href** property, a user can navigate to a new URL, i.e. go to a new webpage.
- It adds an item to the history list (so that when the user clicks the “Back” button, he/she can return to the current page).
- Updating the href property is considered to be faster than using the assign() function (as calling a function is slower than accessing the property).**


### Update a Customer


##### **[18-update-customer-overview.pdf](https://drive.google.com/file/d/1bVbN51iNnWbmZNIucHCNl8LYhYEho3Kr/view?usp=share_link)[1 Update Customer Overview - YouTube](https://www.youtube.com/watch?v=zaXgXDNauos&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=38&ab_channel=freeCodeCampBengali)[2 Update Customer Creating Update Link - YouTube](https://www.youtube.com/watch?v=MdH4jhW7YfA&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=39&ab_channel=freeCodeCampBengali)[7 Update Customer Save Customer to Database Part 2 - YouTube](https://www.youtube.com/watch?v=JeGCMIijaNQ&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=43&ab_channel=freeCodeCampBengali)![](https://lh5.googleusercontent.com/MhO23NO6Ag6NiINalKDS2j7PlKLufws0kZYcOv1Fp9etfFhTXtWFhGGJxywtCRCwwssHLQZ8CepeIEGauSEzdIQuiGVv65-zf3dFgqAYN4-PGMCXxuxZLaBy6_0Pz0u1pD36Rq6rxJFlCRT_XQysfBI)Action Link - Update![](https://lh6.googleusercontent.com/tFCvUNLrXVmGScUDKaynIyECIx7EXQjKBKNKuTUwD4gBaofebrzIgqgCrzW8K81OnNeA54cpEKEP_2GKWzo59HvSulWqar_Oe8vcWXIElv5I19DIDVBCDvsff8CJCA78aoeSanzTJ4Z_RPafvV7KaTw)Each row has an Update link,- current customer id embedded in linkWhen clicked,- will load the customer from database
- prepopulate the form**


##### Dev Process - (Step-By-Step )


##### **1. Update list-customers.jsp

   1. New “Update” link

2. Create/Update customer-form.jsp (already created when developing add customer)

   1. Prepopulate the form
   2. Add a hidden tag for id in customer-form.jsp

3. Process form data

   1. Controller > Service > DAO**Note**: In this case we will update step 2 and step 3 interchangeably.**Checklist**- ~~Update list-customers.jsp~~

  - ~~New “Update” link~~

- ~~Create customer-form.jsp (already created)~~

  - ~~Prepopulate the form~~

- ~~Process form data~~

  - Controller > Service > DAO

    - Update controller

    - Update DAO layer

      - Update the DAO Implementation class**Step 1:****File:** _view/list-customer.jsp_&lt;%@ page language=_"java"_ contentType=_"text/html; charset=ISO-8859-1"_pageEncoding=_"ISO-8859-1"_%>&lt;!-- to enable support for jstl tags -->&lt;%@ taglib uri = _"http&#x3A;//java.sun.com/jsp/jstl/core"_ prefix = _"c"_ %>&lt;!DOCTYPE html>&lt;html> &lt;head>  &lt;meta charset=_"ISO-8859-1"_>  &lt;title>List Customers&lt;/title>   &lt;!-- Reference our style sheet -->   &lt;link type=_"text/css"_  rel=_"stylesheet"_  href=_"_${pageContext.request.contextPath}_/resources/css/style.css"_> &lt;/head> &lt;body>&lt;!--List Customers - coming soon-->&lt;div class=_"wrapper"_>  &lt;div class=_"header"_>        &lt;h2>CRM - Customer Relationship Manager&lt;/h2>        &lt;!-- ${pageContext.request.contextPath} -->  &lt;/div>&lt;/div>&lt;div class=_"container"_>  &lt;div class=_"content"_>        &lt;!-- put new button: add customer -->        &lt;input type=_"button"_ value=_"Add Customer"_        onCLick="window.location.href='showFormForAdd'; return false;"        class=_"add-button"_/>        &lt;table>             &lt;tr>                  &lt;th>First Name&lt;/th>                  &lt;th>Last Name&lt;/th>                  &lt;th>Email&lt;/th>                  &lt;th>Action&lt;/th>             &lt;/tr>             &lt;!-- added taglib directive to enable jstl tags support -->             &lt;c:forEach var=_"tempCustomer"_ items=_"_${customers}_"_>                              &lt;!-- Construct and update link with customer Id -->                  &lt;c:url var=_"updateLink"_ value=_"/customer/showFormForUpdate"_>                        &lt;c:param name=_"customerId"_ value=_"_${tempCustomer.id}_"_>&lt;/c:param>                  &lt;/c:url>                                   &lt;tr>                        &lt;td>${tempCustomer.firstName}&lt;/td>                        &lt;td>${tempCustomer.lastName}&lt;/td>                        &lt;td>${tempCustomer.email}&lt;/td>                        &lt;td>                             &lt;!-- Display the update link -->                             &lt;a href=_'_${updateLink}_'_>Update&lt;/a>                        &lt;/td>                  &lt;/tr>             &lt;/c:forEach>        &lt;/table>  &lt;/div> &lt;/div>&lt;/body>&lt;/html>**Step 3:****Part 3(A):** Prepopulating by calling this controller**/\* Controllers for Update \*/**  ******@GetMapping("/showFormForUpdate")**  ******public String showFormForUpdate(@RequestParam("customerId") int theCustomerId,Model theModel) {**       ********        ******//get the customer from db**        ******Customer theCustomer = customerService.getCustomer(theCustomerId);**                 ********        ******//set this customer as a model attribute to re-populate the form**        ******theModel.addAttribute("customer", theCustomer);**       ********        ******// send the control over to the form**        ******return "customer-form";**  ******}**Calling the above method will do the **step of 2(b)****Part 3(B):** After Step 2**Step 2:** Update customer-form.jsp1. Prepopulate the form
2. Add a hidden tag for id**File**: customer-form.jsp&lt;body>  &lt;div class=_"container"_>        &lt;h3>Save customer&lt;/h3>        &lt;form:form modelAttribute=_"customer"_ action=_"saveCustomer"_ method=_"POST"_>&lt;!-- Add a hidden tag for specifying path for customer id, so that spring knows which id to use and spring can use its setId for updating the customer -->             &lt;form:hidden path=_"id"_>&lt;/form:hidden>             &lt;table>                  &lt;tbody>                        &lt;tr>                             &lt;td>&lt;label>First name:&lt;/label>&lt;/td>                             &lt;td>&lt;form:input path=_"firstName"_ placeholder=_"John"_/>&lt;/td>                        &lt;/tr>                        &lt;tr>                             &lt;td>&lt;label>Last name:&lt;/label>&lt;/td>                             &lt;td>&lt;form:input path=_"lastName"_ placeholder=_"Doe"_>&lt;/form:input>&lt;/td>                        &lt;/tr>                        &lt;tr>                             &lt;td>&lt;label>Email:&lt;/label>&lt;/td>                             &lt;td>&lt;form:input path=_"email"_ placeholder=_"john@gmail.com"_>&lt;/form:input>&lt;/td>                        &lt;/tr>                        &lt;tr>                             &lt;td>&lt;label>&lt;/label>&lt;/td>                             &lt;td>&lt;input type=_"submit"_ value=_"Save"_ class=_"save"_>&lt;/input>&lt;/td>                        &lt;/tr>                  &lt;/tbody>             &lt;/table>        &lt;/form:form>  &lt;/div>  &lt;div style="clear; both">&lt;/div>  &lt;p>        &lt;a href=_"_${pageContext.request.contextPath}_/customer/list"_>Back to List&lt;/a>  &lt;/p>&lt;/body>**Part 2(a)**After clicking update it will call a controller method from **step 3 - Part 3(A)** which will Prepopulate the form****![](https://lh3.googleusercontent.com/Hg7YlVH4GFB2yHvVNz6vtCfIQxKVhqxDmDGPM7IYQFvZ1NX9fXQzAKKOy3sVwoq--HE1Gt-zY7SEojNwberRuYrxT5JmakAPWJRDjyt1cnFZqQ16KFKfnibtclgTDlPWoiB0_aZCYYxXUfj0gRrSVRM)****Since we added customer as a model attribute and thus binded it to the form, thus Spring has the ability to call the getter and setter methods of each field of the form using the path attribute value, for example, for setting First Name spring can use its path=_"firstName"_ attribute, to call its setter method => “get” + “firstName” =>  “get” + “FirstName” => getFirstName()._Now, How will the update work?_**Part 2(B)** Add a hidden tag for idThis tag is very important for updating the customer, it is used for specifying path attributes for customer id, so that spring can use its setId method for updating the customer.             &lt;form:hidden path=_"id"_>&lt;/form:hidden>**Step 3:****Part 3(B):** Update the DAO Layer - DAO Implementation class**File**: @Repository**public** **class** CustomerDAOImpl **implements** CustomerDAO{   @Autowired  **private** SessionFactory sessionFactory;// Other methods  @Override  **public** **void** saveCustomer(Customer theCustomer) {        // **TODO** Auto-generated method stub        Session currentSession = sessionFactory.getCurrentSession();        //currentSession.save(theCustomer);// previous version        currentSession.saveOrUpdate(theCustomer); //updated version for the use of update  }// Other methods}**Method: saveOrUpdate ( . . . )**if (primaryKey / id) emptythen INSERT new customerelse UPDATE existing customerIt inserts a new customer if primaryKey which is the id is empty, otherwise it updates the customer.<https://stackoverflow.com/questions/11881479/how-do-i-update-an-entity-using-spring-data-jpa#:~:text=Perhaps%20I%20should,that%20record%20automatically.>**


### Delete a Customer


##### **[19-delete-customer-overview.pdf](https://drive.google.com/file/d/1JT5jkO9mgfVbAJbt0Q47Ln_Ne0_EOvv9/view?usp=share_link)[1 Delete Customer Overview - YouTube](https://www.youtube.com/watch?v=6GqIQxlwfoo&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=45&ab_channel=freeCodeCampBengali)[2 Delete Customer Creating Delete Link Part 1 - YouTube](https://www.youtube.com/watch?v=Zdgq_6AzUJo&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=46&ab_channel=freeCodeCampBengali)[3 Delete Customer Creating Delete Link Part 2 - YouTube](https://www.youtube.com/watch?v=Y-5wHXEV87s&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=49&ab_channel=freeCodeCampBengali)Controllers, Services, DAO:[4 Delete Customer Delete from Database Part 1 - YouTube](https://www.youtube.com/watch?v=LsHjR-jb15I&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=50&ab_channel=freeCodeCampBengali)[5 Delete Customer Delete from Database Part 2 - YouTube](https://www.youtube.com/watch?v=IfMHFY1u1mI&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=49&ab_channel=freeCodeCampBengali)[6 Delete Customer Delete from Database Part 3 - YouTube](https://www.youtube.com/watch?v=Tbo90m9rLRM&list=PLon9KQO-XVcuvjULTcRDuf8guWy3JSGlA&index=48&ab_channel=freeCodeCampBengali)**


##### Delete Customer - Dev Process (Step by Step)


##### **1. Add “Delete” link on JSP

2. Add code for “Delete”

   1. Controller > Service > DAO

      1. Update controller

      2. Update Service layer

         1. Update Service Interface
         2. Update the Implementation class 

      3. Update DAO layer

         1. Update DAO Interface
         2. Update the DAO Implementation class**Step 1**: Add “Delete” link on JSP&lt;body>&lt;div class=_"container"_>  &lt;div class=_"content"_>        &lt;!-- put new button: add customer -->        &lt;input type=_"button"_ value=_"Add Customer"_        onCLick="window.location.href='showFormForAdd'; return false;"        class=_"add-button"_/>        &lt;table>             &lt;tr>                  &lt;th>First Name&lt;/th>                  &lt;th>Last Name&lt;/th>                  &lt;th>Email&lt;/th>                  &lt;th>Action&lt;/th>             &lt;/tr>             &lt;!-- added taglib directive to enable jstl tags support -->             &lt;c:forEach var=_"tempCustomer"_ items=_"_${customers}_"_>                              &lt;!-- Construct and update link with customer Id -->                  &lt;c:url var=_"updateLink"_ value=_"/customer/showFormForUpdate"_>                        &lt;c:param name=_"customerId"_ value=_"_${tempCustomer.id}_"_>&lt;/c:param>                  &lt;/c:url>                                   &lt;!-- Construct and delete link with customer Id -->                  &lt;c:url var=_"deleteLink"_ value=_"/customer/deleteCustomer"_>                        &lt;c:param name=_"customerId"_ value=_"_${tempCustomer.id}_"_>&lt;/c:param>                  &lt;/c:url>                  &lt;tr>                        &lt;td>${tempCustomer.firstName}&lt;/td>                        &lt;td>${tempCustomer.lastName}&lt;/td>                        &lt;td>${tempCustomer.email}&lt;/td>                        &lt;td>                             &lt;!-- Display the update link -->                             &lt;a href=_'_${updateLink}_'_>Update&lt;/a>                             |                             &lt;a href=_'_${deleteLink}_'_ onClick="return confirm('Are you sure you want to delete this customer?');">Delete&lt;/a>                        &lt;/td>                  &lt;/tr>             &lt;/c:forEach>        &lt;/table>  &lt;/div> &lt;/div>&lt;/body>**Step 2:** **Part 2(1)** Update Controller classFile: CustomerController.java@Controller@RequestMapping("/customer")**public** **class** CustomerController {   @Autowired  CustomerService customerService;   /\* Controllers for Delete \*/  @GetMapping("/deleteCustomer")  **public** String deleteCustomer(@RequestParam("customerId") **int** theCustomerId, Model theModel) {        customerService.deleteCustomer(theCustomerId);        **return** "redirect:/customer/list";  }}**Part 2(2):** Update Service ImplementationsFile: com.dpauld.springdemo.services/CustomerController.java@Service**public** **class** CustomerServiceImpl **implements** CustomerService{  @Autowired  CustomerDAO customerDAO;  @Transactional  @Override  **public** **void** deleteCustomer(**int** theCustomerId) {        // **TODO** Auto-generated method stub        customerDAO.deleteCustomer(theCustomerId);  }}**Part 2(3)**: Update DAO ImplementationsFile: com.dpauld.springdemo.dao/CustomerDAOImpl.java@Repository**public** **class** CustomerDAOImpl **implements** CustomerDAO{  @Autowired  **private** SessionFactory sessionFactory;  @Override  **public** **void** deleteCustomer(**int** theCustomerId) {        // **TODO** Auto-generated method stub        // get the current hibernate session        Session currentSession = sessionFactory.getCurrentSession();         // delete object with primary key        Query theQuery = currentSession.createQuery("delete from Customer where id=: customerId");        theQuery.setParameter("customerId", theCustomerId);        theQuery.executeUpdate();  }}**


### FAQ


##### **1. [How to get the GET request query string with url in Spring?](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.hhysi9wzkwlw)
2. [How to get the request body of a POST request?](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.qzxrx17zd6rb)
3.**


## Project Directory Structure


##### **![](https://lh4.googleusercontent.com/WHrsU6h9qa03ud_nLLsX0e5QF9K6nJ4hd9RPDI5PLF9lVaD_DkaBhYqZEykXfqd3sokAI2hNwN6NjTxYeI9W3GP7yAOyoTNagSJ7mCgEMfaMNr3-WEJ0iSbTCwQfItW6VD37PhH1ZTUKqKHEsNMy7cs)AOPReadings : [Spring AOP Example Tutorial - Aspect, Advice, Pointcut, JoinPoint, Annotations, XML Configuration | DigitalOcean](https://www.digitalocean.com/community/tutorials/spring-aop-example-tutorial-aspect-advice-pointcut-joinpoint-annotations)**


# AOP Aspect-Oriented Programming Overview


##### **[01-spring-aop-overview.pdf](https://drive.google.com/file/d/1dQwp1Mx--FOxqeu7ewP4kAZASEbEvf3w/view?usp=share_link)[02-spring-aop-support.pdf](https://drive.google.com/file/d/1V0_Wt4TmPPsp9mXBATpmcZygeotcCizL/view?usp=share_link)**


## Why do we need AOP?


##### **So far a typical **Application Architecture** looked like this,![](https://lh4.googleusercontent.com/KcQPyP3LiqEmQBVwo_Mm3VJwMSRsxWSxyj6TCbJ8BsbLZM5FSxvyVyvojJElDEBHhGa-idpq4Fc2OsFz2LU27V0o7pfYxvOuOcvIqWZzU5B36B3PbPAfcJ5TOASxyA-O_Kya84KYgvaJUTbYtZxiszs)And **codes for DAO object** looked like this, public void addAccount(Account theAccount, String userId) {Session currentSession = sessionFactory.getCurrentSession();currentSession.save(theAccount);}Now Imagine we have some **new requirements**,1. Logging 

   1. Add some logging statements before the start of the method

2. Security 

   1. Make sure user is authorized before running DAO methodA **possible solution to meet the requirement** is to add some lines of codes for them at the top of the method, just like this,public void addAccount(Account theAccount, String userId) {// codes for logging// code for securitySession currentSession = sessionFactory.getCurrentSession();currentSession.save(theAccount);}Our **solutions are not over yet**, Let’s **add it to all of our layers**…![](https://lh3.googleusercontent.com/c5elVvx9dPVNGY49fD79nKlouv4BCAfvU-6H7-IlyvZWDQi1frPZwMfMM4xDt8IGPaYQSJmCCET1ZDqKZWyImKyM50KtISS9p9TzIUrPNdTSDKwBnU1AxozZ_bG1qY46k74h-un34zVtV1bF8KCptvU)If we have many other DAO’s we have to do the same thing for all of them, doing the same shit everywhere, repetition.![](https://lh4.googleusercontent.com/sjQEcoOM-DXavenpuXMXo6SZ-mh1B8aRB40JoMW2L675pY586AQwQUIsbllloDx7QBUj66hNwTFv34jnuqwbb2sZiQW6ZMN_hAYxDtDYtwGs3OtjvadYN93ujQ1pbqHQa9tRVeQlmstQTqc2TqEhgoo)**


### Two Main Problems Arises


##### **Code Tangling - - Code tangling is caused when a module/a specific piece of code is implemented in a way to handle multiple functions or multiple concerns simultaneously.
- In this case, for a given method: addAccount(...)
- We have logging and security code tangled inCode [Scattering](https://www.google.com/search?q=scattered+meaning&sxsrf=APwXEdfQwT5llz-Y1kRIYYLsXZf3udgTUg%3A1684281352469&ei=CBhkZOqnHKSHg8UPnJ6ouA0&oq=scatter&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQARgBMgwIABCKBRBDEEYQ_wEyBwgAEIoFEEMyBwgAEIoFEEMyDQgAEIoFELEDEIMBEEMyBwgAEIoFEEMyBwguEIoFEEMyBQgAEIAEMgsIABCABBCxAxCDATILCAAQgAQQsQMQgwEyBQgAEIAEOgoIABBHENYEELADOgoIABCKBRCwAxBDOg0IABDkAhDWBBCwAxgBOg8ILhCKBRDIAxCwAxBDGAI6EgguEIoFENQCEMgDELADEEMYAkoECEEYAFDjAljGD2CXKWgBcAF4AIABcogB4QGSAQMwLjKYAQCgAQHIARLAAQHaAQYIARABGAnaAQYIAhABGAg&sclient=gws-wiz-serp#:~:text=occurring%20or%20found%20at%20intervals%20or%20various%20locations%20rather%20than%20all%20together.)- Scattering is caused when code performing a specific function is fragmented and all over the place.
- If we need to change logging or security code
- We have to update ALL classes**Other possible solutions?**Inheritance?- Every class would need to inherit from a base class
- Can all classes extend from your base class? ... plus (java) does not support multiple inheritanceDelegation?- Classes would delegate logging, security calls
- Still would need to update classes if we wanted to
- add/remove logging or security
- add new feature like auditing, API management, instrumentation**FAQ**: What is Delegation?1. [Delegation vs Inheritance in Java - GeeksforGeeks](https://www.geeksforgeeks.org/delegation-vs-inheritance-java/)
2. [Delegation | Java Design Patterns (java-design-patterns.com)](https://java-design-patterns.com/patterns/delegation/#explanation)**


### Best Solution to meet the requirements - AOP


##### **- Programming technique based on concept of an Aspect

- Aspect encapsulates cross-cutting logic

  - Cross-Cutting Concerns

- “Concern” means logic / functionality![](https://lh5.googleusercontent.com/QHcrkG0Q-FmnaQY5EQQPQA-UFPR8YxsIIeoHbdL_oyz5gcWfvdxZGKPyUngFM1Ohj7lua0UzZLQx78P42epQTTVFKWmRUlQFLqjaeWiPivsvQpdigwAOwm_HYTC8D0RtKXdJpbtj7YHB2zIw1spz3lA)AOP breaks the program logic into distinct parts (called concerns). **Cross-cutting concerns** are parts of a program that rely on or must affect many other parts of the system. In aspect-oriented programming, **cross-cutting concerns** are aspects of a program that affect several modules, without the possibility of being encapsulated in any of the modules.To elaborate, aspect-oriented programming (AOP) is a programming paradigm that aims to increase modularity by allowing the separation of cross-cutting concerns. It does so by adding behavior to existing code (an advice) without modifying the code itself, instead separately specifying which code is modified via a "pointcut" specification, such as "log all function calls when the function's name begins with 'set'" or “check if the user is authorized before giving access to call a method”. This allows behaviors that are not central to the [business logic](https://en.wikipedia.org/wiki/Business_logic) (such as logging, or authorization) to be added to a program without cluttering the code core to the functionality.Aspects- Aspect can be reused at multiple locations
- Same aspect/class ... applied based on configuration![](https://lh3.googleusercontent.com/A-pZ_AWy5_SJtE4hGH5elMESjpoMYcZOggFXdHDYnXVGI1zfQbKY8jcrzY-Q-EzXoaCu62leOh-RY2U_QvwmP8Mgd__HKWbuk-07MerryS1LjxiAZwDLprB_sujH3DzGIH_DyDiofPNRzHo9vZ2uIqg)Applying AOP is kind of applying  the Proxy design pattern, where the main app has no idea of any aspects or any proxies. ![](https://lh6.googleusercontent.com/-MEbKpB628nYzcDGlGG34TSskbgtI9-OO_tDh_HYRvq5bcc9xFiARQNZho2t5xXeJGhtGDcntoeDmiQZHPFvYlqaWQjZjZadBHPK-UP1HGqxHQnRtkWdR4j_lTe08fqdNbHSSVCjFxIwGwXQiryNI9o)**


## Benefits of AOP


##### **- Code for Aspect is defined in a single class

  - Much better than being scattered everywhere
  - Promotes code reuse and easier to change

- Business code in your application is cleaner

  - Only applies to business functionality: addAccount
  - Reduces code complexity

- Configurable

  - Based on configuration, apply Aspects selectively to different parts of app
  - No need to make changes to the main application code ... very important!**


### Additional AOP Use Cases


##### **- Most common

  - logging, security, transactions

- Audit logging

  - who, what, when, where

- Exception handling

  - log exception and notify DevOps team via SMS/email

- API Management

  - how many times has a method been called user
  - analytics: what are peak times? What is the average load? Who is the top user?**


## AOP: Advantages and Disadvantages


### Advantages 


##### **1. Reusable modules
2. Resolve code tangling
3. Resolve code scatter
4. Applied selectively based on configuration**


### Disadvantages


##### **1. Too many aspects and app flow is hard to follow
2. Minor performance cost for aspect execution (run-time weaving)**


## AOP Terminology


##### **1. Aspect: module of code for a cross-cutting concern (logging, security, ...); a class
2. Advice: What action is taken and when it should be applied; piece of code, mostly inside a method.
3. Join Point: When to apply code during program execution;
4. Pointcut: A predicate expression for where advice should be applied; this expression represents one or multiple Join Points.**Weaving**- Connecting aspects to target objects to create an advised object
- Different types of weaving
- Compile-time, load-time or run-time
- Regarding performance: run-time weaving is the slowest**


## Advice Types


##### **1. **Before advice**: run before the method
2. **After finally advice**: run after the method (finally)
3. **After returning advice**: run after the method (success execution)
4. **After throwing advice**: run after method (if exception thrown)
5. **Around advice**: run before and after method**


## AOP Frameworks


##### **1. Spring AOP

   1. Spring provides AOP support

   2. Key component of Spring

      1. Security, transactions, caching etc

   3. Uses run-time weaving of aspects

2. AspectJ

   1. Original AOP framework, released in 2001

      1. www.eclipse.org/aspectj

   2. Provides complete support for AOP

   3. Rich support for

      1. join points: method-level, constructor, field
      2. code weaving: compile-time, post compile-time and load-time[02-spring-aop-support.pdf - Google Drive](https://drive.google.com/file/d/1V0_Wt4TmPPsp9mXBATpmcZygeotcCizL/view)**


### Advantages and Disadvantages of Spring AOP


### Advantages and Disadvantages of AspectJ


### Comparing Spring AOP and AspectJ


## Spring AOP Roadmap


##### **1. Create Aspects

2. Develop Advices

   1. Before, After returning, After throwing,
   2. After finally, Around

3. Create Pointcut expressions

4. Apply it to our big CRM project (Spring MVC + Hibernate)**


## Dev Environment


##### **Adding AspectJ JAR File• Need to download AspectJ JAR file• Even though we are using Spring AOP ... still need AspectJ JAR file• Why?• Spring AOP uses some of the AspectJ annotations• Spring AOP uses some of the AspectJ classes**


# AOP @Before Advice Type


##### **[03-spring-aop-before-advice-overview.pdf](https://drive.google.com/file/d/1KwxnFcN7bvYnM1WTSfcPOQ2F4dqYoP5S/view?usp=sharing)[1 AOP @Before Advice Overview - YouTube](https://www.youtube.com/watch?v=grVuZg4EzZg&list=PLteFRIBg620fqItJF4bqKHdpnNhYHtnBY&index=4&ab_channel=courseUpload)[3 AOP @Before Advice Write Some Code - YouTube](https://www.youtube.com/watch?v=AegQENdZi1o&list=PLteFRIBg620fqItJF4bqKHdpnNhYHtnBY&index=6&ab_channel=courseUpload)[4 AOP @Before Advice Add and Test AOP Aspect - YouTube](https://www.youtube.com/watch?v=jSgRJickMv8&list=PLteFRIBg620fqItJF4bqKHdpnNhYHtnBY&index=8&ab_channel=courseUpload)Before advice: run before the method@Before Advice - Use Cases• Most common• logging, security, transactions• Audit logging• who, what, when, where• API Management• how many times has a method been called user• analytics: what are peak times? what is average load? who is top user?![](https://lh3.googleusercontent.com/DUKnXJ3wRySsCqzdF533Fp0qmCeuq0QmRplq5h8-0D7IcHU3ac7Kl4DqLeL2A6VvaSpGbV2kXhQfLOkTcJ7p70l3t5CIX4yBoDIlO4t7vRTb7kUmbYBhvX7KGp3ghi-NGQeUkABqsFE2s83WjqDS4XM)Development Process - @Before Step-By-Step1. Create target object: AccountDAO

2. Create Spring Java Config class

3. Create main app

4. Create an Aspect with @Before advice

   1. Add @Aspect annotation
   2. Add @Component annotation 
   3. Inside the class, just on top of the advice function add @Before annotation by passing a string which consists of an **execution method(**it indicates method execution joint cut point**)** that receives a pointcut expression.

5. Extra Step: Test the code without Advice then Try Advice**Step 1**: Create Target Object: AccountDAO@Componentpublic class AccountDAO {public void addAccount() {System.out.println("DOING MY DB WORK: ADDING AN ACCOUNT");}}**Step 2**: Create Spring Java Config class@Configuration**@EnableAspectJAutoProxy**@ComponentScan("com.luv2code.aopdemo")public class DemoConfig {}**Step 3**: Create main apppublic class MainDemoApp {public static void main(String\[] args) {// read spring config java classAnnotationConfigApplicationContext context =new AnnotationConfigApplicationContext(DemoConfig.class);// get the bean from spring containerAccountDAO theDAO = context.getBean("accountDAO", AccountDAO.class);// call the business methodtheDAO.addAccount();// close the contextcontext.close();}}**Step 4**: Create an Aspect with @Before advice@Aspect@Componentpublic class MyDemoLoggingAspect {@Before("execution(public void addAccount())")public void beforeAddAccountAdvice() {System.out.println("Executing @Before advice on addAccount()");}}**


# AOP Pointcut Expressions 


##### **[Spring aop aspectJ pointcut expression examples - HowToDoInJava](https://howtodoinjava.com/spring-aop/aspectj-pointcut-expressions/)[04-spring-aop-pointcut-expressions-overview-part-1.pdf](https://drive.google.com/file/d/1Yf53s4vTfhyJ996qJCIsZy8oyEFWFEIB/view?usp=sharing)[05-spring-aop-pointcut-expressions-overview-part-2.pdf](https://drive.google.com/file/d/1_t--tJuE_LWgczS_SHXq5AMTvwH-GO7L/view?usp=sharing)**


## Pointcut Expression Language


##### **- Spring AOP uses AspectJ’s pointcut expression language
- We will start with execution pointcuts
- Applies to execution of methods**


## AOP Pointcut Expressions - Match Methods and Return Types


### Pointcut Expressions Language


##### **execution(modifiers-pattern? return-type-pattern declaring-type-pattern? method-name-pattern(param-pattern) throws-pattern?)**Note**: The pattern is optional if it has “?”**


### Pointcut Expressions Example


#### Match on Method Name


##### ****Example Scenario 1:** Match only **addAccount()** method in **AccountDAO class**@Before("execution(public void com.luv2code.aopdemo.dao.AccountDAO.addAccount())")![](https://lh5.googleusercontent.com/p0HUQO_yvo6-tzyCV9uUk4kLJ3i4BvicapGqdXpa3TFpLPgjTpO2w5Mp0Eia-ojb7u4Xh2PvPlq2rcSkOQP9yuncUa4gc_8tPNmwlaoZEy2lluRYDPWG8HSnkeahNQO_BR-nTZ6jlWKkaw0DcCUvPBo)**Example Scenario 2:** Match any **addAccount**() method in **any class**@Before("execution(public void addAccount())")![](https://lh6.googleusercontent.com/lj6ve72QyM9z4wX8qtvuZ3GJqRoprSR9XHRAkCR5w5QhfnxTN0TJoDHKflZ8aJlpHpTEY-7ofX5tZyTFG7LRO7cfpIaboCjhfYkSiY6GMPpfyLV_6foMiyCT_s5wY8IFQs6aFdjQAZf-P9EM-p-bbwo)**


#### Match on method names (using wildcards)


##### ****Example Scenario 3:** Match methods **starting with add** in **any class**@Before("execution(public void add\*())")![](https://lh4.googleusercontent.com/DAbQDSTRiVEohKAhaOwz0ieORZ3ZtqlzRHNfT0un9RMzOXt9qzNP2L7CUe1Eeq3mZ4Hr5Nz50Qu9tA7YiXVDvQAP8bt5jVU4mEG-Mrd36mm-eAfMKXwkdrd8SdgfmXMJZuFcSSz6A2uY5B7hN11MRFQ)**Example Scenario 4:** Match methods **starting with processCreditCard** in **any class**@Before("execution(public VerificationResult processCreditCard\*())")![](https://lh5.googleusercontent.com/_W5268rxlZtA7gSXBKE46ZBfKGWHn_LsV1Brwu5LBdGgNANLLRK2hdBiFdV4-3Owrh_D8m_RcUfSgkbIpD_kVODOpAd3JwQSphYMZQYIdAHrYE6ZXknbyJTm9DtiYt40oJfoTdv2HMxLzjlNZqV2uDQ)**


##### Use wildcards on return type


##### ****Example Scenario 4:** Match methods ****with **any return type** and **starting with processCreditCard** in **any class.**@Before("execution(public \* processCreditCard\*())")![](https://lh3.googleusercontent.com/wZP4GBQjH2b31C1a5q17j91VKgw7V_t7Ud6aHsyupL7THr3jywRBEg3d5NQs1lw6BeoIlupUnAqyMEy922aXfXSJ0omG-GEFWkH-hqXIAvfvtyEJyQ6VYGWcwIJ1A1bTGeMAMtXE1Rxopk9xB-9Le4M)Remember? Modifier is optional ... so you don’t have to list itexecution(modifiers-pattern? return-type-pattern declaring-type-pattern? method-name-pattern(param-pattern) throws-pattern?)@Before("execution(\* processCreditCard\*())")![](https://lh4.googleusercontent.com/pTKgrWy9HscYTHSjGolZpHtknXOYMeXQycdwF-BeprN4ZB2owzNF4fBkWeMuieSkHEqzLU-WKQfBd1j-j7QfnmuBm1Uu9VI6F-yvlqu_IudxOe5K2ZSNKoOTfQmx_JWHf2MSCyxxyF8Ii8iWKk7dlk4)**


## AOP Pointcut Expressions - Match Method Parameter Types


##### **execution(modifiers-pattern? return-type-pattern declaring-type-pattern? method-name-pattern(param-pattern) throws-pattern?)**Note**: The pattern is optional if it has “?”For param-pattern- () - matches a method with no arguments
- (\*) - matches a method with one argument of any type
- (..) - matches a method with 0 or more arguments of any type**


### Pointcut Expression Examples


##### ****Example Scenario 5:** Match addAccount methods with **no arguments**@Before("execution(\* addAccount())")![](https://lh6.googleusercontent.com/WecOdQs5-iJz1my9B976L4HeFQZpYqBpGCoz6ZdlzIprdHNu7c8eVQu6mMwswL6tNsUfskNXfONw8A_K87e3HDcmR0eUNTO_Riwmy05knDKuN_L1HYQRo8QyN4dMcho9Cr_jKEwHNOwah24kBVH91Hg)**Example Scenario 6:** Match addAccount methods that **have Account param**@Before("execution(\* addAccount(com.dpauld.aopdemo.Account)))")![](https://lh6.googleusercontent.com/WecOdQs5-iJz1my9B976L4HeFQZpYqBpGCoz6ZdlzIprdHNu7c8eVQu6mMwswL6tNsUfskNXfONw8A_K87e3HDcmR0eUNTO_Riwmy05knDKuN_L1HYQRo8QyN4dMcho9Cr_jKEwHNOwah24kBVH91Hg)**


#### Match on method parameters (using wildcards)


##### ****Example Scenario 6:** Match addAccount methods with any number of arguments@Before("execution(\* addAccount(..)))")**


## ![](https://lh4.googleusercontent.com/_ZIJl1QkjrLqvDNz-Igp0wnbz3SG3fud-GovMN8rBvirdwOQ9E6SJN8DeJs9PJJOf9XoRa0dC_TQ7BFw5Arvm6yGDMdRtMhNOhIy1qc2cZdNcMvP5X6AB5oppGFfmww3fA2UHYrMcCCRM8m6TlOJNiM)Match on Package


### Package - Pointcut Expression Examples


##### ****Example Scenario 6:** Match any method in our **DAO package: com.dpauld.aopdemo.dao**@Before("execution(\* com.dpauld.aopdemo.dao.\*.\*(..)))")![](https://lh4.googleusercontent.com/eFRdHk7YUjGU8Eu5rU6f3Ynk0kx7fZt9zb067VRp3-GaWKvKcoBImdZMq-SAWm-JBb48LIAxVzb6SsGS6pMO0bCugslMZAmIzd9wgtuOj-pFvBjc8lBYjCqTp3odaL6Hxnczn8i6gX8dJS3SceP-UdA)com.dpauld.aopdemo.dao.\* => the star at the end of this indicates any other package or class inside this is also applicable.**


# AOP Pointcut Declarations


##### **[06-spring-aop-pointcut-declarations-overview.pdf](https://drive.google.com/file/d/1A3jBuo0s8mGed2BCQzWsNnuPkz7FtBbe/view?usp=sharing)[07-spring-aop-pointcut-combine-overview.pdf](https://drive.google.com/file/d/1wQeJCDwOaFNZxOZuKZxNI8lD0JSZPz_x/view?usp=share_link)**


# AOP Ordering Aspects


##### **[08-spring-aop-order-aspects.pdf](https://drive.google.com/file/d/1wnU44nx701J1d5x6FAt-MPlwV3t17ZBS/view?usp=sharing)**


# AOP JoinPoints


##### **[09-spring-aop-joinpoints-overview.pdf](https://drive.google.com/file/d/13z1dX_QQDuR9HCMrEOiKLSljuwNdPh2O/view?usp=sharing)[10-spring-aop-reading-joinpoint.pdf](https://drive.google.com/file/d/1AOWFc0goXT9wRxurh9rdPzq9aVAIHolb/view?usp=sharing)[11-spring-aop-progress-check.pdf](https://drive.google.com/file/d/1HtV2zXyv4plycvtcS1UxG4Cf19BQos0p/view?usp=sharing)**


# AOP @AfterReturning Advice Type


##### **[12-spring-aop-after-returning-advice-overview.pdf](https://drive.google.com/file/d/1Hym9gK8YbW4vmKwXVIhDFosQHKoHvUEN/view?usp=sharing)[13-spring-aop-after-returning-code.pdf](https://drive.google.com/file/d/115bZ_PFeFdU_QU83EKnMFZMg_SmybxDs/view?usp=sharing)[14-spring-aop-after-returning-modify-advice-overview.pdf](https://drive.google.com/file/d/1q_008xApLMRNonSM9Cjq-aZXaqSAm9B_/view?usp=sharing)**


# AOP @AfterThrowing Advice Type


##### **[15-spring-aop-after-throwing-advice-overview.pdf](https://drive.google.com/file/d/10Vu-Xns5M8EH-pGcrzeNxZ4WuFLRA_e1/view?usp=sharing)**


# AOP @After Advice Type


##### **[16-spring-aop-after-returning-code.pdf](https://drive.google.com/file/d/14WjBdv7V4psEr6iIAzLwJl1T7H0X9TxU/view?usp=sharing)[17-spring-aop-after-finally-advice-overview.pdf](https://drive.google.com/file/d/1X92GP3YkT4yiaJWR2KGrsA2C00g9vb-U/view?usp=sharing)[18-spring-aop-after-finally-code.pdf](https://drive.google.com/file/d/1A6nu3Yc_EAXJxovN3GO3JZNmrpreRpYj/view?usp=sharing)**


# AOP @Around Advice Type


##### **[19-spring-aop-around-advice-overview.pdf](https://drive.google.com/file/d/1swRduW4JJCYrmBj8oCaVSnGoJHDqtC1W/view?usp=sharing)[20-spring-aop-around-code.pdf](https://drive.google.com/file/d/1mCo6MYgQzYQLc7BDyOENBJ6_eO-9dd50/view?usp=sharing)[21-spring-aop-around-advice-logger-overview.pdf](https://drive.google.com/file/d/1gGnGXZ87DbUSGaqG1v8uRsepgwxHRcI7/view?usp=sharing)[22-spring-aop-around-advice-overview-revisited.pdf](https://drive.google.com/file/d/1AzpjZ1TsvC2WW0WU-p9SCZI3t8h1_EOm/view?usp=sharing)[23-spring-aop-handle-exception-code.pdf](https://drive.google.com/file/d/1tIY0GcldvrPbHeHMXsUPRjxkbwdZim99/view?usp=sharing)[24-spring-aop-around-advice-revisited-rethrow-exception-overview.pdf](https://drive.google.com/file/d/17dzSWHo9kyFf_2R0-ddOsNXOyEOejE4o/view?usp=sharing)**


# AOP Add AOP Logging to Spring MVC App - Real-Time Project


##### **[25-spring-aop-with-spring-mvc-crm-app-overview.pdf](https://drive.google.com/file/d/1-nDjfUla2bhOz_-wIbgEVpul3-SPpWUR/view?usp=sharing)[java - What is the difference between @Before @After and @AfterExecution in Spring aop - Stack Overflow](https://stackoverflow.com/questions/31294698/what-is-the-difference-between-before-after-and-afterexecution-in-spring-aop#:~:text=Before%20Advice%20it%20is%20executed,after%20the%20actual%20method%20call.)[Spring AOP: After or AfterReturning which advice will invoked first - Stack Overflow](https://stackoverflow.com/questions/38202051/spring-aop-after-or-afterreturning-which-advice-will-invoked-first)**


## pointcut expressions


##### **execution(**public** EmployeeDTO EmployeeManager.\*(EmployeeDTO, Integer))within()[Spring aop aspectJ pointcut expression examples - HowToDoInJava](https://howtodoinjava.com/spring-aop/aspectj-pointcut-expressions/)Spring Security[Spring Security - Google Docs](https://docs.google.com/document/d/1uiHiv1au5wOmCTZnYjJpSSSxmmBIc5M4lpf9NXw6LYY/edit#heading=h.4nn9olbs7glb)JPA<https://stackoverflow.com/a/4477349/4212710>Spring Annotation- @Compoent

  - @Component is an annotation that allows Spring to detect our custom beans automatically. In other words, without having to write any explicit code, Spring will:

    - Scan our application for classes annotated with @Component thus detecting our custom beans
    - Instantiate them and inject any specified dependencies into them
    - Inject them wherever needed

  - However, most developers prefer to use more specialized stereotype annotations to serve this function. Spring has provided a few specialized stereotype annotations: @Controller, @Service and @Repository. They all provide the same function as @Component. [Source](https://www.baeldung.com/spring-component-annotation#:~:text=3.%20%40Component,Spring%20Boot%20project%3A)

- @Autowired 

- @Value 

- @RequestMapping

- @Valid 

- @BindingResults

- @ModelAttribute

  - **@ModelAttribute is an annotation that binds a method parameter or method return value to a named model attribute, and then exposes it to a web view**, explanation: since the form has the same modelAttribute name(here "student") as the controller Model object's attribute, any changes in the form that will change the student object will also reflect the change in the theStudent parameter here in the controller method.@**ModelAttribute** and @**RequestParam** are for decoding query parameters from URL. The only difference is @**ModelAttribute** will bind all the fields and give a full object. But if @RequestParam is used then you have to build the entire object by mapping all the fields manually. It is used for binding data from request param (in key value pairs).In thee example ModelAttribute binded student model with the theStudent object. So we get the theStudent object filled with values without any extra build up codes.public String processForm(@ModelAttribute("student") Student theStudent) { System.out.println("Full name: " + theStudent.getFirstName() + " " + theStudent.getLastName());return "student-confirmation"; }On the other hand the annotation is used to define objects which should be part of a Model. So if you want to have a Person object referenced in the Model you can use the following method:@ModelAttribute("person")public Person getPerson(){    return new Person();}This annotated method will allow access to the Person object in your View, since it gets automatically added to the Models by Spring.See "Using @ModelAttribute".<https://stackoverflow.com/a/14616749>- [@RequestParam vs @ModelAttribute](https://stackoverflow.com/questions/29370581/spring-mvc-please-explain-difference-between-requestparam-and-modelattribute)@**ModelAttribute** and @**RequestParam** are for decoding query parameters from URL. The only difference is @**ModelAttribute** will bind all the fields and give a full object. But if @RequestParam is used then you have to build the entire object by mapping all the fields manually. It is used for binding data from request param (in key value pairs).- **@RequestBody vs** @**ResponseBody** @RequestBody specifies the body of the request . It is used for binding data from the whole body of the requests like POST,PUT. On the other hand, @ResponseBody specifies the body of the Response. It is mostly used when designing REST apis with Spring boot.[**@requestbody alternative**](https://stackoverflow.com/questions/7476372/alternative-of-requestbody)**:**Take a parameter of **HttpServletRequest**, and read the **ServletInputStream** using **getInputStream()** from there. The stream will contain the body of the request.@Controllerpublic class MyController {    @RequestMapping("/test")    public String aTest(HttpServletRequest request) {        InputStream body = request.getInputStream();        //process request body        return myReturnVal;    }}- **Next****AFAQ**1. [java - Spring: @Value vs. @Autowired - Stack Overflow](https://stackoverflow.com/questions/29551761/spring-value-vs-autowired)
2. [How Does Spring use @RequestMapping("/showForm") annotation to get to the controller method showForm() and ultimately get the view page?](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.j0ql7pu9v7bw)
3.JSP [Expression Language (oracle.com)](https://docs.oracle.com/javaee/1.4/tutorial/doc/JSPIntro7.html) \| [The J2EE(TM) 1.4 Tutorial (oracle.com)](https://docs.oracle.com/javaee/1.4/tutorial/doc/index.html)_JavaServer Page_ (JSP) is Java's answer to Microsoft's _Active Server Pages_ (ASP). 1. A **JSP script is a regular HTML page containing Java programs**. Recall that JSP is "_Java inside HTML_" (whereas [**servlet** ](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.wh95kdbv7q54)is "_HTML inside Java_"). The Java statements are enclosed by &lt;% ... %> (called _JSP scriptlet_) or &lt;%= ... %> (called _JSP expression_).
2. _JSP Scriptlet_ &lt;% code fragment %> is used to include Java statements.
3. _JSP Directives_ &lt;%@ directive attribute="value" %> are the elements that supply/relay directions and instructions to the container and affect how it compiles the JSP page. These special instructions are used for translating JSP to corresponding servlet code.**


# JSP


### First JSP Example - "Java inside HTML"


##### **📂first.jsp|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%@ page language="java" contentType="text/html; charset=ISO-8859-1"    pageEncoding="ISO-8859-1"%>&lt;!DOCTYPE html>&lt;html> &lt;head>&lt;title>First JSP&lt;/title>&lt;/head> &lt;body>   &lt;%     double num = Math.random();     if (num > 0.95) {   %>       &lt;h2>You'll have a luck day!&lt;/h2>&lt;p>(&lt;%= num %>)&lt;/p>   &lt;%     } else {   %>       &lt;h2>Well, life goes on ... &lt;/h2>&lt;p>(&lt;%= num %>)&lt;/p>   &lt;%     }   %>   &lt;a href="&lt;%= request.getRequestURI() %>">&lt;h3>Try Again&lt;/h3>&lt;/a> &lt;/body> |To execute the JSP script: Simply start your Tomcat server and use a browser to issue an URL to browse the JSP page (i.e., http&#x3A;//localhost:8080/hello/first.jsp).From your browser, choose the "View Source" option to check the response message. It should be either of the following depending on the random number generated.|                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;html> &lt;h2>You'll have a luck day!&lt;/h2> &lt;p>(0.987)&lt;/p> &lt;a href="first.jsp">&lt;h3>Try Again&lt;/h3>&lt;/a> &lt;/html> |or|                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;html> &lt;h2> Well, life goes on ... &lt;/h2> &lt;p>(0.501)&lt;/p> &lt;a href="first.jsp">&lt;h3>Try Again&lt;/h3>&lt;/a> &lt;/html> |Source: [Getting Starting with JSP with Examples (ntu.edu.sg)](https://www3.ntu.edu.sg/home/ehchua/programming/java/JSPByExample.html)**


## JSP Scripting elements - [JSP Scripting elements](https://docs.oracle.com/cd/B14099_19/web.1012/b14014/genlovw.htm#sthref37)


##### **JSP Scriptlet &lt;% code fragment %> is used to include Java statements. These elements are used to include java codes such as declarations, expressions, scriptlets, and comments. **


## Objects and scopes - [_Objects_ and _scopes_](https://docs.oracle.com/cd/B14099_19/web.1012/b14014/genlovw.htm#sthref51)


##### **JSP objects can be created either explicitly or implicitly and are accessible within a given scope, such as from anywhere in the JSP page or the session.**


## JSP Directives


##### **JSP Directives are the elements that supply/relay directions and instructions to the container and affect how it compiles the JSP page. These special instructions are used for translating JSP to corresponding servlet code.Syntax:&lt;%@ directive attribute = "value" %>Directives can have a number of attributes which you can list down as key-value pairs and separated by commas.There are three types of directive tag −1. page directive, &lt;%@ page attribute = "value" %>
2. include directive,  &lt;%@ include file = "relative url" >
3. taglib directive, &lt;%@ taglib uri="uri" prefix = "prefixOfTag" >**


### Page Directive


##### **Defines page-dependent attributes, such as scripting language, error page, and buffering requirements.The page directive is used to provide instructions to the container. These instructions pertain to the current JSP page. You may code page directives anywhere in your JSP page. By convention, page directives are coded at the top of the JSP page.The taglib directive follows the syntax given below −&lt;%@ page attribute = "value" %>Example:|                                                                                                                                                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;%@ page language="java" contentType="text/html; charset=ISO-8859-1"     pageEncoding="ISO-8859-1"%> &lt;!DOCTYPE html> &lt;html> &lt;head> &lt;meta charset="ISO-8859-1"> &lt;title>Insert title here&lt;/title> &lt;/head> &lt;body> &lt;h1>Welcome to main menu&lt;/h1> &lt;/body> &lt;/html> |**


### Include directive


##### **Includes a file during the translation phase.The include directive is used to include a file during the translation phase. This directive tells the container to merge the content of other external files with the current JSP during the translation phase. You may code the include directives anywhere in your JSP page.The include directive follows the syntax given below −&lt;%@ include file = "relative url" >For more details with examples, check the [Include Directive.](https://www.tutorialspoint.com/jsp/include_directive.htm)**


### Taglib directive


##### **Declares a tag library, containing custom actions, used in the pageThe JavaServer Pages API allows you to define custom JSP tags that look like HTML or XML tags and a tag library is a set of user-defined tags that implement custom behavior.The taglib directive declares that your JSP page uses a set of custom tags, identifies the location of the library, and provides means for identifying the custom tags in your JSP page.The taglib directive follows the syntax given below −&lt;%@ taglib uri="uri" prefix = "prefixOfTag" >For more details with examples, check the [Taglib Directive](https://www.tutorialspoint.com/jsp/taglib_directive.htm).**


## JSP Action


##### ****The &lt;jsp:include> standard action:**&lt;jsp:include page="header.jsp" />Dynamic: adds the content from the value of the page attribute to the current page at request time. Was intended more for dynamic content coming from JSPs.**


## AFAQ


##### **- What is the difference between &lt;jsp:include page = ... > and &lt;%@ include file = ... >? Or What's the difference between including files with JSP include directive, JSP include action and using JSP Tag Files?

  - [What's the difference between including files with JSP include directive, JSP include action and using JSP Tag Files? - Stack Overflow](https://stackoverflow.com/a/14763794) \*\*\*\*\*\*
  - [What is the difference between &lt;jsp:include page = ... > and &lt;%@ include file = ... >? - Stack Overflow](https://stackoverflow.com/questions/7879906/what-is-the-difference-between-jspinclude-page-and-include-file)
  - ![](https://lh6.googleusercontent.com/EJZd2QS0kpO92shCs_MzaakFxOzM18Gw06uRCJ71ILCUqBp66ibrFlD3QRyqbi2cM2aTM91D22eIRVwzeK0antVOUxBq4kBYxzMDh9a8alU-cciizeEuPsi6yohZ_oG-Vpa6D7Dr7mcXE8AzT9zYSjw)**


## JSP - Standard Tag Library (JSTL)


##### **- [JSP - Standard Tag Library (JSTL) Tutorial (tutorialspoint.com)](https://www.tutorialspoint.com/jsp/jsp_standard_tag_library.htm#:~:text=The%20JavaServer%20Pages%20Standard%20Tag,internationalization%20tags%2C%20and%20SQL%20tags.)
- [JSTL Tutorial and Examples - javatpoint](https://www.javatpoint.com/jstl)Read More:1. [Learn JSP Tutorial - javatpoint](https://www.javatpoint.com/jsp-tutorial)
2. [JSP - Syntax (tutorialspoint.com)](https://www.tutorialspoint.com/jsp/jsp_syntax.htm) \*\*\*\*\***


## Expression Language(EL) used in JSP


##### **[Expression Language (javaee.github.io)](https://javaee.github.io/tutorial/jsf-el.html)XML[XML Schema Part 0: Primer Second Edition (w3.org)](https://www.w3.org/TR/xmlschema-0/)[Namespaces in XML 1.0 (Third Edition) (w3.org)](https://www.w3.org/TR/REC-xml-names/)**


# A Reference to an XML Schema


##### ****AFAQ** 1. How does Java works with XML file?

   1. [How to Read XML File in Java - Javatpoint](https://www.javatpoint.com/how-to-read-xml-file-in-java)**


#### This XML document has a reference to an XML Schema:


##### **&lt;?xml version="1.0"?>&lt;notexmlns="https&#x3A;//www.w3schools.com"xmlns:xsi="http&#x3A;//www.w3.org/2001/XMLSchema-instance"xsi:schemaLocation="https&#x3A;//www.w3schools.com/xml note.xsd">  &lt;to>Tove&lt;/to>  &lt;from>Jani&lt;/from>  &lt;heading>Reminder&lt;/heading>  &lt;body>Don't forget me this weekend!&lt;/body>&lt;/note>**Source:** [XML Schema How To?](https://www.w3schools.com/xml/schema_howto.asp#:~:text=A%20Reference%20to%20an,%3C/note%3E)For the following XML fragment:&lt;projectxmlns="http&#x3A;//maven.apache.org/POM/4.0.0"xmlns:xsi="http&#x3A;//www.w3.org/2001/XMLSchema-instance"xsi:schemaLocation="http&#x3A;//maven.apache.org/POM/4.0.0http&#x3A;//maven.apache.org/xsd/maven-4.0.0.xsd">A single `xmlns` is used to define the default namespace for the document (The first xmlns=""). Any element in the document without explicit namespace prefix will be in the default namespace. xmlns:xxx will define a non-default namespace, which must be explicitly prefixed to an element when using. Note: Also note that a default namespace is not mandatory; Icould instead declare a namespace prefix for http&#x3A;//maven.apache.org/POM/4.0.0 and use it explicitly.These answers in the this question clears a lot of things: 1. [xml - xmlns, xmlns:xsi, xsi:schemaLocation, and targetNamespace? - Stack Overflow](https://stackoverflow.com/questions/34202967/xmlns-xmlnsxsi-xsischemalocation-and-targetnamespace)
2. [What exactly is the purpose of the URL in an XML namespace? - Stack Overflow](https://stackoverflow.com/questions/57125057/what-exactly-is-the-purpose-of-the-url-in-an-xml-namespace)
3. [java - How do XML namespaces work without a working network connection? - Stack Overflow](https://stackoverflow.com/questions/8863233/how-do-xml-namespaces-work-without-a-working-network-connection)
4. [Why are URLs in XML namespaces? - Stack Overflow](https://stackoverflow.com/questions/5758041/why-are-urls-in-xml-namespaces)
5. [Spring bean configuration xml - Stack Overflow](https://stackoverflow.com/questions/27289559/spring-bean-configuration-xml)[XSD - &lt;schema> element](https://www.w3schools.com/xml/schema_schema.asp)Now lets understand Spring Configuration xml1. Green colored section: &lt;beans>&lt;/bean> is the root element and has the attributes of namespaces. xmlns=_"uri"_ defines the default namespace and others are explicit namespace. Xmlns:xsi => [Schema-Related Markup in Documents Being Validated](https://www.w3.org/TR/xmlschema-1/#Instance_Document_Constructions).Any elements coming from xmlns:tx namespace should be prefixed with tx. Any elements coming from xmlns:context namespace should be prefixed with context. 

   1. **AFAQ**: How did we not use tx:schemalocation?

2. Blue colored section: Here we use context prefix to use the element component-scan of context namespace.

3. Purple Colored section: here we used the element &lt;bean> of default namespcae.

4. Magenta Colored Section: here we used the element annotation-driven of tx namespace.&lt;?xml version=_"1.0"_ encoding=_"UTF-8"_?>&lt;beans xmlns=_"http&#x3A;//www.springframework.org/schema/beans"_    xmlns:xsi=_"http&#x3A;//www.w3.org/2001/XMLSchema-instance"_    xmlns:context=_"http&#x3A;//www.springframework.org/schema/context"_    xmlns:tx=_"http&#x3A;//www.springframework.org/schema/tx"_    xmlns:mvc=_"http&#x3A;//www.springframework.org/schema/mvc"_    xsi:schemaLocation=_"_      _____http&#x3A;//www.springframework.org/schema/beans_      _____http&#x3A;//www.springframework.org/schema/beans/spring-beans.xsd_      _____http&#x3A;//www.springframework.org/schema/context_      _____http&#x3A;//www.springframework.org/schema/context/spring-context.xsd_      _____http&#x3A;//www.springframework.org/schema/mvc_      _____http&#x3A;//www.springframework.org/schema/mvc/spring-mvc.xsd_      _____http&#x3A;//www.springframework.org/schema/tx_      _____http&#x3A;//www.springframework.org/schema/tx/spring-tx.xsd"_>     &lt;!-- Add support for component scanning -->    &lt;context:component-scan base-package=_"com.dpauld.springdemo"_ />     &lt;!-- Add support for conversion, formatting and validation support -->    &lt;mvc:annotation-driven/>       &lt;!-- Define Spring MVC view resolver -->    &lt;bean        class=_"org.springframework.web.servlet.view.InternalResourceViewResolver"_>      &lt;property name=_"prefix"_ value=_"/WEB-INF/view/"_ />      &lt;property name=_"suffix"_ value=_".jsp"_ />    &lt;/bean>     &lt;!-- Step 1: Define Database DataSource / connection pool -->    &lt;bean id=_"myDataSource"_ class=_"com.mchange.v2.c3p0.ComboPooledDataSource"_    destroy-method=_"close"_>   &lt;property name=_"driverClass"_ value=_"com.mysql.cj.jdbc.Driver"_ />   &lt;!-- &lt;property name="jdbcUrl" value="jdbc:mysql://localhost:3306/web_customer_tracker?useSSL=false&amp;amp;serverTimezone=UTC" />  -->   &lt;!-- &lt;property name="user" value="springstudent" /> -->   &lt;!--  &lt;property name="password" value="springstudent" />  -->     &lt;!-- Alternative Hosting Provider MySQL -->           &lt;property name=_"jdbcUrl"_ value=_"jdbc:mysql://aws.connect.psdb.cloud/web_customer_tracker?sslMode=VERIFY_IDENTITY"_ />   &lt;property name=_"user"_ value=_"e216vcfelvsojo0pkal8"_ />   &lt;property name=_"password"_ value=_"pscale_pw_p3KX4VI1bzcpKMvF785GSd4WbB5E5Z39vYcLbTdeLdV"_ />             &lt;!-- these are connection pool properties for C3P0 -->      &lt;property name=_"initialPoolSize"_ value=_"5"_/>   &lt;property name=_"minPoolSize"_ value=_"5"_ />   &lt;property name=_"maxPoolSize"_ value=_"20"_ />   &lt;property name=_"maxIdleTime"_ value=_"30000"_ />    &lt;/bean>       &lt;!-- Step 2: Setup Hibernate session factory -->    &lt;bean id=_"sessionFactory"_      class=_"org.springframework.orm.hibernate5.LocalSessionFactoryBean"_>      &lt;property name=_"dataSource"_ ref=_"myDataSource"_ />      &lt;property name=_"packagesToScan"_ value=_"com.dpauld.springdemo.entity"_ />      &lt;property name=_"hibernateProperties"_>         &lt;props>            &lt;prop key=_"hibernate.dialect"_>org.hibernate.dialect.MySQLDialect&lt;/prop>            &lt;prop key=_"hibernate.show_sql"_>true&lt;/prop>         &lt;/props>      &lt;/property>   &lt;/bean>      &lt;!-- Step 3: Setup Hibernate transaction manager -->    &lt;bean id=_"myTransactionManager"_       class=_"org.springframework.orm.hibernate5.HibernateTransactionManager"_>   &lt;property name=_"sessionFactory"_ ref=_"sessionFactory"_/>    &lt;/bean>       &lt;!-- Step 4: Enable configuration of transactional behavior based on annotations -->    &lt;tx:annotation-driven transaction-manager=_"myTransactionManager"_ />     &lt;!-- Add support for reading web resources: css, images, js, etc ... -->    &lt;mvc:resources location=_"/resources/"_ mapping=_"/resources/\*\*"_>&lt;/mvc:resources>       &lt;/beans>Must Known Spring Boot Annotations- Bean
- @Service
- @Repository
- @Configuration
- @Controller
- @RequestMapping
- @Autowired
- @Value
- @Component
- @SpringBootApplicationSpecialized1. Repository
2. TransactionalRead more: [Spring Boot Annotations Everyone Should Know \[2023\] | upGrad blog](https://www.upgrad.com/blog/spring-boot-annotations/)Servlet and/vs CGI**


# Servlet


##### **Simply put, a Servlet is a class that handles requests, processes them and replies back with a response.For example, we can use a Servlet to collect input from a user through an HTML form, query records from a database, and create web pages dynamically.Servlets are under the control of another Java application called a Servlet Container. When an application running in a web server receives a request, the Server hands the request to the Servlet Container – which in turn passes it to the target Servlet.\_\_\_\_\_Today we all are aware of the need of creating dynamic web pages i.e the ones which have the capability to change the site contents according to the time or are able to generate the contents according to the request received by the client. If you like coding in Java, then you will be happy to know that using Java there also exists a way to generate dynamic web pages and that way is **Java Servlet**. But before we move forward with our topic let’s first understand the need for server-side extensions. Servlet technology is used to create a web application (resides at server side and generates a dynamic web page). Servlets are the Java programs that run on the Java-enabled web server or application server. They are used to handle the request obtained from the web server, process the request, produce the response, then send a response back to the web server.Servlet technology is robust and scalable because of the Java language. Before Servlet, [CGI ](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.3454cvu922je)(Common Gateway Interface) scripting language was common as a server-side programming language. However, there were many disadvantages to this technology. We have discussed these disadvantages below.There are many interfaces and classes in the Servlet API such as Servlet, GenericServlet, HttpServlet, ServletRequest, ServletResponse, etc.Properties of Servlets are as follows:- Servlets work on the server-side.
- Servlets are capable of handling complex requests obtained from the web server.Read this at last, [Introduction to Java Servlets | Baeldung](https://www.baeldung.com/intro-to-servlets)Sources: [Introduction to Java Servlets - GeeksforGeeks](https://www.geeksforgeeks.org/introduction-java-servlets/)[Learn Servlet Tutorial - javatpoint](https://www.javatpoint.com/servlet-tutorial)**Important**: To Understand Servlet, [Create a Web Service using Servlet - YouTube](https://www.youtube.com/watch?v=0L9yTE_zFM0&ab_channel=CodeTips)Read Stackoverflow Answers1. [java - Servlet Mapping using web.xml - Stack Overflow](https://stackoverflow.com/questions/8198312/servlet-mapping-using-web-xml)
2. [java - How are Servlet url mappings in web.xml used? - Stack Overflow](https://stackoverflow.com/questions/15385596/how-are-servlet-url-mappings-in-web-xml-used)
3.**


# CGI


##### **Read  [Long Story Short](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.w3c44tmer6ec) at first, describing in what situation CGI was created.A real-life example: a complicated database that needs to be shown on a website. Since the database was designed somewhere around 1986 (!), lots of data was packed in different ways to save on disk space.As the development went on, the developers could no longer solve complicated data requests in SQL alone, for example because the sorting algorithms were unusual.There are three sensible solutions:1. quick and dirty: send the unsorted data to PHP, sort it there. Obviously a very expensive solution, because this would be repeated every time the page is called
2. write a plugin to the database engine -- but the admin wasn't ready to allow foreign code to run on their server, or
3. you can process the data in a program (C, Perl, etc.), and output HTML. The program itself goes into /cgi-bin, and is called by the web server (e.g. Apache) directly, not through PHP.CGI runs your script in Solution #3 and outputs the effect to the browser. You have the speed of the compiled program, the flexibility of a language broader than SQL, and no need to write plugins to the SQL server. (Again, this is an example specific to SQL and C)—--**Another example**: Let’s suppose, for example, that your server is running under MS DOS. Well, in real life none of them do, but there are Windows servers, and Windows can handle MS DOS commands.Now, let us say you would like to send the listing of your current directory to the web (not a good idea, but it shows just how simple it is). Well, MS DOS has the dir command that sends the directory listing to standard output.**How does The Output is Send Back to the Browser Client and What about the two steps?**True, dir will not explain it is sending plain text before sending it. But never fear! You can write a batch file like this:   echo Content-type: text/plain   echo.   dirThe first line of this batch file tells the browser to expect plain text. The second sends a blank line. The third lists the contents of the current directory.—--An amazing tutorial ["CGI Programming Is Simple!" - CGI Tutorial](http://www.whizkidtech.redprince.net/cgi-bin/tutorial), which explains the concepts in the simplest possible way. After reading this article you may want to read [Getting Started with CGI Programming in C](http://www.cs.tut.fi/~jkorpela/forms/cgic.html) or [Getting Started with CGI Programming in C (iitb.ac.in)](https://www.cse.iitb.ac.in/~cs406/old/assignment2/03329023_2/cgic.html) to supplement your understanding with actual code samples. The CGI is specified in [RFC 3875](http://www.ietf.org/rfc/rfc3875.txt) [Mirror](https://www.rfc-editor.org/rfc/rfc3875).**


## Long Story Short


##### **The CGI is specified in [RFC 3875](http://www.ietf.org/rfc/rfc3875.txt), though that is a later "official" codification of the original [NCSA document](http://hoohoo.ncsa.uiuc.edu/cgi/). Basically, CGI is an interface specification that defines a protocol(define other things as well) to pass data about a HTTP request from a web server to an executable program to process - any program, in any language. It can be seen as an interface specification between a web server (HTTP server) and an executable program. **Story:** At the time the spec was written (1993), most web servers contained only static pages, "web apps" were a rare and new thing, so it seemed natural to keep them apart from the "normal'' static content, such as in a cgi-bin directory apart from the static content, and having them end in .cgi. At this time, there also were no dedicated "web programming languages" like PHP, and C was the dominating portable programming language - so many people wrote their CGI scripts in C. But Perl quickly turned out to be a better fit for this kind of thing, and CGI became almost synonymous with Perl for a while. Then there came Java Servlets, PHP and a bunch of others and took over large parts of Perl's market share.HTTP request is sent by a client and the web server uses an interface called as CGI which defines protocol to pass data(includes stdin, environment variables, content type, length etc) about the HTTP request to an executable program that processes the data and send the response according to the CGI protocol. It describes how certain properties of that request should be communicated to the environment of that program and how the program should communicate the response back to the server and how the server should 'complete' the response to form a valid reply to the original HTTP request.CGI is an interface which tells the web server how to pass data to and from an application. More specifically, it describes how request information is passed in environment variables (such as request type, remote IP address), how the request body is passed in via standard input, and how the response is passed out via standard output. You can refer to the CGI specification for details.To use your image:**_user (client) request for page_** _--->_ **_webserver_** _---_**_\[CGI] (It can be a script, called as CGI Script)_**_---->_ **_Server side Program(Also called as CGI program)_** _---> MySQL Server or Do other things._Source: [What is Common Gateway Interface (CGI)? - Stack Overflow](https://stackoverflow.com/questions/2089271/what-is-common-gateway-interface-cgi)**


# DispatcherServlet


##### **<https://www.baeldung.com/spring-boot-dispatcherservlet-web-xml>The DispatcherServlet is an actual Servlet (it inherits from the HttpServlet base class) in Spring, instead of using the typical Servlet they Implemented their own version named DispatcherServlet. In a traditional Spring web application, this servlet is defined in the web.xml file. You need to map requests that you want the DispatcherServlet to handle, by using a URL mapping in the same web.xml file. DispatcherServlet is used to create web applications and REST services in Spring MVC.Eclipse **


# Tomcat Server


## FAQ - ETS


##### **1. Starting Tomcat v9.0 Server at localhost has encountered a problem. The server cannot be started because one or more of the ports are invalid. Open the server editor and correct invalid ports. [Source](https://stackoverflow.com/questions/59549059/the-server-cannot-started-because-one-or-more-of-the-ports-are-invalid-tomcat-i)

   1. _Answer_: The issue is that the Tomcat admin port was not defined. You need to have it as an actual number such as 9000 rather than as a hyphen -. To change it Go to Eclipse => Window => Show View => Servers => DoubleClick on Tomcat Server => Change admin port to "1" 

   2. leave the HTTP port to "8080"

   3. **Make sure to kill any processes which are running on port 8080**.You will find your project on localhost:8080/java project name , if you don't add java project name it will give you error 404. Hope this works ! However u can check which process is running on port 8080 by going _Resource Monitor => Network => Listening Ports => find port 8080 from the table_. To kill the process do this,

      1. Option 01 - npx kill-port 8080

      2. Option 02 - Most commonly used

         1. Step 01: Open Windows command prompt as Administrator
         2. Step 02: Find the PID of the port you want to kill with the below command:netstat -ano|findstr "PID :8080"TCP 0.0.0.0:8080 0.0.0.0:0 LISTENING 182643. Step 03: Kill the PID you received above with the below command (In my case PID is 18264): taskkill /PID 18264 /f2. Server configuration is missing in Eclipse

   1. Probably, you have some problems with your server's configuration. Follow these steps to remove and create a new one, it might help you. In Eclipse

      1. 1\. Window -> Show view -> Servers (If you cannot see it, you might need to choose Others -> Server)
      2. 2\. From Server view -> Delete the server which has problems.
      3. 3\. Right click -> New -> Server : to create a new oneIn my case, after new server was created, I get rid of this "localhost-config is missing"2.Have Spring package directory in a single line:[Eclipse: how to make directory trees show as packages - Stack Overflow](https://stackoverflow.com/questions/4559350/eclipse-how-to-make-directory-trees-show-as-packages#:~:text=In%20the%20Package%20Explorer%2C%20right,Build%20Path%20/%20Exclude.)Question and Explanation related with Spring topic**


##### How Does Spring use @RequestMapping("/showForm") annotation to get to the controller method showForm() and ultimately get the view page?


##### **1.|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @Controller public class HomeController { @RequestMapping("/") public String showPage() { // this method is only returning the view page name as a string. Internally Spring will add suffix and prefixes using this name and then show the page to the user. return "main-menu"; } @RequestMapping("/showForm") public String showForm() { return "helloworld-form"; } @RequestMapping("/processForm") public String processForm() { return "helloworld"; } @RequestMapping("/processFormVersionTwo") public String processFormVT(HttpServletRequest r, Model m) { String theName = r.getParameter("studentName"); System.out.println(theName); String result = "Yo " + theName.toUpperCase(); m.addAttribute("message",result); System.out.println(result); return "helloworld"; } } |This could be explained like: since @Controller inherited @Component annotation↓.How?|                                                                                             |
| ------------------------------------------------------------------------------------------- |
| @Component  public @interface MyControllers{} @MyControllers public class HomeController{ } |Then adding the component scan tag in the xml file will enable the program to scan the HomeController component and put it in the register for future use. Then when the spring server runs the program spring will pick the HomeController component then create an instance variable of HomeController class like  behind the scene, like,|                                               |
| --------------------------------------------- |
| **HomeController hc = new HomeController();** |_Or equivalent when using full xml_|                                                                             |
| --------------------------------------------------------------------------- |
| HomeController hc = context.getBean("homeController",HomeController.class); |After this point Spring can access all the methods of **hc** object and use them. Now Spring will also use the metadata “/showform” or anything else provided by @RequestMapping(“/showform”) annotation and compare it to requested url, and if the url and metadata matches Spring will call the showForm() method to get the view page name. And then it can use this String of view page name to access the view page.**


##### When to use ApplicationContext to manually create a context and when to use WebApplicationContext for auto creation?


##### **2. 1. [ApplicationContext and WebApplicationContext in Spring MVC - GeeksforGeeks](https://www.geeksforgeeks.org/webapplicationcontext-in-spring-mvc/#:~:text=Difference%20Between%20ApplicationContext,this%20working%20flow)
3. [java - Why is Spring's ApplicationContext.getBean considered bad? - Stack Overflow](https://stackoverflow.com/questions/812415/why-is-springs-applicationcontext-getbean-considered-bad)**


##### When to use xml and when not to? Do we need xml configuration every time?


##### **2.**


##### [Is it mandatory to have hibernate.cfg.xml file for configuration - Stack Overflow](https://stackoverflow.com/questions/8830357/is-it-mandatory-to-have-hibernate-cfg-xml-file-for-configuration#:~:text=Basically%20you%20are%20setting%20all,the%20configure()%20method%20does.&text=Save%20this%20answer.,-Show%20activity%20on)


##### **2. 1.**


##### What do we do by defining a bean in a xml config file?


##### **2. 1. Normal programming case: The fact is we can define a class then inject/set values of different attributes(members of the class) in many ways

      1. by calling the constructor during the creation of object
      2. By calling the set methods
      3. Or by some other ways.

   2. Xml case: in xml we can inject values of the attributes of the class(objects are called bean in spring) defining a bean with bean tag and passing values inside it. One thing to notice is the class itself is already defined, all we are doing is injecting values or objects with the xml file. When we execute the main method, the application looks for the xml file to inject the values using xml and then uses an object of that class/bean. Once we have the object we can change the values of the attribute from the main method. **The xml is used for initial injection.**

   3. Doing the xml thing in java: we can use pure java to do the same thing following the bean definition and di conventions and rules.**


##### How does the Request Parameter work? What is Request parameter? 


##### **2. 1. [How are parameters sent in an HTTP POST request? - Stack Overflow](https://stackoverflow.com/questions/14551194/how-are-parameters-sent-in-an-http-post-request)
   2. In an **HTTP GET request**, parameters are sent as a **query string**:[_http://example.com/page?parameter=value&also=another_](http://example.com/page?parameter=value&also=another)3. In an **HTTP POST request**, the parameters are sent in the **request body**.POST /path/script.cgi HTTP/1.0From: frog@jmarshall.comUser-Agent: HTTPTool/1.0Content-Type: application/x-www-form-urlencodedContent-Length: 32home=Cosby&favorite+flavor=flies**


##### [How to get the GET request query string with url in Spring?](https://stackoverflow.com/questions/16675191/get-full-url-and-query-string-in-servlet-for-both-http-and-https-requests)


##### **7.@GetMapping("/deleteCustomer")  **public** String deleteCustomer(@RequestParam("customerId") **int** theCustomerId, Model theModel, HttpServletRequest request) {        String uri = request.getScheme() + "://" + // "http" + "://                  request.getServerName() + // "localhost"                  ":" + // ":"                  request.getServerPort() + // "8080"                  request.getRequestURI() + // "web-customer-tracker/customer/deleteCustomercustomer"                  "?" + // "?"                  request.getQueryString(); // "Id=15"         System.**_out_**.println(uri);        customerService.deleteCustomer(theCustomerId);        **return** "redirect:/customer/list";  }Output: http&#x3A;//localhost:8080/web-customer-tracker/customer/deleteCustomer?customerId=16**


##### How to get the request body of a POST request?


##### **8.@PostMapping("/saveCustomer")  **public** String saveCustomer (@ModelAttribute("customer") Customer theCustomer, HttpServletRequest request, Model theModel) {        **try** {             System.**_out_**.println(request.getInputStream());        } **catch** (IOException e) {             // **TODO** Auto-generated catch block             e.printStackTrace();        }// add HttpServletRequest request as a parameter in this controller method to use this line        customerService.saveCustomer(theCustomer);        **return** "redirect:/customer/list";  }Output: org.apache.catalina.connector.CoyoteInputStream@7dec1ea4**


##### Next


##### **9.**


## Frequently faced errors and mistakes


##### ****Spring + Hibernate**1. org.springframework.web.servlet.dispatcherservlet **no handler found** 

   1. The reason could be that the **package name** mentioned in the **.xml config** file for component scan is **incorrect**.

2. java.sql.SQLSyntaxErrorException: **Unknown column 'customer0\_.lastName' in 'field list'** 

   1. Most probably the value of the name parameter for say, column_name at @Column(name="column_name") is different from the name given in the mysql database. It has to match with the database column name. Entity class member name could be anything but the column_name must be the same with the database. In this case using **'last_name'** instead of **'lastName'** solves the issue.

3. javax.servlet.jsp.PageContext cannot be resolved to a type

   1. Make sure to Add **servlet-api** dependency and jsp-api dependency, this might solve the issue.

   2. **Alternative** approach

      1. Right click on project and go to properties
      2. Click over Targeted Runtimes
      3.  Check the mark server you are using. For example, "Apache Tomcat v8.0"

4. org.hibernate.HibernateException: Could not obtain transaction-synchronized Session for current thread

   1. Probably @Transactional annotation is missing in service layer

5.Spring Project1. <https://youtu.be/DYMj8B3cVZI?list=PL5mjp3QjkuoKZ0CKox-o0ag9WAft7m_kc>
2.Web and InternetHTTPS and URL: [What is the meaning of '://' after http or https in an internet url? E.g., https://www.quora.com - Quora](https://www.quora.com/What-is-the-meaning-of-after-http-or-https-in-an-internet-url-E-g-https-www-quora-com)**


# REST API


##### **[rest - How to understand "RESTful API is stateless"? - Stack Overflow](https://stackoverflow.com/questions/34130036/how-to-understand-restful-api-is-stateless)Software Development[object oriented - What really is the "business logic"? - Software Engineering Stack Exchange](https://softwareengineering.stackexchange.com/questions/234251/what-really-is-the-business-logic)[Interactive Refactoring Course: Dive Into Refactoring + Design Pattern](https://refactoring.guru/refactoring/course)**


# Design Pattern


## Books


##### **1. [Head First Design Patterns: Building Extensible and Maintainable Object-Oriented Software 2nd Edition: Freeman, Eric, Robson, Elisabeth: 9781492078005: Amazon.com: Books](https://www.amazon.com/Head-First-Design-Patterns-Object-Oriented-dp-149207800X/dp/149207800X/ref=dp_ob_title_bk)
2. Gang of Four(GOF) - [Design Patterns: Elements of Reusable Object-Oriented Software: Erich Gamma, Richard Helm, Ralph Johnson, John Vlissides, Grady Booch: 8601419047741: Amazon.com: Books](https://www.amazon.com/dp/0201633612)
3. Companion of GOF - [The Design Patterns Smalltalk Companion: Alpert, Sherman, Brown, Kyle, Woolf, Bobby: 9780201184624: Amazon.com: Books](https://www.amazon.com/Design-Patterns-Smalltalk-Companion/dp/0201184621#customerReviews)**


## Structural Patterns


### Proxy Pattern


##### **[Proxy Pattern | Object Oriented Design (oodesign.com)](https://www.oodesign.com/proxy-pattern)**


## DTO(Data transfer object) pattern


##### **[model view controller - What is a Data Transfer Object (DTO)? - Stack Overflow](https://stackoverflow.com/a/1058186/7828981)DTOs or Data Transfer Objects are objects that carry data between processes in order to reduce the number of method calls. Read more [The DTO Pattern (Data Transfer Object) | Baeldung](https://www.baeldung.com/java-dto-pattern#:~:text=DTOs%20or%20Data%20Transfer%20Objects,Fowler%20in%20his%20book%20EAA.)**


# Software Architecture


## Books


##### **1. [Fundamentals of Software Architecture: An Engineering Approach: Richards, Mark, Ford, Neal: 9781492043454: Amazon.com: Books](https://www.amazon.com/Fundamentals-Software-Architecture-Comprehensive-Characteristics/dp/1492043451/ref=sr_1_21?keywords=Java+Design+Patterns&qid=1683852267&sr=8-21)
2. [Clean Architecture: A Craftsman's Guide to Software Structure and Design (Robert C. Martin Series): Martin, Robert: 9780134494166: Amazon.com: Books](https://www.amazon.com/Clean-Architecture-Craftsmans-Software-Structure/dp/0134494164/ref=pd_rhf_d_se_s_pd_sbs_rvi_sccl_2_1/130-9527237-9753858?pd_rd_w=y4mrC&content-id=amzn1.sym.a089f039-4dde-401a-9041-8b534ae99e65&pf_rd_p=a089f039-4dde-401a-9041-8b534ae99e65&pf_rd_r=FHQ47WSA2JZYK3NZ56MV&pd_rd_wg=XSAo4&pd_rd_r=9b4cd191-974a-4242-8dda-b251a940664e&pd_rd_i=0134494164&psc=1)**


# System Design


## Books


##### **1. [Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems: Kleppmann, Martin: 9781449373320: Amazon.com: Books](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321?tag=javamysqlanta-20)
2. [Clean Code: A Handbook of Agile Software Craftsmanship: Robert C. Martin: 9780132350884: Amazon.com: Books](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882/ref=d_bmx_dp_bk22ez0n_sccl_2_1/130-9527237-9753858?pd_rd_w=lHNJD&content-id=amzn1.sym.e3b35db1-c427-46b1-86ca-67bddaf5745a&pf_rd_p=e3b35db1-c427-46b1-86ca-67bddaf5745a&pf_rd_r=NWGCDHKREX4A72Q8DDAF&pd_rd_wg=WFeJ8&pd_rd_r=5c1bbfd0-3391-461c-b54e-331ef93faae4&pd_rd_i=0132350882&psc=1)
3. [System Design Interview – An insider's guide: Xu, Alex: 9798664653403: Amazon.com: Books](https://www.amazon.com/dp/B08CMF2CQF/ref=sspa_dk_detail_4?psc=1&pd_rd_i=B08CMF2CQF&pd_rd_w=PRymM&content-id=amzn1.sym.eb7c1ac5-7c51-4df5-ba34-ca810f1f119a&pf_rd_p=eb7c1ac5-7c51-4df5-ba34-ca810f1f119a&pf_rd_r=XWS09F2R8FW626XJVSER&pd_rd_wg=kI5V0&pd_rd_r=0b224c1f-1e46-4856-801c-3d92980eee35&s=books&sp_csd=d2lkZ2V0TmFtZT1zcF9kZXRhaWw&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFJOU40Q1lQR0VHM0smZW5jcnlwdGVkSWQ9QTEwMzkyNjgyTTQ5NFdVREMzMUNMJmVuY3J5cHRlZEFkSWQ9QTAxNTg0ODAxU1o1N0JXWDRTM1VXJndpZGdldE5hbWU9c3BfZGV0YWlsJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ==)
4. [System Design Interview – An Insider's Guide: Volume 2: Xu, Alex, Lam, Sahn: 9781736049112: Amazon.com: Books](https://www.amazon.com/System-Design-Interview-Insiders-Guide/dp/1736049119/ref=sr_1_27?keywords=Java+Design+Patterns&qid=1683852267&sr=8-27)
5. [Head First Object-Oriented Analysis and Design: Brett D. McLaughlin, Gary Pollice, Dave West: 9780596008673: Amazon.com: Books](https://www.amazon.com/dp/0596008678/?tag=javamysqlanta-20#customerReviews)Other Random Topic**


# REST, RESTFul


##### **[architecture - What's the difference between REST & RESTful - Stack Overflow](https://stackoverflow.com/a/24584128/7828981)[If REST applications are supposed to be stateless, how do you manage sessions? - Stack Overflow](https://stackoverflow.com/questions/3105296/if-rest-applications-are-supposed-to-be-stateless-how-do-you-manage-sessions?rq=1)**


# Domain Object vs POJO vs Entity vs Model Object vs Repository vs Service 


##### **[c# - What is the difference between domain objects, POCOs, and entities? - Stack Overflow](https://stackoverflow.com/a/6154611/7828981)Java Topics - New**


# Java Annotation - [Java Annotations (With Examples) (programiz.com)](https://www.programiz.com/java-programming/annotations)


##### **Best Tutorial on Annotation: [Annotations In Java Tutorial - How To Create And Use Your Own Custom Annotations](https://youtu.be/DkZr7_c9ry8)Great Answers: [How do annotations like @Override work internally in Java? - Stack Overflow](https://stackoverflow.com/questions/18189980/how-do-annotations-like-override-work-internally-in-java)[Why java annotation syntax has () \[parentheses\]? - Stack Overflow](https://stackoverflow.com/questions/61661257/why-java-annotation-syntax-has-parentheses)**


## Custom Annotations


##### **It is also possible to create our own custom annotations.Its syntax is:\[Access Specifier] @interface&lt;AnnotationName> {           DataType &lt;Method Name>() \[default value];}Here is what you need to know about custom annotation:- Annotations can be created by using @interface followed by the annotation name.
- The annotation can have elements that look like methods but they do not have an implementation.
- The default value is optional. The parameters cannot have a null value.
- The return type of the method can be primitive, enum, string, class name or array of these types.**


### **Example 6: Custom annotation example**


##### **|                                                                                                                                                                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| @interface MyCustomAnnotation {   String value() default "default value"; } class Main {   @MyCustomAnnotation(value = "programiz")   public void method1() {     System.out.println("Test method 1");   }   public static void main(String\[] args) throws Exception {     Main obj = new Main();     obj.method1();   } } |**


### [An Introduction to Annotations and Annotation Processing in Java (reflectoring.io)](https://reflectoring.io/java-annotation-processing/)


##### **-
- [Java Annotations Explained - belief driven design (belief-driven-design.com)](https://belief-driven-design.com/java-annotations-explained-4f54e6e6c3f/)
- Inherited Annotation Explained and Using the Metadata of Annotation: [Java @Inherited | How Java @Inherited work With Examples to Implement (educba.com)](https://www.educba.com/java-inherited/)More:1. [How do annotations like @Override work internally in Java? - Stack Overflow](https://stackoverflow.com/questions/18189980/how-do-annotations-like-override-work-internally-in-java)
2. [How to use custom type annotations in Java - Stack Overflow](https://stackoverflow.com/questions/27606778/how-to-use-custom-type-annotations-in-java/27781761#27781761)
3. [How should I write my own custom Annotation in Java - Stack Overflow](https://stackoverflow.com/questions/29050248/how-should-i-write-my-own-custom-annotation-in-java)
4. [Understanding annotation in Java - Stack Overflow](https://stackoverflow.com/questions/5685795/understanding-annotation-in-java/5686231#5686231)**


# Java Generics


##### **[Java Generics Example Tutorial - Generic Method, Class, Interface | DigitalOcean](https://www.digitalocean.com/community/tutorials/java-generics-example-method-class-interface)[Generic Constructors and Interfaces in Java - GeeksforGeeks](https://www.geeksforgeeks.org/generic-constructors-and-interfaces-in-java/)[Generics in Java - javatpoint](https://www.javatpoint.com/generics-in-java)[Java Generics (With Examples) (programiz.com)](https://www.programiz.com/java-programming/generics)**


# Interface


##### **Passing Interface as an Argument???[oop - interface as a method parameter in Java - Stack Overflow](https://stackoverflow.com/questions/2575429/interface-as-a-method-parameter-in-java)[Why would a method ask for an interface to be passed as a parameter in one of its arguments? - Quora](https://www.quora.com/Why-would-a-method-ask-for-an-interface-to-be-passed-as-a-parameter-in-one-of-its-arguments)- SerializableWrite an example.**


# Inner Class Review


##### ****


# Lamda Expression


##### **Introduced at Java 8[Arrow Operator in Java - Javatpoint](https://www.javatpoint.com/arrow-operator-in-java)[What does the arrow operator, '->', do in Java? - Stack Overflow](https://stackoverflow.com/questions/15146052/what-does-the-arrow-operator-do-in-java)**


# Java Optional


##### **Introduced at Java 8**


# Delegation


##### **What is Delegation?[Delegation | Java Design Patterns (java-design-patterns.com)](https://java-design-patterns.com/patterns/delegation/#explanation)**


## Delegation vs Inheritance


##### **[Delegation vs Inheritance in Java - GeeksforGeeks](https://www.geeksforgeeks.org/delegation-vs-inheritance-java/)**


# Difference between attribute, parameter and argument


##### ****Attributes** are those "variables" declared outside a method in a class, a.k.a. "fields"; **Parameter** is the variable in the declaration of the function.**Argument** is the actual value of this variable that gets passed to the function.Note: In **html** href, type etc are called **attributes**.&lt;a href="<https://www.w3schools.com>" type="text/html">Visit W3Schools.com!&lt;/a>**


# Passing class as an Argument into a Method


##### **[How do I pass a class as a parameter in Java? - Stack Overflow](https://stackoverflow.com/questions/4872978/how-do-i-pass-a-class-as-a-parameter-in-java)**


# Java Web Programming


##### **Follow the content of this[জাভা ওয়েব প্রোগ্রামিং: আ ন ম বজলুর রহমান - Java Web Programming: A N M Bazlur Rahman | Rokomari.com](https://www.rokomari.com/book/200057/java-web-programming)**


## Tutorials


##### **- [Introduction to Servlet in Java | Servlet & JSP #1 - YouTube](https://www.youtube.com/watch?v=xve6QEgIR-0&list=PL0zysOflRCel5BSXoslpfDawe8FyyOSZb&ab_channel=LearnCodeWithDurgesh)
- [Java Servlets & JSP \[2\] - Creating a Java Web Application - YouTube](https://www.youtube.com/watch?v=0FpLve7ffoY&list=PLfu_Bpi_zcDOn8ajnuLY6g1C6hc_eeDFl&ab_channel=KodySimpson)Change The Way You Think@InitBinderpublic void initBinder(WebDataBinder dataBinder) {StringTrimmerEditor stringTrimmerEditor = new StringTrimmerEditor(true);dataBinder.registerCustomEditor(String.class, stringTrimmerEditor);}Most probably, The implementation of **@InitBinder** Annotation is a combination of **@Autowires** and some **other Annotation**. If It is true, then we can think of the initBinder method like this: **an object named “dataBinder” of class type “WebDataBinder” is injected into the initBinder method**.Computer Science Fundamentals:**Memory Types**![](https://lh5.googleusercontent.com/xtTYAu-oGWPh6Ym39EMGLxnm5Jk15iNsjgTFFryOFSZsEUMSjRiQP-n6L1aaaQmkEQntLheW9qwzIp_e0Xp1QU42zw0-WcaHc903tF-KDoj68glNUM0tzmjooFuNQG27VgU4jM2GvmGuHcvlpVueCzE)Cache memory is a high-speed memory, which is small in size but faster than the main memory (RAM). Cache memory can only be accessed by CPU. It acts as a temporary storage area that the computer's processor can retrieve data from easily. So, it makes sure that the data is instantly available for the CPU whenever the CPU needs this data. In other words, if the CPU finds the required data or instructions in the cache memory, it doesn't need to access the primary memory (RAM). Thus, by acting as a buffer between RAM and CPU, it speeds up the system performance.Cache memory is sometimes called [CPU](https://www.techtarget.com/whatis/definition/processor) (central processing unit) memory because it is typically integrated directly into the CPU chip or placed on a separate chip that has a separate [bus](https://www.techtarget.com/searchstorage/definition/bus) interconnect with the CPU. Therefore, it is more accessible to the processor, and able to increase efficiency, because it's physically close to the processor. **L1**: In 99% of cases L1 cache is directly on the chip itself. If a CPU has four cores (quad core cpu), then each core will have its own level 1 cache. As this memory is present in the CPU, it can work at the same speed as the CPU. The size of this memory ranges from 2KB to 64 KB. The L1 cache further has two types of caches: Instruction cache, which stores instructions required by the CPU, and the data cache that stores the data required by the CPU.**Level 2** cache, may be inside the CPU or outside the CPU. All the cores of a CPU can have their own separate level 2 cache, or they can share one L2 cache among themselves. In a vast majority ( there are always exceptions ) of cases, located directly outside of the chip core of the processor. In case it is outside the CPU, it is connected with the CPU with a very high-speed bus. The memory size of this cache is in the range of 256 KB to 512 KB. In terms of speed, they are slower than the L1 cache.L1 caches are generally very small. Considering their location. L2 caches can be a lot bigger, but size still is limited to die space.**L3** cache is used to enhance the performance of Level 1 and Level 2 cache. L3 cache which is somewhere on the motherboard completely outside of the processor or CPU;  some high-end processors may have this type of cache inside. L3 cache is located very close to the CPU, just not actually within the CPU and it is shared by all the cores of a CPU. Its memory size ranges from 1 MB to 8 MB. Although it is slower than L1 and L2 cache, it is faster than Random Access Memory (RAM).**Cache Memory vs Virtual Memory**Cache memory is a memory unit and is very fast to access. Virtual memory is a technique and involves a hard disk and is slower to access. CPU and related hardwares manages cache memory. Operating System manages virtual memory.[**Connection Pooling**](https://docs.google.com/document/d/1qNEe_SvQaTemoMJQhga8SIMkvnZgjicchT0TvwSgRQQ/edit#heading=h.10mtmo8jkzqx)- [****What is connection pooling and when it is used?****](<https://www.quora.com/What-is-connection-pooling-and-when-it-is-used#:~:text=We%E2%80%99ll%20use%20a,in%20my%20experience).>)
- [****java - database connection pool purpose? - Stack Overflow****](https://stackoverflow.com/questions/23174985/database-connection-pool-purpose#:~:text=With%20connection%20pooling%20you%20get,container%20handle%20the%20connection%20pooling.)
- [****Connection Pool Overview — MongoDB Manual****](https://www.mongodb.com/docs/manual/administration/connection-pool-overview/)**


# Database


## SQL


##### ****CREATE** USER IF NOT EXISTS 'hbstudent'@'localhost' IDENTIFIED **BY** 'hbstudent';  **Formate**: CREATE USER 'username'@'host' IDENTIFIED BY 'password';with authentication_plugin for some other backend tech like php that we can do separately later with an alter tag.**Formate**: CREATE USER 'username'@'host' IDENTIFIED WITH authentication_plugin BY 'password';GRANT ALL PRIVILEGES ON \* . \* TO 'hbstudent'@'localhost';\#\# Starting with MySQL 8.0.4, the MySQL team changed the \# default authentication plugin for MySQL server \# from mysql_native_password to caching_sha2_password.\#\# The command below will make the appropriate updates for your user account.\#\# See the MySQL Reference Manual for details: \# https&#x3A;//dev.mysql.com/doc/refman/8.0/en/caching-sha2-pluggable-authentication.html\#ALTER USER 'hbstudent'@'localhost' IDENTIFIED WITH mysql_native_password BY 'hbstudent';[SQL | DDL, DQL, DML, DCL and TCL Commands - GeeksforGeeks](https://www.geeksforgeeks.org/sql-ddl-dql-dml-dcl-tcl-commands/)**


### Alias


##### **Except where clause you can use any alias anywhere. Incase of the where clause, you can use aliases of Table name or Subquery or Database name.But **You can not use aliases of a field name in the where clause, it will produce an error. For example**SELECT first_name AS fname FROM hb_student_tracker.student WHERE ~~fname~~ ="Sanjida" ❌**However you can use aliases of a field name in the HAVING clause** to overcome this issue.SELECT first_name AS fname FROM hb_student_tracker.student HAVING fname="Sanjida" ✅**


### Hibernate with SQL


#### SQL Dialect


##### **A database is a computer program that can store and process large amounts of data. There are many different vendors of databases. PostgreSQL, MySQL, Oracle, and SQL Server are all database products by different vendors. SQL is the programming language used to talk to these databases, and each database product has its own variant of SQL. We call these variants SQL dialects. In hibernate project they have different dialect package for different venders of databases, |                      |                                         |
| -------------------- | --------------------------------------- |
| **RDBMS**            | **Dialect**                             |
| Oracle (any version) | org.hibernate.dialect.OracleDialect     |
| Oracle9i             | org.hibernate.dialect.Oracle9iDialect   |
| Oracle10g            | org.hibernate.dialect.Oracle10gDialect  |
| MySQL                | org.hibernate.dialect.MySQLDialect      |
| Microsoft SQL Server | org.hibernate.dialect.SQLServerDialect  |
| PostgreSQL           | org.hibernate.dialect.PostgreSQLDialect |[What Is a SQL Dialect, and Which one Should You Learn? | LearnSQL.com](https://learnsql.com/blog/what-sql-dialect-to-learn/)**


## HQL


## Database Terms and Technologies


### Connection Pooling


##### **A programming technique where a pool of connections(a number of connections, let's say 10) is built during the application lifecycle.When a user requests for a db operation, the application picks a connection from the pool of these 10 connections as per their availability. When the operation is completed the connection is being released to the pool to serve other requests. Thus limiting to a certain size of connections, we can reduce the overhead involved in performing database connections and read/write database operations.[A Simple Guide to Connection Pooling in Java | Baeldung](https://www.baeldung.com/java-connection-pooling)**


## AFAQ


##### **1. **Should I create user login and user profile in different table?**

   1. [Keep user and user profile in different tables?](https://softwareengineering.stackexchange.com/questions/241089/keep-user-and-user-profile-in-different-tables)
   2. [database - Does it make sense to separate the table of user profile to that of the login details - Stack Overflow](https://stackoverflow.com/questions/36028538/does-it-make-sense-to-separate-the-table-of-user-profile-to-that-of-the-login-de)
   3. [mysql - Should I create 2 tables: first for usernames and passwords, and other for user information like dob, name, etc? - Stack Overflow](https://stackoverflow.com/questions/17683571/should-i-create-2-tables-first-for-usernames-and-passwords-and-other-for-user)
   4.**


# Web Development


##### ****Session based vs Token based authentication:**Session-based authentication (which maintains server state) vs Token-based authentication (which is stateless)Session based authentication:- On login, server generates a unique (very difficult to guess) session id, passes this to the client (browser) which stores it (eg. browser cookie)
- Maintains all session state on the server keyed on session id
- All future incoming requests from client provide this session id to server, which can authenticate the clientToken based authentication- On login, server generates an authentication token based on some cryptographic scheme, passes this to the client (browser) which stores it (eg. browser cookie)
- No state is maintained on the server
- All future incoming requests from client provide the auth token to server. Server then uses the features of the cryptographic scheme to verify the auth token on the fly to authenticate clientRef: [Sessions vs. Token based authentication](https://stackoverflow.com/questions/40200413/sessions-vs-token-based-authentication)**


# Security


## Securing Password


### Salt Pepper


##### **[What Is Peppering in Password Security and How Does It Work? (makeuseof.com)](https://www.makeuseof.com/what-is-peppering-how-does-it-work/)[security - Best Practices: Salting & peppering passwords? - Stack Overflow](https://stackoverflow.com/questions/16891729/best-practices-salting-peppering-passwords)[passwords - How to apply a pepper correctly to bcrypt? - Information Security Stack Exchange](https://security.stackexchange.com/questions/21263/how-to-apply-a-pepper-correctly-to-bcrypt)[What Is Password Salting - GlobalSign](https://www.globalsign.com/en/blog/what-is-password-salting)**AFAQ**1. [****_How do you store username and salt in separate table?_****](https://www.quora.com/How-do-you-store-username-and-salt-in-separate-table-passwords-password-management-password-cracking-security)

   1. **While you _could_ store the user’s login name and their password salt in separate tables, _there is no need to do so._**Many people misunderstand the purpose of password salt. The salt value is _not_ a secret that a potential attacker must guess. Instead, it is an additional input to the hash function that forces the resulting password hash to be different for each user, _even if their plaintext password is the same_.Without a salt value, an attacker could conduct a brute-force password guessing attack by pre-computing a hash for each possible password, and searching the table of password hashes for matching values. Using a different random salt value for each user forces the attacker to do much more work — they must compute hashes for possible passwords individually for each user, using that user’s salt value._To give a simplified example, let’s assume that the attacker has obtained a table of password hashes for 5000 users, and also knows that all passwords are 8-character mixed-case values. Without salt, the attacker can compute hashes for all 53 trillion possible hashes in about 3 days using modern hardware. The attacker can check every user password hash against these values as they are generated, and brute-force all 5000 passwords during a single 3-day run — breaking about one account a minute.__HOWEVER, if there is a different 256-bit random salt value for each user, the attacker must compute the hashes for each user to incorporate the salt value. With salt, the attacker will break about one password every 36 hours — and take more than 20 years to brute-force all 5000 passwords!_**It is a best practice to use _both_ SALT and PEPPER in password hashes:**- **SALT** is a non-secret random value that is different for each user. Since the salt value is not secret, it may be stored with the user’s login name and password hash for easy access. _The purpose of the salt is to force an attacker to compute hash values on a per-user basis._
- **PEPPER** is a secret random value that is the same for all users managed by the system. _The purpose of the pepper is to add entropy to the system, forcing an attacker to perform much more work to do a brute force search of password hashes._Both the salt and pepper values should be random values that have about the same number of bits as the password hash’s output value.The password hash function should accept three inputs: the user’s plain text password, the salt value, and the pepper value. Of these three, the user’s plain text password must never be stored on the system; the salt value may be stored along with other information about the user; and the pepper must be stored in a separate (and hopefully more-secure) location that can be accessed when needed._To go back to my example above, the system has relatively weak passwords (45 bits of entropy). Without either salt or pepper, the attacker can brute-force about one password a minute. Adding a random salt value (that the attacker knows) to the password hash slows this to about one every 36 hours. Adding a random 256-bit pepper value makes the hashes practically unbreakable unless the attacker is able to obtain the pepper value as well._Analysing Java Developer Job Requirement**


### **Job requirements**


##### **- REST/JSON and **SOAP**/XML
- HTML/CSS: twitter-bootstrap, foundation etc., Jquery
- Oracle and PostgreSQL
- Maven, Git, Jenkins
- Experience in Azure
- It's a plus (Java certifications, working with AWS, Spring boot)
- Experience in web application development using at least one of these frameworks (Spring, MVC, Grails)
- A plus but not required (Java certifications, working with AWS, experience in Spring boot)New Update of the course**


### **NEW - Spring Boot 3 Quick Start**


##### **70, 71 , 72, 73 + some new contentWhat Are REST Services - Part 1**


### **NEW - Spring Boot 3 - Inversion of Control and Dependency Injection**


##### ****


### **NEW - Spring Boot 3 - Database Access with Hibernate/JPA CRUD**


##### ****


### **NEW - Spring Boot 3 - REST CRUD APIs**


##### **56 - 69 , 74 - 77 combination of both**


### **NEW - Spring Boot 3 - REST API Security**


##### ****


### **NEW - Spring Boot 3 - Spring MVC Introduction with Thymeleaf**


##### **78, 79**


### **NEW - Spring Boot 3 - Spring MVC CRUD**


##### **8081**


### **NEW - Spring Boot 3 - Spring MVC Security**


##### 47 - 55 AKA Spring Security
