---
title       : Datenstrukturen
description : 
attachments :
  slides_link : 

--- type:NormalExercise lang:r xp:100 skills:1,3 key:02429cb8ed
## Eingabe von Vektoren

Geben Sie die vorliegenden Daten des Autodatensatzes jeweils als Vektor in die Software R ein.

Preis: 850, 4400, 14250 

Alter: 14, 8, 2

Kilometer: 252000, 189000, 8600

Benennen Sie die Variablen mit 'preis', 'alter' und 'kilometer'

*** =hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

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
            

success_msg("Good work!")            
#success_msg("Richtig! Weiter zur nächsten Aufgabe...")
```

--- type:NormalExercise lang:r xp:100 skills:1,3 key:7aebe50357
## Eingabe von Matrizen

Geben Sie die vorliegenden Daten Matrix mit dem Namen 'testMatrix' ein.

Preis: 850, 4400, 14250 

Alter: 14, 8, 2

Kilometer: 252000, 189000, 8600

*** =hint

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

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki
test_error()
test_object("testMatrix",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
success_msg("Richtig! Weiter zur nächsten Aufgabe...")
```



--- type:NormalExercise lang:r xp:100 skills:1,3 key:0d6d0b19b4
## Eingabe von Datensätzen

Geben Sie die vorliegenden Daten nun als data.frame mit dem Namen 'testDataframe' ein.

Preis: 850, 4400, 14250 

Alter: 14, 8, 2

Kilometer: 252000, 189000, 8600

*** =hint

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

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki
test_error()
test_object("testDataframe",
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
success_msg("Richtig! Weiter zur nächsten Aufgabe...")
```


