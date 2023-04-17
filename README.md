# big-app.kotlin
Sample application with ~500 Kotlin classes to test performance of Kotlin compiler

See issue https://youtrack.jetbrains.com/issue/KT-20055

# to measure compilation time
 
... just run from command line:

```
./gradlew clean classes --rerun-tasks
```

# Results on my machine (MacBook Pro 2017) 
* Kotlin 1.1.4-3:         `BUILD SUCCESSFUL in 8m 0s`
* Kotlin 1.2.41:          `BUILD SUCCESSFUL in 7m 9s`
* Kotlin 1.2.50:          `BUILD SUCCESSFUL in 6m 20s`
* Kotlin 1.2.51:          `BUILD SUCCESSFUL in 4m 52s`
* Kotlin 1.2.60:          `BUILD SUCCESSFUL in 4m 54s`
* Kotlin 1.2.61:          `BUILD SUCCESSFUL in 4m 9s`
* Kotlin 1.2.70:          `BUILD SUCCESSFUL in 3m 43s`
* Kotlin 1.2.71:          `BUILD SUCCESSFUL in 4m 7s`,   // -nowarn: `BUILD SUCCESSFUL in 3m 43s`
* Kotlin 1.3.0:           `BUILD SUCCESSFUL in 3m 58s`
* Kotlin 1.3.10:          `BUILD SUCCESSFUL in 3m 50s`
* Kotlin 1.3.21:          `BUILD SUCCESSFUL in 3m 2s`
* Kotlin 1.3.30:          `BUILD SUCCESSFUL in 2m 35s`
* Kotlin 1.3.31:          `BUILD SUCCESSFUL in 3m 18s`
* Kotlin 1.3.40:          `BUILD SUCCESSFUL in 3m 52s`
* Kotlin 1.3.50:          `BUILD SUCCESSFUL in 3m 6s`
* Kotlin 1.3.60:          `BUILD SUCCESSFUL in 3m 16s`
* Kotlin 1.3.70:          `BUILD SUCCESSFUL in 2m 51s`
* Kotlin 1.3.71:          `BUILD SUCCESSFUL in 2m 40s`
* Kotlin 1.3.72:          `BUILD SUCCESSFUL in 3m 27s`
* Kotlin 1.4.0:           `BUILD SUCCESSFUL in 4m 18s`
* Kotlin 1.4.10:          `BUILD SUCCESSFUL in 3m 33s`
* Kotlin 1.4.20:          `BUILD SUCCESSFUL in 4m 57s`
* Kotlin 1.4.21:          `BUILD SUCCESSFUL in 3m 49s`
* Kotlin 1.4.30:          `BUILD SUCCESSFUL in 4m 4s`
* Kotlin 1.4.31:          `BUILD SUCCESSFUL in 5m 10s`
* Kotlin 1.5.0:           `BUILD SUCCESSFUL in 3m 28s`
* Kotlin 1.5.10:          `BUILD SUCCESSFUL in 3m 34`
* Kotlin 1.5.20:          `BUILD SUCCESSFUL in 4m 10s`
* Kotlin 1.5.21:          `BUILD SUCCESSFUL in 3m 54s`
* Kotlin 1.5.30:          `BUILD SUCCESSFUL in 4m 5s`
* Kotlin 1.5.31:          `BUILD SUCCESSFUL in 3m 57s`
* Kotlin 1.6.0:           `BUILD SUCCESSFUL in 4m 19s`
* Kotlin 1.6.10:          `BUILD SUCCESSFUL in 2m 11s`    | M1 `48s`
* Kotlin 1.7.0:           `BUILD SUCCESSFUL in 3m 35s`
* Kotlin 1.7.0-k2:        `BUILD SUCCESSFUL in 2m 7s`

The following times are measured on MacBook Pro M1 2021:
* Kotlin 1.8.0:           `BUILD SUCCESSFUL in 35s`
* Kotlin 1.8.10:          `BUILD SUCCESSFUL in 39s`
* Kotlin 1.8.20:          `BUILD SUCCESSFUL in 33s`


