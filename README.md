# Gengo Scraper
## About
Gengo Scraper is an application to retrieve info from Gengo website by scraping its contents.

Currently it retrieves info about archived jobs.

## Download and use on Windows environment
- Download resources under 'run' folder:
  - gengoscraper-1.0.0.jar
  - config.properties
  - runme.bat
- Ensure that you have Java 8 installed.
- Edit **config.properties** to set your user, password and max number of pages to retrieve. Each page contains 20 archived jobs.
- Run **runme.bat**.
- The results will be stored in a file called **results.csv** in the same folder.

## Download and use on other environments
- Same above steps, but instead of running **runme.bat** you can run the JAR file directly:

```
java -jar ./gengoscraper-1.0.0.jar --spring.config.location=file:./config.properties
```

## If you prefer to compile
- Ensure that you have Java 8 installed.
- Download sources under **src** folder.
- Compile them with Maven: **mvc package**
- The compiled binaries will be generated into **target** folder.
- Create a **config.properties** like the one you can find under **run** folder and configure it.
- Run the application as stated above.
