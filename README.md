# Введение в тестирование Python 

Склонируйте репозитарий
```
git clone git@github.com:den-sad/backend_test_homework.git
```

Активируйте виртуальное окружение и установите зависисмости

```
cd backend_test_homework
python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt
```
## Запуск тестирования
Выполните команду pytest Результат не должен содержать ошибок

```
test_program.py::test_program PASSED
```

## Запуск тестирования с ошибкой

Добавьте в файл test_program.py в список "dir_files" название файла отсутствующего в каталоге

```
files_list = ['program.py', 'readme.md', 'error_file']
```

Запустите тестирование. Должна появиться ошибка c указанием на отсутсвующий файл

```
test_program.py:11: AssertionError
```
