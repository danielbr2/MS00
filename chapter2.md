---
title       : Funktionen
description : Üben Sie hier den Umgang mit Funktionen.


--- type:NormalExercise lang:r xp:100 skills:1 key:1ed65e9ca4
## Übersicht über den Datensatz


*** =instructions
Lesen Sie den Datensatz ein und verschaffen Sie sich einen Überblick.

*** =hint

*** =pre_exercise_code
```{r}
```

*** =sample_code
```{r}
# nutzen Sie den read.csv() Befehl
# die erforderlichen Daten befinden sich unter http://s3.amazonaws.com/assets.datacamp.com/production/course_2115/datasets/Datensatz_A1.csv
# nutzen Sie den summary() Befehl
```

*** =solution
```{r}
datensatz <-read.csv( 'http://s3.amazonaws.com/assets.datacamp.com/production/course_2115/datasets/Datensatz_A1.csv' , sep= ';')
summary(datensatz)
```

*** =sct
```{r}
test_function_result("summary")
success_msg("Richtig! Weiter gehts...")
```



--- type:NormalExercise lang:r xp:100 skills:1 key:7e4ee704e0
## Varianz Berechnung 


*** =instructions
Berechnen Sie die Varianz des Merkmals preis mit der Formel: $\frac{1}{n} \sum_{i=1}^n (X_i-\mu)^2$

*** =hint

*** =pre_exercise_code
```{r}
datensatz <-read.csv( 'http://s3.amazonaws.com/assets.datacamp.com/production/course_2115/datasets/Datensatz_A1.csv' , sep= ';')
```

*** =sample_code
```{r}
# der Datensatz ist bereits eingelesen als 'datensatz'
# speichern Sie das Ergebnis unter der Variablen varianz.b
```

*** =solution
```{r}
mittelwert<-mean(datensatz$preis)
varianz.b<-mean((datensatz$preis-mittelwert)^2)

```

*** =sct
```{r}
test_object("varianz.b", 
        incorrect_msg = "Die Varianz wurde nicht korrekt berechnet!")
success_msg("Richtig! Weiter gehts...")      
```
