# Actions on Google Java/Kotlin Client Library with fix for SmartPhoneApp.kt channel close.


* [GitHub repo](https://github.com/actions-on-google/actions-on-google-java)
* [Reference docs](https://actions-on-google.github.io/actions-on-google-java/)
* [Actions on Google docs](https://developers.google.com/assistant)
* [Actions on Google samples](https://developers.google.com/assistant/actions/samples)

## changes from master branch

* add dependency for javax.annotation to allow compilation with java>8
* remove jar signing

* to allow publishing to github let mvn know your github account info
~/.m2/settings
```
<settings>
    <servers> 
        <server>
            <id>github</id>
            <username>devs-emporia</username>
            <password>personal token value</password>
        </server>
    </servers>
</settings>
```



## build instructions

$ mvn install:install-file -Dfile=lib/libactions_java_lib.jar -DgroupId=com.google.actions -DartifactId=actions-bindings -Dversion=2.0.0 -Dpackaging=jar -DgeneratePom=true \
$ mvn install:install-file -Dfile=lib/libdialogflow_java_lib.jar -DgroupId=com.google.actions -DartifactId=dialogflow-bindings -Dversion=2.0.0 -Dpackaging=jar -DgeneratePom=true

$ mvn install
