# Обучалка для java mosules

## Компилируем все с исходниками и помещаем в папку out
> javac src/main/java/module-info.java src/main/java/com/github/mattthey/main/Main.java -d out

```bash
java --module-path {путь до директории с модулем} --module {имя модуля}/{главный класс модуля}
java --module-path out --module main/com.github.mattthey.main.Main
```

## Работа с jar-ом
### Создание
```bash
jar --create --verbose --file ./out/result.jar -C ./out .
```

### Выполнение
```bash
java --class-path ./out/result.jar com.github.mattthey.main.Main
```

## Опции module-info.java
- requires - указание название модуля от которого зависит наш модуль

## Полезные ссылки
https://metanit.com/java/tutorial/11.1.php

https://habr.com/ru/post/499872/

https://jenkov.com/tutorials/java/modules.html#multi-java-version-module-jar-files

https://youtu.be/hEnvRXNyDgI

https://www.baeldung.com/java-9-modularity

https://www.baeldung.com/maven-multi-module-project-java-jpms
