---
title       : Datenstrukturen
description : 
attachments :
  slides_link : 

--- type:NormalExercise lang:r xp:100 skills:1,3 key:02429cb8ed
## Eingabe von Vektoren



*** =instructions
Geben Sie die vorliegenden Daten des Autodatensatzes jeweils als Vektor in die Software R ein.

Preis: 850, 4400, 14250 
Alter: 14, 8, 2
Kilometer: 252000, 189000, 8600



*** =hint
Nutzen Sie `<-`


*** =sample_code
```{r}
# Benennen Sie die Variablen mit preis, alter und kilometer

```

*** =solution
```{r}
preis<-c(850,4400,14250)
alter<-c(14,8,2)
kilometer<-c(252000,189000,8600)
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki
test_error()
test_object("preis",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
test_object("alter",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
test_object("kilometer",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
            

success_msg("Richtig! Weiter gehts...")
```

--- type:NormalExercise lang:r xp:100 skills:1,3 key:7aebe50357
## Eingabe von Matrizen




*** =instructions
Geben Sie die vorliegenden Daten als Matrix ein.

Preis: 850, 4400, 14250 
Alter: 14, 8, 2
Kilometer: 252000, 189000, 8600


*** =hint
cbind 

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer
preis<-c(850,4400,14250)
alter<-c(14,8,2)
kilometer<-c(252000,189000,8600)
```

*** =solution
```{r}
testMatrix<- cbind(preis,alter,kilometer)
```

*** =sample_code
```{r}
# speichern Sie die Matrix unter der Variable testMatrix
# die Vektoren aus der vorherigen Aufgabe sind bereits eingelesen, d.h. Sie können auf preis, alter und kilometer zugreifen
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki
test_error()
test_object("testMatrix",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
success_msg("Richtig! Weiter gehts...")
```



--- type:NormalExercise lang:r xp:100 skills:1,3 key:0d6d0b19b4
## Eingabe von Datensätzen


*** =instructions
Geben Sie die vorliegenden Daten als data.frame ein.

Preis: 850, 4400, 14250 
Alter: 14, 8, 2
Kilometer: 252000, 189000, 8600


*** =hint
data.frame()

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer
preis<-c(850,4400,14250)
alter<-c(14,8,2)
kilometer<-c(252000,189000,8600)
```

*** =solution
```{r}
testDataframe<- data.frame(preis,alter,kilometer)
```


*** =sample_code
```{r}
# speichern Sie den data.frame unter der Variable testDataframe
# die Vektoren aus der vorherigen Aufgabe sind bereits eingelesen, d.h. Sie können auf preis, alter und kilometer zugreifen
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki
test_error()
test_object("testDataframe",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
success_msg("Richtig! Weiter gehts...")
```


