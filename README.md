# big-app.kotlin
Sample application with ~500 Kotlin classes to test performance of Kotlin compiler

# to measure compilation time
 
... just run from command line:

```
./gradlew clean classes
```

# Results on my machine (MacBook Pro 2017) 
* Kotlin 1.1.4-3:         `BUILD SUCCESSFUL in 8m 0s`
* Kotlin 1.2.41:          `BUILD SUCCESSFUL in 7m 9s`
* Kotlin 1.2.50:          `BUILD SUCCESSFUL in 6m 20s`