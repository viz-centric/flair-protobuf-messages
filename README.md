[![Build Status](https://dev.azure.com/VizCentric/Flair%20BI/_apis/build/status/viz-centric.flair-protobuf-messages?branchName=master)](https://dev.azure.com/VizCentric/Flair%20BI/_build/latest?definitionId=2&branchName=master)

# flair-protobuf-messages
Message definitions for flair communication

## Build

To build the application and install in local maven repository use

```
mvn clean install
```

## Release

To perform a release you need:
*  have configured credentials in settings.xml

    ```
    <settings>  
        <servers>  
            <server>
                <id>github-credentials</id>  
                <username>myUser</username>  
                <password>myPassword</password>  
            </server>   
        </servers>
    </settings>   
    ```
* run following command you need to set development version and release version:

   ``` 
   mvn release:clean release:prepare release:perform -DreleaseVersion=${releaseVersion} -DdevelopmentVersion=${developmentVersion}
   ```

