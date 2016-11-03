---
title       : Datenstrukturen
description : 
attachments :
  slides_link : 

--- type:NormalExercise lang:r xp:100 skills:1,3
## Eingabe von Vektoren

Geben Sie die vorliegenden Daten des Autodatensatzes jeweils als Vektor in die Software R ein.

Preis       Alter (in Jahren)       Kilometer
-------     -------                 -------
850         14                      252000
4400        8                       189000
14250       2                       86000

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
test_object(c("preis","alter","kilometer"),
            undefined_msg = "Hier hat etwas nicht geklappt. Versuchen Sie es erneut!",
            incorrect_msg = "Es wurden falsche Werte zugewiesen.")
success_msg("Richtig! Weiter zur nächsten Aufgabe...")
```

--- type:NormalExercise lang:r xp:100 skills:1,3
## Eingabe von Matrizen

Geben Sie die vorliegenden Daten des Autodatensatzes nun als Matrix mit dem Namen 'testMatrix'.

Preis       Alter (in Jahren)       Kilometer
-------     -------                 -------
850         14                      252000
4400        8                       189000
14250       2                       86000

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


