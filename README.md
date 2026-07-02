# Fauna Django
Aplicació Django per gestionar fauna, espècies i observacions de camp. El projecte proporciona una base robusta per a sistemes de monitorització ambiental, recerca en biodiversitat i seguiment d’espècies, amb una API REST preparada per integrar dades en aplicacions externes.

## Funcionalitats
Registre d’animals (espècie, identificador, estat de salut)  
Observacions amb data, coordenades i notes  
API REST amb Django REST Framework  
Arquitectura modular i escalable  
Preparat per ampliar amb mapes, filtres, dashboards o integracions GIS

## Tecnologies utilitzades
Python 3.12  
Django 5+  
Django REST Framework  
GitHub Codespaces (entorn de desenvolupament)

## Instal·lació i execució
Instal·la les dependències:  
pip install django djangorestframework

Crea el projecte Django:  
django-admin startproject wildlifemonitor .  
python manage.py startapp animals

Executa el servidor:  
python manage.py runserver

## Desenvolupament en Codespaces
Aquest projecte es desenvolupa en GitHub Codespaces, utilitzant un entorn VS Code al núvol amb sincronització automàtica via Git. Permet treballar des de qualsevol dispositiu sense configuracions locals.

## Estructura del projecte
fauna-django/  
├── animals/  
│ ├── models.py  
│ ├── views.py  
│ ├── serializers.py  
│ ├── urls.py  
├── wildlifemonitor/  
│ ├── settings.py  
│ ├── urls.py  
│ └── wsgi.py  
├── manage.py  
└── README.md

## API REST
El projecte inclou una API REST per consultar i gestionar dades de fauna.  
Endpoints previstos:  
GET /animals – Llista d’animals  
POST /animals – Crear un animal  
GET /animals/<id> – Detall d’un animal  
GET /observations – Llista d’observacions  
POST /observations – Crear una observació  
La API està dissenyada per integrar-se amb aplicacions externes de recerca, monitorització ambiental o sistemes GIS.

## Roadmap
Fase 1 – Models i API bàsica  
Fase 2 – Autenticació i permisos  
Fase 3 – Filtres avançats i cerca  
Fase 4 – Dashboard amb gràfics  
Fase 5 – Integració amb mapes (Leaflet o Mapbox)  
Fase 6 – Exportació de dades (CSV, JSON)

## Badges
Status: En desenvolupament  
Tecnologia: Django 5  
Entorn: GitHub Codespaces  
Llicència: MIT

## Contributing
Les contribucions són benvingudes.  
Per participar:  
1. Fes un fork del repositori  
2. Crea una branca amb la funcionalitat o millora  
3. Envia un pull request  
4. Explica clarament els canvis realitzats  
Aquest projecte segueix bones pràctiques de desenvolupament i revisió de codi.

## Changelog
v0.1 – Creació del projecte, models inicials i API bàsica  
v0.2 – Afegits endpoints d’observacions  
v0.3 – Millores en l’estructura del projecte i documentació  
v0.4 – Preparació per a integració amb mapes  
v0.5 – Afegida secció de contribució i roadmap  
v0.6 – Afegides seccions FAQ, Limitacions i Objectius científics  
v0.7 – Afegides seccions Crèdits, Arquitectura, Glossari i Models de dades  
v0.8 – Afegides seccions Seguretat, IA, Exemples d’ús, Roadmap científic, Metodologia de camp i FAIR

## Sobre el projecte
Fauna Django és un projecte orientat a recerca i monitorització ambiental.  
L’objectiu és proporcionar una base flexible per gestionar dades de fauna i observacions de camp, amb possibilitat d’integrar-se en sistemes més grans de biodiversitat, conservació o gestió d’ecosistemes.

## Captures de pantalla
Aquesta secció mostrarà exemples visuals del projecte quan estigui més avançat.  
Es poden incloure:  
Pantalla principal  
Llista d’animals  
Detall d’un animal  
Dashboard de dades  
Mapa d’observacions

## FAQ
Puc utilitzar aquest projecte per a recerca?  
Sí, està pensat per a projectes de recerca, seguiment d’espècies i estudis de biodiversitat.

És necessari tenir coneixements avançats de Django?  
No, el projecte està estructurat perquè sigui fàcil d’entendre i ampliar.

Es pot integrar amb mapes?  
Sí, el roadmap inclou integració amb Leaflet o Mapbox.

