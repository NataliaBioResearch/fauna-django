# Fauna Django
Aplicació Django per gestionar fauna, espècies i observacions de camp. El projecte proporciona una base robusta per a sistemes de monitorització ambiental, recerca en biodiversitat i seguiment d’espècies, amb una API REST preparada per integrar dades en aplicacions externes.

## Funcionalitats
- Registre d’animals (espècie, identificador, estat de salut)
- Observacions amb data, coordenades i notes
- API REST amb Django REST Framework
- Arquitectura modular i escalable
- Preparat per ampliar amb mapes, filtres, dashboards o integracions GIS

## Tecnologies utilitzades
- Python 3.12
- Django 5+
- Django REST Framework
- GitHub Codespaces (entorn de desenvolupament)

## Instal·lació i execució

### Instal·la les dependències
```bash
pip install django djangorestframework
Crea el projecte Django
bash
django-admin startproject wildlifemonitor .
python manage.py startapp animals
Executa el servidor
bash
python manage.py runserver
Desenvolupament en Codespaces
Aquest projecte es desenvolupa en GitHub Codespaces, utilitzant un entorn VS Code al núvol amb sincronització automàtica via Git. Permet treballar des de qualsevol dispositiu sense configuracions locals.

Estructura del projecte
bash
fauna-django/
│
├── animals/
│   ├── models.py
│   ├── views.py
│   ├── serializers.py
│   ├── urls.py
│
├── wildlifemonitor/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── manage.py
└── README.md
Llicència
MIT License
