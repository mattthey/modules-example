# Обучалка для java mosules

Компилируем все с исходниками и помещаем в папку out
> javac src/main/java/module-info.java src/main/java/com/github/mattthey/main/Main.java -d out

```bash
java --module-path {путь до директории с модулем} --module {имя модуля}/{главный класс модуля}
java --module-path out --module main/com.github.mattthey.main.Main
```

## Полезные ссылки
https://metanit.com/java/tutorial/11.1.php

https://habr.com/ru/post/499872/

https://jenkov.com/tutorials/java/modules.html#multi-java-version-module-jar-files

https://youtu.be/hEnvRXNyDgI