Hi ha previst suport per a usuaris i permisos?  
Sí, està contemplat a la fase 2 del roadmap.

## Limitacions actuals
No inclou autenticació ni permisos avançats.  
No hi ha interfície gràfica, només API.  
La gestió de mapes encara no està implementada.  
No hi ha sistema de filtres avançats ni cerca.  
Les exportacions de dades estan planificades però no disponibles.

## Objectius científics del projecte
Facilitar la recollida i gestió de dades de fauna per a estudis de biodiversitat.  
Permetre l’anàlisi temporal i espacial d’observacions.  
Integrar dades en sistemes GIS per a recerca ecològica.  
Donar suport a projectes de conservació i seguiment d’espècies.  
Crear una base de dades estructurada per a investigació ambiental.

## Crèdits
Desenvolupament: Gaia Natalia Ràfols  
Documentació: Equip de recerca i suport tècnic  
Inspiració: Projectes de biodiversitat, monitorització ambiental i ciència de dades  
Tecnologies: Django, Python, GitHub Codespaces

## Arquitectura del sistema
El sistema segueix una arquitectura modular basada en Django:  
Models – Representen animals, espècies i observacions  
Serializers – Converteixen models a formats JSON per a la API  
Views – Gestionen la lògica de la API  
URLs – Defineixen els endpoints  
Settings – Configuració del projecte i aplicacions  
Aquesta arquitectura permet escalar el projecte, afegir noves funcionalitats i integrar-lo en sistemes més grans.

## Glossari de termes científics
Espècie – Categoria biològica que agrupa organismes similars  
Observació – Registre d’un animal en un lloc i moment determinat  
Coordenades – Posició geogràfica d’una observació  
Estat de salut – Condició física o clínica de l’animal observat  
Biodiversitat – Varietat d’espècies en un ecosistema  
Monitorització – Seguiment sistemàtic de dades ambientals o biològiques

## Models de dades explicats
Animal – Conté espècie, identificador i estat de salut  
Observació – Inclou data, coordenades, notes i referència a un animal  
Espècie – Pot incloure nom científic, nom comú i classificació  
Aquests models permeten estructurar dades de fauna de manera clara i interoperable.

## Seguretat de dades
El projecte segueix bones pràctiques de seguretat per garantir la protecció de la informació:  
Les dades es processen en entorns controlats.  
No es comparteixen dades sensibles sense consentiment.  
Es recomana utilitzar HTTPS en desplegaments de producció.  
Els models poden ampliar-se amb camps d'anonimització per protegir identitats.  
La integritat de les dades es manté mitjançant validacions i control d’errors.

## Integració amb IA
Fauna Django pot integrar-se amb models d’intel·ligència artificial per ampliar les capacitats del sistema:  
Classificació automàtica d’espècies a partir d’imatges.  
Detecció d’anomalies en observacions.  
Predicció de moviments o patrons de fauna.  
Anàlisi temporal i espacial amb models estadístics o de deep learning.  
Integració amb APIs externes per enriquir dades ambientals.

## Exemples d’ús
Projectes de seguiment d’espècies en reserves naturals.  
Estudis de biodiversitat en zones protegides.  
Monitorització de fauna urbana.  
Integració en aplicacions mòbils de ciència ciutadana.  
Sistemes de recollida de dades per a investigació ecològica.

## Roadmap científic
Fase A – Definició de models ecològics bàsics.  
Fase B – Integració amb dades ambientals (clima, hàbitat).  
Fase C – Anàlisi espacial avançada amb GIS.  
Fase D – Models predictius de distribució d’espècies.  
Fase E – Publicació de datasets FAIR per a recerca internacional.

## Metodologia de camp
Les observacions han de seguir protocols estandarditzats:  
Registrar data, hora i coordenades amb precisió.  
Anotar condicions ambientals rellevants.  
Evitar duplicats mitjançant identificadors únics.  
Respectar la fauna i evitar interferències.  
Utilitzar eines homologades per a la recollida de dades.

## Normes de qualitat FAIR
El projecte segueix els principis FAIR per garantir dades reutilitzables:  
Findable – Dades fàcilment localitzables amb metadades clares.  
Accessible – Accés obert o controlat segons necessitats del projecte.  
Interoperable – Ús d’estàndards com JSON, Darwin Core o Dublin Core.  
Reusable – Documentació completa per facilitar la reutilització científica.

## Llicència
MIT License
