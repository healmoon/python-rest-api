python-rest-api
задание:
Вам предстоит доработать интернет-магазин.

Будет необходимо:

a. апи для создания продукта;
b. апи для получения страницы продуктов;
c. апи для получения продукта по его ID;
d. написать в readme.md инструкцию, в ней должно быть:
— как запустить сервер;
— как создать продукт;
— как получить все продукты;
— как получить продукт по id.

для развертывание проекта выполните следующие команды:
склонируйте репозиторий к себе на компьютер или скачайте проект zip файлом.
git clone https://github.com/healmoon/python-rest-api.git
создайте виртуальное окружение:
python -m venv myenv
source myenv/bin/activate # для Linux и macOS
myenv\Scripts\activate # для Windows
где myenv — это название вашего виртуального окружения.
установите зависимости pip install -r requirements.txt
в консоли зайдите в папку проекта и оттуда запустите приложение командой >> python main.py

инструкция к API интернет магазина в Postman:

Создать продукт:
1. http://127.0.0.1:5000/api/v1/product
   в Body указать {"id": "str", "name": "str", "price": 0.0}
   использовать метод POST
   
Запросить продукт:
3. http://127.0.0.1:5000/api/v1/product?page=0&limit=10
   использовать метод GET
   
Запросить продукт по id:
4. http://127.0.0.1:5000/api/v1/product/id
   использовать метод GET

Создать заказ:
5. http://127.0.0.1:5000/api/v1/order
   в Body указать {"product_ids": ["1", "2"]}
   использовать метод POST

Запросить заказ:
6. http://127.0.0.1:5000/api/v1/order?page=0&limit=10
   использовать метод GET
   
Запросить заказ по id:
7. http://127.0.0.1:5000/api/v1/order/id
   использовать метод GET