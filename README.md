# Java Barcode Reader

The sample shows how to use [Dynamsoft Barcode Reader SDK](https://www.dynamsoft.com/Products/Dynamic-Barcode-Reader.aspx) to build a simple Java barcode reader.

## Usage

Set a valid [license key](https://www.dynamsoft.com/CustomerPortal/Portal/Triallicense.aspx):

```java
br = new BarcodeReader("LICENSE-KEY");
```

Run the Java program in command-line tools:

```
mvn clean install assembly:assembly
java -cp target/test-1.0-SNAPSHOT-jar-with-dependencies.jar com.dynamsoft.App images/AllSupportedBarcodeTypes.png
```

## Docker Linux Container

```
docker rmi dynamsoft/barcode-reader -f
docker build -t dynamsoft/barcode-reader -f Dockerfile .
docker run -it dynamsoft/barcode-reader
```

![Java barcode reader in Docker](https://www.codepool.biz/wp-content/uploads/2020/02/java-barcode-reader-docker.png)
