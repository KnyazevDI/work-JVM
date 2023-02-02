# Работа JVM по грфикам visualVM

![схема](D:\IdeaProjects\JVM\работа visualVM.JPG)

1. Начинает работать ClassLoader, загружаются системные кллассы. Классы связываются и инициализируются.
Классы загружаются в Metaspace.

2. Первый запуск метода  loadToMetaspaceAllFrom, загружаается 529 классов "io.vertx".

3. Второй запуск loadToMetaspaceAllFrom, загружаается 2117 классов "io.netty".

4. Третий запуск loadToMetaspaceAllFrom, загружаается 869 классов "org.springframework".

5. Первый запуск createSimpleObjects, в куче создаются 5_000_000 объектов.

6. Второй запуск createSimpleObjects, в куче создаются еще 5_000_000 объектов.

7. Третий запуск createSimpleObjects, в куче создаются еще 5_000_000 объектов.

8. работа сборщика мусора.