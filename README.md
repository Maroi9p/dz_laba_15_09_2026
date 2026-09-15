Создайте репозиторий git-task-system:
<img width="974" height="209" alt="image" src="https://github.com/user-attachments/assets/8150e053-4403-4c8a-8d1d-17fce39e81f5" />
Смоделируйте разработку простого TODO-трекера: Шаг 1: Создайте файл todo.py с базовым массивом задач tasks = [] . Закоммитьте с сообщением по стандарту Conventional Commits:
<img width="974" height="343" alt="image" src="https://github.com/user-attachments/assets/9473fbfc-8451-4160-9900-1dd5a74fb9cc" />
<img width="899" height="320" alt="image" src="https://github.com/user-attachments/assets/fed549b7-576a-4b68-bd8e-8c18a593aa29" />
Создайте файл config.py с настройками приложения и допишите в todo.py функцию добавления задачи add_task(name):
<img width="974" height="383" alt="image" src="https://github.com/user-attachments/assets/d9e076b5-02e6-48bf-bde2-95d4e2360372" />
<img width="974" height="532" alt="image" src="https://github.com/user-attachments/assets/4a44349f-03cb-426e-9238-f76a6b0252ba" />
<img width="974" height="274" alt="image" src="https://github.com/user-attachments/assets/f7966681-7218-415c-a6de-00346af116ce" />
Разделите эти изменения на два независимых атомарных коммита (сначала закоммитьте конфиг, затем логику в todo.py ):
<img width="974" height="364" alt="image" src="https://github.com/user-attachments/assets/4fb1c3d4-6495-4621-a928-283821b8fbbd" />
С помощью команд git log и git cat-file -p найдите хеш объекта blob файла config.py:
<img width="847" height="120" alt="image" src="https://github.com/user-attachments/assets/c2bdf05e-ef6e-4fa8-a448-689f9494aece" />
Переименуйте файл config.py в settings.py (содержимое не меняйте) и добавьте в индекс ( git add . ).
<img width="859" height="100" alt="image" src="https://github.com/user-attachments/assets/0346af0b-d3cb-450d-afd3-4e28bd3c2e2e" />
<img width="872" height="114" alt="image" src="https://github.com/user-attachments/assets/0c21e591-50ea-44a7-8f3e-2eab50ac213f" />
Проверьте хеш блоба нового файла. Сделайте вывод в отчете: почему при смене имени файла хеш блоба остался прежним?
<img width="969" height="320" alt="image" src="https://github.com/user-attachments/assets/a320a1d8-f309-4d89-8339-7529ad4a11d2" />

Не поменялся, потому что не закоммитили изменения. 
PS: В конце я все же закоммитил последние изменения, чтобы закинуть на hub.
