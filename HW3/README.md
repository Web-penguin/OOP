# Что нужно для запуска?
Прописать в pom.xml проекта:
```sh
<dependency>
    <groupId>com.beust</groupId>
    <artifactId>jcommander</artifactId>
    <version>1.72</version>
</dependency>
```
# Что умеет?
1. Делит большое изображение на маленькие по черным линиям
2. В несколькох тредах выполняет манипуляции над маленькими изображениями, а именно, это может быть:
* Поворот на 90/180/270 градусов
* Вертикальное или горизонтальное отзеркаливание
3. Собирает из маленьких изображение большое в соответствующем порядке

# Как запускать?
Передавать в качестве аргументов командной строки следующие флаги:
* -i Путь до изображения
* -res Путь до результирующего файла ascii изображения
* -r Количество градусов для поворота маленьких ascii изображений
* -vm Вертикально отзеркаливать маленькие ascii изображения
* -hm Горизонтально отзеркаливать маленькие ascii изображения

# Пример
-i D:\OOP\HW2\src\main\java\example.png -res D:\OOP\HW2\src\main\java\result -hm
Означает получить большое ascii изображение из маленьких отзеркаленных горизонтально
Флаги -i, -res обязательны, так же обязателен только один из флагов -hm, -vm -rm.
Так же указывать путь до результата нужно без расширения: D:\OOP\HW2\src\main\java\result, а не D:\OOP\HW2\src\main\java\result.txt