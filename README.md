# LinkStash

Aplicación web simple hecha con Django para guardar enlaces útiles.

La idea es mantener el proyecto chico: crear enlaces, buscarlos y eliminarlos.
No usa JavaScript ni dependencias de frontend.

## Funciones

- Guardar un enlace con título, URL y una nota opcional
- Buscar por título o nota
- Abrir enlaces desde la lista
- Eliminar registros

## Instalación

```bash
git clone <tu-repo>
cd linkstash

python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Abrí:

```text
http://127.0.0.1:8000/
```

## Estructura

```text
linkstash/
├── bookmarks/
├── config/
├── static/
├── templates/
├── manage.py
└── requirements.txt
```

## Notas

El proyecto usa SQLite para desarrollo. La `SECRET_KEY` puede pasarse por variable de entorno:

```bash
export DJANGO_SECRET_KEY="cambia-esto"
```
