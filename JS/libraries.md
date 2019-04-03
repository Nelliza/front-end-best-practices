1. **Ни в коем случае никакой файл библиотеки не редактировать. Если есть небольшая полезная либа, у которой не хватает небольшой правки, то нужно сделать fork и отдельно в зависимостях указать путь до своей версии**;

2. **Изучайте best-practices для крупных библиотек, которые вы используете в проекте**:
    >Например:
    > * для Angular-а есть: [руководство](https://github.com/mgechev/angularjs-style-guide/blob/master/README-ru-ru.md);
    > * для React-а есть: [руководство](https://github.com/airbnb/javascript/tree/master/react) или [это](https://medium.com/lexical-labs-engineering/redux-best-practices-64d59775802e);

3. **Модули должны использоваться из node_modules**;
    > Если используются дополнительные модули, то в package.json должны быть прописаны пути до локальных модулей, которые вы установили.

4. **Когда для поставленной задачи можно использовать библиотеку, никогда не делать выбор за первой попавшейся в поисковике. Надо сначала проанализировать как минимум 3 самых популярных решения и для каждого:**
    > * есть ли у нее отдельный публичный репозиторий и где он находится;
    > * есть ли у нее документация и описывает ли она использование библиотеки для нашей поставленной проблемы;
    > * если доков нет или нет нормального описания, надо внимательно изучить код библиотеки и понять API, которое позволит решить проблему;
    > * осмотреть открытые `issue` (хотя бы пробежать глазами по первым двум страницам) и изучить те, что могут повлиять на работу библиотеки в контексте нашего проекта;
    > * принять решение о использовании библиотеки только совместно с другими равными по статусу или старшими фронтенд-разработчиками из команды.