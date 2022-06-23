1. Создать внешний репозиторий c названием XML.
В GitHub нажать справа кнопку New > в названии Repository написать название XML >
вибрать пункт Public > поставить галочку рядом с Добавить файл README. Внизу нажать кнопку Создать репозиторий

2. Клонировать репозиторий XML на локальный компьютер.
https://github.com/Ishmariia/XML.git

3. Внутри локального XML создать файл “new.xml”.
touch new.xml
 
 4. Добавить файл под гит.
git add .
 
 5. Закоммитить файл.
git commit -m "add new.xml file"

6. Отправить файл на внешний GitHub репозиторий.
git push

7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
 vim new.xml
<?xml version="1.0" encoding="UTF-8"?>
<personal>
 <FullName>Severova Irma Leonidovna</FullName>
  <Pets>No</Pets>
   <DesiredSalary>800,900,1000</DesiredSalary>
</personal>

8. Отправить изменения на внешний репозиторий.
git add .
git commit -m "change file new.xml"

9. Создать файл preferences.xml
touch preferences.xml
 
 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
 vim preferences.xml
<?xml version="1.0" encoding="UTF-8"?>
<Several>
 <FavoriteMovie>1+1</FavoriteMovie>
 <FavoriteTVseries>Friends</FavoriteTVseries>
 <Favoritefood>pasta</Favoritefood>
 <Favoritetimeofyear>spring</Favoritetimeofyear>
 <Country>Spain</Country>

  11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
cat >> sklls.xml
<?xml version="1.0" encoding="UTF-8"?>
<Skills>
<Gitbash>true</Gitbash>
<Android_studio>true</Android_studio>
<GitHub>true</GitHub>
<Postman>true</Postman>
<Text_data_transfer_formats>Json,CSV,XML</Text_data_transfer_formats>
 
12. Сделать коммит в одну строку.
git add .
git commit -m  "new files preferences & skill"

  13. Отправить сразу 2 файла на внешний репозиторий.
git push

  14. На веб интерфейсе создать файл bug_report.xml.
В репозитории GitHub нажать на кнопку "add file"> выбрать create new file > создать bug_report.xml

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit changes в Github внизу

  16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
<?xml version="1.0" encoding="UTF-8"?>
<Bug_report>
<ID_696>
     <Title>Parameters of the "Send e-mail" button, do not send data to e-mail when the data is entered correctly</Title>
       <Severity> Major</Severity>
      <Priority> Medium </Priority> 
      <Environment> Xiaomi mi 9 Lite,  Android 10 </Environment>         
      <Precondition> Installed app on the device </Precondition>
      <STR>:  
         1. Open the APP
         2.Fill in the field with the data to send 
         3. Tap “Send Email” button
      </STR>
         
     <AR>: App return different links not related to sending email</AR>
     <ER>: App return  links related to sending emai</ER>
</ID_696>
</Bug_report>
 
  17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit changes в Github внизу

  18. Синхронизировать внешний и локальный репозиторий XML
git pull
