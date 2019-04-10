---
layout: post
title: "Лабораторная работа №1"
---

# Лабораторная работа №1

Работа посвящена созданию этого сайта.

На страницах должны быть использованы следующие конструкции markdown:
+ текстовый список;
+ ссылки на внешние ресурсы;
+ вставка изображения;
+ программный код с подсветкой.

Пример программного кода с подсветкой:

```python
import csv
authorsEmail = {}
with open( "calculator.history", "rt" ) as file:
    reader = csv.reader( file )
    for row in reader:
        name = row[0]
        email = row[1]
        if name not in authorsEmail:
            authorsEmail[ name ] = []
        emailList = authorsEmail[ name ]
        if email not in emailList:
            emailList.append( email )
for name, email in authorsEmail.items():
    print name, email
```
