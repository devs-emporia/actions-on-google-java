# Actions on Google Java/Kotlin Client Library with fix for SmartPhoneApp.kt channel close.


* [GitHub repo](https://github.com/actions-on-google/actions-on-google-java)
* [Reference docs](https://actions-on-google.github.io/actions-on-google-java/)
* [Actions on Google docs](https://developers.google.com/assistant)
* [Actions on Google samples](https://developers.google.com/assistant/actions/samples)

## changes from master branch

* add dependency for javax.annotation to allow compilation with java>8
* remove jar signing


## build

* install provided jars in lib directory to your local m2
mvn install:install-file -Dfile=lib/libactions_java_lib.jar -DgroupId=com.google.actions -DartifactId=actions-bindings -Dversion=2.0.0 -Dpackaging=jar -DgeneratePom=true
mvn install:install-file -Dfile=lib/libdialogflow_java_lib.jar -DgroupId=com.google.actions -DartifactId=dialogflow-bindings -Dversion=2.0.0 -Dpackaging=jar -DgeneratePom=true

* build and install locally

mvn install
