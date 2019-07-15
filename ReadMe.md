# Some Samples of Elasticsearch
This project contains some samples of Elasticsearch which is edited by java.

## Development Environment
Java: orcle jdk-1.8 

elasticsearch: 5.4.3

## About the Dependciens
```aidl

    <dependencies>
        <dependency>
            <groupId>org.elasticsearch.client</groupId>
            <artifactId>transport</artifactId>
            <version>5.4.3</version>
        </dependency>

        <dependency>
            <groupId>org.elasticsearch</groupId>
            <artifactId>elasticsearch</artifactId>
            <version>5.4.3</version>
        </dependency>

        <dependency>
            <groupId>org.apache.logging.log4j</groupId>
            <artifactId>log4j-api</artifactId>
            <version>2.8.2</version>
        </dependency>

        <dependency>
            <groupId>org.apache.logging.log4j</groupId>
            <artifactId>log4j-core</artifactId>
            <version>2.8.2</version>
        </dependency>
    </dependencies>

```
## File List
ESSample.java: contains some samples

HelloES.java: Program Entry

## Sample Lists
### QueryDoc
Obtain a doc form a index.

**INPUT**

- TransportClient client
- String index
- String type
- String id

**OUTPUT**

a doc in Json

**EXAMPLE**
```aidl
"account_number":1,"balance":39225,"firstname":"Amber","lastname":"Duke","age":32,"gender":"M","address":"880 Holmes Lane","employer":"Pyrami","email":"amberduke@pyrami.com","city":"Brogan","state":"IL"
```
### UploadData

**INPUT**

- TransportClient client
- String index
- String type
- String json

**OUTPUT**

the state of the query, if successed, return "created"
