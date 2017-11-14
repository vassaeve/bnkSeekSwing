#Программа по работе (CRUD) со справочником БИК. 
 
 
 - загрузка файла `BNKSEEK.dbf` и сопутствующих `PZN.DBF, REG.DBF, TNP.DBF, UER.DBF`;
 - Создание, удаление, редактирование записей справочника;
 - Фильтрация списка по полям БИК, регион, тип.
 
  Используемая БД - `hsqldb`, версия `2.4.0`
  
  Возможно использование любой другой, на выбор пользователя, БД. 
  Настройки соединения - см. `src/main/resources/liquibase.properties`

 Сборка и инициализация БД:
 - `mvn clean install`


 Процедура инициализации БД:

 - `mvn liquibase:update`

Запуск:

- скопировать каталог `data` после инициализации БД в `target`
- из каталога target: `java -jar BankSeekSwing-0.1.jar`
