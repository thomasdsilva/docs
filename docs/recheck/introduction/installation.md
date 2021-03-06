# Installation

!!! info 
	You should only need to define the dependency if you plan to extend ***recheck*** yourself. You may use an already implemented extension.

## Extensions

***recheck*** is usually used with extensions that provide the capability for converting the objects of a specific technology into the domain model of ***recheck***.

Available extensions:

* [***recheck-web***](https://github.com/retest/recheck-web): Testing websites and web applications based on [Selenium](https://www.seleniumhq.org/).
* *More to come*

Alpha extensions (proof of concept):

* [***recheck-logs***](https://github.com/retest/recheck-logs): Verify text-based logs.
* [***recheck-xml***](https://github.com/retest/recheck-xml): Verify `xml` files.

!!! tip
	If you are developing an extension for ***recheck***, we would be happy if you [contact us](https://retest.de/contact-us/) or add your extension with a short description here.

!!! tip
	Extensions, but also frontends such as the recheck.cli or review, are supposed to be compatible across [minor versions](https://semver.org/). That is, you can view reports from, e.g., recheck-web 1.5.1 with recheck.cli 1.5.0 as they both share the minor version 5, which means they use recheck 1.5.x under the hood.

## Build tools

You can add ***recheck*** as an external dependency to your project. It is available in [Maven central](https://mvnrepository.com/artifact/de.retest/recheck) or via the [release-page](https://github.com/retest/recheck/releases), which allows you to include it into your favorite build tool.

For the current version, please refer to the release-page.

### Maven

```xml
<dependency>
	<groupId>de.retest</groupId>
	<artifactId>recheck</artifactId>
	<version>${LATEST_VERSION_FROM_ABOVE_LINK}</version>
</dependency>
```

### Gradle

```gradle
compile 'de.retest:recheck:${LATEST_VERSION_FROM_ABOVE_LINK}'
```
