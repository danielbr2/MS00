---
title       : Subsetting
description : Üben Sie hier den Zugriff auf verschiedene Datenstrukturen


--- type:NormalExercise lang:r xp:100 skills:1 key:c1956471ec
## Ersetzen von fehlenen Werten


*** =instructions

Ersetzen Sie den fehlenden Wert in der Variable Kilometer durch den Mittelwert der übrigen Werte.

*** =hint
Berechnen Sie zunächst den Mittelwert der "nicht NA" Werte.
Weisen Sie anschließend mit [] diesen berechneten Wert dem NA Wert zu.

*** =pre_exercise_code
```{r}
datensatz <-read.csv( 'http://s3.amazonaws.com/assets.datacamp.com/production/course_2115/datasets/Datensatz_A1.csv' , sep= ';')
```

*** =sample_code
```{r}
# der Datensatz ist bereits eingelesen als 'datensatz'
# speichern Sie das Ergebnis ebenfalls unter der Variablen 'datensatz'
```

*** =solution
```{r}
mw.kilometer<-mean(datensatz$kilometer,na.rm=TRUE) # warum reicht der einfache mean() Befehl nicht aus?
datensatz$kilometer[9]<-mw.kilometer
```

*** =sct
```{r}
test_error()
test_object("datensatz",
             incorrect_msg = "Der richtige Wert wurde nicht ersetzt!")
success_msg("Richtig! Weiter gehts...")
```
