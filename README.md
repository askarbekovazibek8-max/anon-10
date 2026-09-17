# AnonSocial & Map

Анонимная социальная сеть на Django с лентой публикаций, анонимными ID, друзьями и приватным обменом геолокацией через Leaflet/OpenStreetMap.

## Запуск

```powershell
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Откройте `http://127.0.0.1:8000/`. Админ-панель доступна по адресу `/admin/` после создания администратора командой `python manage.py createsuperuser`.

Локация пользователя сохраняется только после отправки координат. На карте отображаются координаты только подтверждённых друзей.