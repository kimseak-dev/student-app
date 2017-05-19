# student-app
maven with inheritance and aggre 
Basic Understanding about Maven

# What is MAVEN?
- [x] It is a project management tool which based on the Project Object Model (POM). 
- [ ] It helps helps developers with complete build lifecycle.
- [ ] Developer team can be automate a certain project’s build infrastructure
# Maven Explanation

- [x] Why  maven?
- [ ] There is no standard way to manage software project. For example: when handle  compilation + packaging ( JARs, WARs) +  test  differently in different project. 
- [ ] Maven sole this problem with convention over the configuration principle. If all projects follow the same conventions( similar directory layout, way of running test, …). It mean that programer do not have to create process themselves. Do not have know every configuration-related detail. Maven crate the default project structure -> developer just have to put file accordingly.
- [ ] There may be several situations when we have several independent project with different JAR. We want a standard way to build our project + shared JAR across several project.
- [ ] MAVEN = build automation tool or software project management tool.
- [ ] It provide the guidelines for the best practice development. For example : unites, documentations, dependencies.
- [x] What are these configurations?
- [ ] Compilation of java source code
- [ ] package source code into JARs or WARs
- [ ] Running tests
- [ ] Generate project documents
- [x] Framework  Used
- [ ] Spring Framework for java enterprise projects.
- [ ] VAADIN framework to build UI related to applications.
- [ ] Hibernate in order to manage database related problems.
- [ ] 
# What is Maven repository?
- [ ] A repository is location or directory where all the project jars, libraries and plugin are stored.
- [ ] These artifacts be used by Maven.
- [x] The are three type of Maven repo  : 
1. local( on your own machine ),
2.  central ( on a predefined website )
3. remote ( we can define the location of our server for example)

# What is the Maven build lifecycles?
- [x]  A Maven lifecycle is just a sequence of phase which define the order in which goals are to be executed. 


- If we use the MVN command  -> we use maven lifecycle parse or goals. Lifecycle -> It has phase. Plugin -> it have goals.
- Maven has  3  lifecycle ( clean, site, default ) and every lifecycle contains multiple phases.

- [x] Clean
- [ ] In order to clean project (mvn clean). It’s going to remove the target folder with the JAR file.
- [ ] contain 3 phase: pre-clean, clean, post-clean. Maven executes all the phases up to the one we invoke.
- [ ] phases are not able to do anything. They call plugin, and plugin will do the work ( remove target folder )
- [x] Site  
- [ ] Generate project documentation about the current project.
- [ ] Contain 4 phases: pre-site, site, post-site, site-deploy. 
- [ ] We are able to generate a documentation by running the maven command(mvn site).
- [ ] If we run mvn site-deploy -> all the previous phases will run as well.
- [x] Default 
- [ ] It has 22 phases all together
- [ ] Maven uses this lifecycle to build and distribute the given project
- [ ] If run mvn install  all the pre-phases will run as well

- process-resource: copy the resource into target folder
- compile: compile the source code
- test: run the tests
- package: make a distributable format such as JARs or Wars
- install: install the package into the local repository
- deploy: copy the package to remote repository  

- [ ] Plugins
- [ ] Maven is a plugin execution framework
- [ ] Every operation is executed by a plugin
- [ ] It has plugins like :
- clean: cleans up the target folder
- compiler: compiles the source code
- surefire : run the unit test
- jar: build a JAR from the project
- war: builds a WAR from project
- javadoc: generates document  

# What is the POM file?
- [x] It mean Project Object Model.
- [ ] Basically it is an XML file located in the base directory of the project.
- [ ] It contains all the information needed by Maven in order to build the project


- [x] GroupId is the name of the organization which own the the project and usually a reversed domain name.
- [x] ArtifactId is the name of the project, library, plugin or software component.
- [ ]  Version  is the version.,
# What is Maven reactor?
- [ ] When we have server modules and
- [ ] One module depend on another module or
- [ ] Modules then the order build can not be random because dependencies
- [ ] A depends on B, B must be build before A.
- [ ] Maven reactor helps to come up withe the order ( with topological sort) which the modules has to be compiled and built.

# What is a Maven artifact?

- [ ] Basically everything that can be deployed to a Maven repository.
- [ ] Usually artifacts are JAR file.
- [ ] Each artifacts has a groupId  + an artifactId  + a version
- [ ] These parameters are uniquely identify every single artifact.

# What is a SNAPSHOT?
- [x] SNAPSHOT is special version that indicate a current development copy.
- [ ] SNAPSHOT version might get updates.
- [x] So 1.0 SNAPSHOT might have different file today than downloading it yesterday
- [x] Usually snapshot dependencies should only exist during development.
- [x] Unlike regular version, Maven checks for new snapshot version in the remote repository for every build.

# What is a Maven artifact?

- [ ] Basically everything that can be deployed to a Maven repository.
- [ ] Usually artifacts are JAR file.
- [ ] Each artifacts has a groupId  + an artifactId  + a version
- [ ] These parameters are uniquely identify every single artifact.







