# [забейболт.рф](http://забейболт.рф)
# [bmstu.fun](http://bmstu.fun)

Это сайт-помощник для студентов технических специальностей. Здесь представлена масса задач по различным дисциплинам.
* Выберите нужный раздел, найдите интересующую вас задачу (или воспользуйтесь поиском по стайту)
* Введите свои исходные данные
* Наслаждайтесь подробным решением именно вашей задачи!

После того как вы клонировали репозиторий, для запуска проекта вам понадобится выполнить следующие команды:
```bash
#копируем настройки и базу даных в том виде, в котором они необходимы для запуска проекта
cp BOLT_PROJECT/src/BOLT_PROJECT/settings-example.py src/BOLT_PROJECT/settings.py
cp BOLT_PROJECT/src/db-example.sqlite3 src/db.sqlite3
#устанавливаем pip3
sudo apt-get install python3-pip
#устанавливаем virtualenv
pip3 install virtualenv
cd BOLT_PROJECT
#создаём и активируем вируальное окружение
virtualenv --python=/usr/bin/python3.5 env
source env/bin/activate
#устанавливаем необходимые для работы приложения пакеты
pip3 install -r requirements.txt 
cd src/
python manage.py runserver
```
Наслаждаемся! Теперь наш проект доступен по адресу: localhost:8000
