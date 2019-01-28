Based on Udemy 'Selenium WebDriver With Java - Novice To Ninja'
Section 42, Lecture 210 Creating and importing Maven project
==============================================================

Create Quickstart project
-------------------------
$ mvn archetype:generate -DarchetypeArtifactId=maven-archetype-quickstart -DgroupId=dragan -DartifactId=cucumberselenium -DinteractiveMode=false

Remove unneeded files
---------------------
Remove 'main' folder under 'src' and 'dragan' under 'src/test'

Update POM file
---------------
Add following dependencies:

```
  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.12</version>
      <scope>test</scope>
    </dependency>
    <dependency>
    	<groupId>org.seleniumhq.selenium</groupId>
    	<artifactId>selenium-java</artifactId>
    	<version>3.141.59</version>
    </dependency>
    <dependency>
    	<groupId>cobertura</groupId>
    	<artifactId>cobertura</artifactId>
    	<version>1.9rc1</version>
    </dependency>
    <dependency>
    	<groupId>info.cukes</groupId>
    	<artifactId>cucumber-jvm-deps</artifactId>
    	<version>1.0.5</version>
    </dependency>
    <dependency>
    	<groupId>net.masterthought</groupId>
    	<artifactId>cucumber-reporting</artifactId>
    	<version>4.3.0</version>
    </dependency>
    <dependency>
    	<groupId>info.cukes</groupId>
    	<artifactId>gherkin</artifactId>
    	<version>2.12.2</version>
    	<scope>provided</scope>
    </dependency>
    <dependency>
    	<groupId>org.mockito</groupId>
    	<artifactId>mockito-all</artifactId>
    	<version>1.10.19</version>
    </dependency>
    <dependency>
    	<groupId>info.cukes</groupId>
    	<artifactId>cucumber-core</artifactId>
    	<version>1.2.5</version>
    </dependency>
    <dependency>
    	<groupId>info.cukes</groupId>
    	<artifactId>cucumber-junit</artifactId>
    	<version>1.2.5</version>
    </dependency>
    <dependency>
    	<groupId>info.cukes</groupId>
    	<artifactId>cucumber-java</artifactId>
    	<version>1.2.5</version>
    </dependency>
  </dependencies>
```