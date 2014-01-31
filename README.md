commons-opensource-super-pom
============================

Commons Super POM for Open Source projects.

The Super POM contains build configuration that is common to many (sometimes all) modules.

The motivation for its use is to single-source as much of the lightweight, often-used build configuration as possible.

Usage
-----

Add the following to the top of your project's root or parent pom.xml:

```xml
<parent>
    <groupId>com.bazaarvoice.commons</groupId>
    <artifactId>bv-opensource-super-pom</artifactId>
    <version>1.2</version>
    <relativePath />
</parent>
```
