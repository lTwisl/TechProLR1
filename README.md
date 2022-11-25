#Лабораторная работа №1 

##Выполнил студенты: Белов Александр, Деревянченко Кирилл, Федосеев Вячеслав. Группы М3О-406С-19 

Ход работы Git это распределенная система контроля версий в которой есть множесто премуществ например для совершенияя операций необходимы только локальные файлы и ресурсы тоесть информация в сети с других компьютеров не нужна, также Git следит за целостностью файлов. 

Этапы работы: 

1) Установка Gita и его первоначальная настройка. Перевым делом что нужно сделать после установки это указать ваше имя и адрес почты используя команды git config user.name “Вася Пупкин” git config user.email vpupkin@exmple.com После нужно выбрать сервер для центрального репозитория мы будем использовать GitHub 
1) Создание репозитория TechProLR1 в нём же создание файла LR1.txt с содержимым “Morning” 

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.001.jpeg)

3) Добавление членов бригады к репозиторию 

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.002.jpeg)

4) Создание веток каждому члену бригады. Далее с помощью команды git clne [url] каждыйскачивает репозиторий себе на компьютер. После каждый изменяет строку Morning на Morning *name*, когда были сделаны изменения в файле нужно отправить изменения на сервер. Чтобы отправить на сервер в начале нужно вести git status, увидив что наш изменённый файл не отслеживается вводим git add. 

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.003.jpeg)

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.004.jpeg)

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.005.jpeg)

5) Переходим на свою ветку с помощью команды git checkout [название ветки], теперь делаем комит git commit -m “мой первый коммит” и отправляем на сервер git push 
5) Далее производим слияние всех веток в мастер ветку. Для этого нужно перейти в ветку мастер и там уже производить слияние с помощью команды git merge “название ветки”. Но что мы видим происходит конфликт это связанно с тем что надписи находятся на одной строчке 

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.006.jpeg)

7) Создаем docx и md файлы в репозитории и сравниваем удобства работы с ними 

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.007.jpeg)

8) Далее откатываемся к коммиту где объединяли все ветки с поощью команды git revert “hash” 

![](Aspose.Words.11446527-8c4d-4b58-997b-eb888162ec35.008.jpeg)

9) Смотрим историю работы с помощью команды git log –graph –pretty=oneline – abbrev-commit и что мы видим что после отката создался новый комит с инвертированными изменения. 

В ходе лабараторной работы мы приобрели и отработали новые навики, такие как: совместная работа в команде, использование системы контроля версий и цикл совместной разработки. Даный опыт работы позволил нам сделать следующие выводы: при совместной работе нужно использовать систему контроля версий так как она вомного раз упрощает процесс совместной разработки, самый неудобный файл для работы это файл docx так как мы не можем наблюдать содержимое файла в GitHub, а также он перезаписывается полностью, а не построчно. 
