# Admin i NoQ
Första versionen av lösningen kommer från denna video: https://www.youtube.com/watch?v=XqkqbsdtoMI

## Installation av python och bibliotek
All installation nämns i videon. Detta är en sammanfattning med alla kommandon:

1. Installera python och verifiera att versionen är minst 3.10.*:
```
    python --version eller python3 --version på Mac
```    

2. Installera nödvändiga bibliotek
```
    pip install django django-ninja django-extensions
```
3. Skapa databas - om det saknas databas
```
    Navigera till biblioteket som innehåller manage.py
    python manage.py makemigrations
    python manage.py migrate
```
```
    Skapa admin user
    python manage.py createsuperuser
```
4. Starta webbservern 
```
    python manage.py runserver
```
5. Surfa till http://127.0.0.1:8000/admin 

## Översikt admin UI
![Alt text](admin.png)
## Detaljbild hosts
![Alt text](hosts.png)

## Programkod
Django framework innehåller så mycket standardfunktionalitet. Denna kod är i stort sett allt som krävs för hosts-tabellen ovan.

![Alt text](programkod.png)

För mer info se Django tutorial: https://docs.djangoproject.com/en/5.0/intro/tutorial01/