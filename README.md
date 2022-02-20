## **Repository 1 JSON**
**4. Создать внешний репозиторий c названием JSON**
- **version via GitHub**:
	- push `NEW` button
	- enter repository name "JSON"
	- choose a `README file` option
	- push `Create repository` button
	-
- **version via Terminal for authenticated users only**:
	- use API link to send POST request:
[API link](https://api.github.com/)
	- enter the command:
```bash
curl -u "YourGitHubName" https://api.github.com/user/repos -d "{"name":"JSON","public": true}"
```
	- enter your password
	- under response find URL named "clone_url": and copy it
	- go to GitHub by copied link and find your new repository

- **version via Terminal for any user**:
```bash
mkdir JSON
cd JSON
git init
touch README.md
git commit -m "commit of json"
```
```bash
git remote add origin 
git@github.com:YourGitHubName/<JSON>.git
```
```bash
curl -u YourGitHubName:YourTokinORYourPassword https://api.github.com/user/repos -d '{"name":"JSON"}'
```

**5. Клонировать репозиторий JSON на локальный компьютер**
- copy link of repository under `Code` button
![Commit button](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- commands:
```bash
cd MyDirectory	//where new project to be placed locally
git clone + <copied link>
```

**6. Внутри локального JSON создать файл “new.json”**
```bash
cd JSON
touch new.json
```
**7. Добавить файл под гит**
```bash
git add new.json // to add exact file
git add . // to add all files
```
**8. Закоммитить файл**
```bash
git commit -m "json commit"
```
**9. Отправить файл на внешний GitHub репозиторий**
```bash
git status
git push
```
**10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON**

```bash
cd JSON
vim new.json
```
- enter json data:
[Json data](https://github.com/Olga-Ivasenko/JSON/blob/27513d59fa33744fef1ea328b0a6ed88cbe8a368/new.json)

**11. Отправить изменения на внешний репозиторий**
```bash
git status
git commit -m "new json changes" // if all added files
git commit -m "new json changes" new.json // if selected file
git push
```

**12. Создать файл preferences.json**
```bash
cd JSON
touch preferences.json
```

**13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON**
```bash
cd JSON
vim preferences.json
```
- enter json data:
[Json data](https://github.com/Olga-Ivasenko/JSON/blob/27513d59fa33744fef1ea328b0a6ed88cbe8a368/preferences.json)


**14. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON**
```bash
cd JSON
touch sklls.json
vim sklls.json // or without touch but save before closing
```
- enter json data
[Json data](https://github.com/Olga-Ivasenko/JSON/blob/27513d59fa33744fef1ea328b0a6ed88cbe8a368/skills.json)

**15. Отправить сразу 2 файла на внешний репозиторий**
```bash
cd JSON
git status
git add skills.json preferences.json
git status
git commit -m "add two files"
git push
```
**16. На веб интерфейсе создать файл bug_report.json**
- go to GitHub, repository you`ve created
- push `Add File` dropdown button
- choose `Create new file`
![Commit button](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture4.jpg)
- name your file "bug-report.json"

**17. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- choose `Edit new file` tab
- enter \{} to the edit field of the file
- choose `Preview` tab
- push `Commit your file` button
![Commit button](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture3.jpg)

**18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON**
- go to main branch of repository
- step on your file "bug-report.json"
- choose `edit` pictogram
![how to find Edit](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture1.jpg)
- enter json data:
[Json data](https://github.com/Olga-Ivasenko/JSON/blob/27513d59fa33744fef1ea328b0a6ed88cbe8a368/bug_report.json)

**19. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- go down of edit file page
- optional: add description
- click `Commit changes` button
![Commit button](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture2.jpg)

**20. Синхронизировать внешний и локальный репозиторий JSON**
```bash
git fetch ---all
git status
git merge
git push

```



