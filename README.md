# commons-opensource-super-pom

Commons Super POM for Open Source projects. The Super POM contains build
configuration that is common to many (sometimes all) modules.

The motivation for its use is to single-source as much of the lightweight,
often-used build configuration as possible.

## OWASP Dependency Check Plugin

This module includes the [OWASP dependency check plugin][1], which checks the
project dependencies for versions with publicly disclosed security
vulnerabilities. It is important to keep this plugin up to date, just as it is
important to react to its warnings and update vulnerable dependencies.

## Usage

Add the following to the top of your project's root or parent pom.xml. Make
sure that you specify the latest version:

```xml
<parent>
    <groupId>com.bazaarvoice.commons</groupId>
    <artifactId>bv-opensource-super-pom</artifactId>
    <version>1.4</version>
    <relativePath />
</parent>
```

[1]: http://mvnrepository.com/artifact/org.owasp/dependency-check-maven
