## 1. Запустите локальный веб-визуализатор репозитория и сделайте так, чтобы в нём отображалось нормальное описание репозитория.
Сначала войдём в wsl.
```
wsl 
```
Потом установим руби.
```
sudo apt-get install ruby 
sudo apt install libcgi-pm-perl 
sudo apt install libcgi-pm-perl --fix-missing 
```
Редактируем описание репозитория в папке .git/description
```
The new description.
```
Далее перезапускаем веб-визуализатор по команде
```
git instaweb --httpd=webrick
```
И по порту 1237 (а по дефолту 1234) находим веб-визуализатор
![](1.bmp)