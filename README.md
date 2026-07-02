# Fauna Django

Aplicació Django per gestionar fauna, espècies i observacions de camp. Inclou models d’animals, seguiment geogràfic, comportament i estat de salut, amb API REST per integrar dades ecològiques en sistemes externs. Projecte modular, escalable i orientat a recerca i conservació.

## Funcionalitats
- Registre d’animals (espècie, identificador, estat de salut)
- Observacions amb data, coordenades i notes
- API REST amb Django REST Framework
- Estructura preparada per ampliar amb mapes, filtres i dashboards

## Requisits
- Python 3.12
- Django 5+
- Django REST Framework

## Instal·lació
```bash
pip install django djangorestframework
django-admin startproject wildlifemonitor .
python manage.py startapp animals
