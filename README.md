1. На локальном репозитории сделать ветки для:
- Postman
```
git branch Postman
```
- Jmeter
```
 git branch Jmeter
```
- CheckLists
```
git branch CheckLists
```
- Bag Reports
```
git branch Bag_Reports
```
- SQL
```
git branch SQL
```
- Charles
```
git branch Charles
```
- Mobile testing
```
git branch Mobile_testing
```
2. Запушить все ветки на внешний репозиторий -
```
git push -all
```
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
```
 git checkout Bag_Reports
touch BadReport.txt
vim BadReport.txt
```
|Stucture | Стурктура|  
|--- | ---|  
|ID | Номер|  
Summary | Описание  
STR | Шаги воспроизведения  
Actual_result | Фактический результат  
Expected_result | Ожидаемый резульат  
Environment | Окружение  
Build | Версия  
Severity | Серьезность  
Priority | Приоритет  
Attachments | Приложение

4. Запушить структуру багрепорта на внешний репозиторий
```
 git add . 
git commit -m "new touch txt"
git push origin Bag_Reports
```
5. Вмержить ветку Bag Reports в Main
```
 [Compare & pull request] - [create pull request] - [Merge pull request] -[confirm merge]
```
6. Запушить main на внешний репозиторий.
```
git checkout main 
git pull
```
7. В ветке CheckLists набросать структуру чек листа.
```git checkout CheckLists
touch CheckLists.txt
vim CheckLists.txt
```
Title  
	Actual_result  
	Expected_result  
	Attachments  

8. Запушить структуру на внешний репозиторий 
```
 git add .
git commit -m "new touch txt"
git push origin CheckLists
```
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
```
 [Compare & pull request] - [create pull request] - [Merge pull request] -[confirm merge]
```
10. Синхронизировать Внешнюю и Локальную ветки Main
```
git checkout main 
git pull
```
