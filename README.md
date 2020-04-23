# Java DotCode Reader
The two samples demonstrate how to decode DotCode using [Dynamsoft Barcode Reader SDK v7.4 for Java](https://www.dynamsoft.com/Downloads/Dynamic-Barcode-Reader-Download.aspx).

## Trial License
Get a [valid license](https://www.dynamsoft.com/CustomerPortal/Portal/Triallicense.aspx) and update relevant code:

```java
mBarcodeReader = new BarcodeReader("LICENSE-KEY");
```

## Usage

- command-line

  ```
  mvn clean install assembly:assembly -Dmaven.test.skip=true
  java -cp target/command-line-dotcode-1.0-SNAPSHOT-jar-with-dependencies.jar com.java.barcode.App test.png
  ```

- opencv
  
  1. Install OpenCV to Maven local repository.
  
      ```
      mvn install:install-file -Dfile=opencv-430.jar -DgroupId=org -DartifactId=opencv -Dversion=4.3.0 -Dpackaging=jar
      ```
    
  2. Build and run the project.
  
      ```
      mvn clean install assembly:assembly -Dmaven.test.skip=true
     java -cp target/opencv-dotcode-1.0-SNAPSHOT-jar-with-dependencies.jar com.java.barcode.App
      ```

     ![Java DotCode Reader](http://www.codepool.biz/wp-content/uploads/2020/04/java-dotcode-reader.png)
