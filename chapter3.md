---
title       : Funktionen
description : Üben Sie hier den Umfang mit Funktionen


--- type:NormalExercise lang:r xp:100 skills:1 key:1ed65e9ca4
## Übersicht über den Datensatz

Verschaffen Sie sich einen Überblick über den Datensatz.


*** =instructions
Verschaffen Sie sich einen Überblick über den Datensatz.

*** =hint

*** =pre_exercise_code
```{r}
datensatz<- read.csv( "http://s3.amazonaws.com/assets.datacamp.com/production/course_2115/datasets/Datensatz_A1.csv", sep=";")
```

*** =sample_code
```{r}
# nutzen Sie den summary() Befehl
```

*** =solution
```{r}
summary(datensatz)
```

*** =sct
```{r}
test_function_result("summary")
```
