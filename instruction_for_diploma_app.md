Шаг 1: Установка необходимых библиотек
Установите необходимые библиотеки через терминал с помощью командной строки:
	pip install fastapi uvicorn dill pandas pydantic

Шаг 2: Запуск FastAPI приложения
Запустите приложение через терминал с помощью командной строки:
	uvicorn app:app --reload
Теперь приложение должно быть доступно по адресу http://127.0.0.1:8000

Шаг 3: Тестирование приложения
	1 Тестирование через браузер или Postman:
 		◦ Перейдите на http://127.0.0.1:8000/status для проверки статуса.
 		◦ Перейдите на http://127.0.0.1:8000/version для проверки версии модели.
 	2 Тестирование POST-запроса: В Postman создайте новый POST-запрос к http://127.0.0.1:8000/predict с JSON телом, например:
{  
	"session_id": "9055434745589932991.1637753792.1637753792",
	"client_id": "2108382700.1637753791",
	"visit_date": "2021-11-24",
	"visit_time": "14:36:32",
	"visit_number": "1",
	"utm_source": "ZpYIoDJMcFzVoPFsHGJL",
      "utm_medium": "banner",
      "utm_campaign": "LEoPHuyFvzoNfnzGgfcd",
      "utm_adcontent": "vCIpmpaGBnIQhyYNkXqp",
      "utm_keyword": "puhZPIYqKXeFPaUviSjo",
      "device_category": "mobile",
      "device_os": "Android",
      "device_brand": "Huawei",
      "device_model": "",
      "device_screen_resolution": "360x720",
      "device_browser": "Chrome",
      "geo_country": "Russia",
      "geo_city": "Zlatoust"
}
