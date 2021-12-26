# Javacore-homework4.1.2VisualVM

Please open 'ru.netology.JvmExperience' in VisualVm

22:25:55.325949800: loading io.vertx

22:25:55.400156500: loaded 0 classes

22:25:58.411750200: loading io.netty

22:25:59.962607500: loaded 2749 classes

22:26:02.963973200: loading org.springframework

22:26:02.969963100: loaded 0 classes

22:26:05.979236600: now see heap

22:26:05.979236600: creating 5000000 objects

22:26:06.349942600: created

22:26:09.350807400: creating 5000000 objects

22:26:09.759701800: created

22:26:12.857712900: creating 5000000 objects

22:26:13.189596700: created


С первого раза не запустились ни проект, ни visualVM. После плясок с бубном visualvm заработал.
Проект пересобрал в mavene, подгрузил нужные библиотеки, тоже все заработало. Но дальше есть несостыковки между 
логом и графиком. На картинке 1 видно, что в 22:25:55 загрузилось 267 классов, в логе loaded 0 classes
![1](https://github.com/Savser91/Javacore-homework4.1.2VisualVM/blob/master/1.png)

Далее картинка 2. Тоже несостыковка В логе для io.netty loaded 2749 classes. В visualVM 2929.
![2](https://github.com/Savser91/Javacore-homework4.1.2VisualVM/blob/master/2.png)

Далее картинка 3. В логе сообщение 22:26:02.969963100: loaded 0 classes для org.springframework, что соответствует картинке на графике. Ну и справа вверху выделил добавление 5000000 объектов в кучу 3 раза. 
![3](https://github.com/Savser91/Javacore-homework4.1.2VisualVM/blob/master/3.png)
Process finished with exit code 0
