# home_about

Proyecto Django simple: página principal y página "acerca de".

## 🧩 Descripción

Este proyecto tiene el objetivo de mostrar un sitio web básico con:
- Página principal (`home`)
- Página de información (`about`)
- Plantillas en `templates/` (`home.html`, `about.html`, `_base.html`)
- App Django: `pages`

Se utiliza una configuración clásica de Django con rutas y vistas minimalistas.

## 📁 Estructura de archivos

- `manage.py` - comando del proyecto
- `db.sqlite3` - base de datos SQLite (local)
- `requirements.txt` - dependencias Python
- `base_project/` - configuración del proyecto Django
  - `settings.py`, `urls.py`, `wsgi.py`, `asgi.py`
- `pages/` - aplicación principal
  - `views.py`, `urls.py`, `models.py`, `tests.py`, `migrations/`
- `templates/` - plantillas HTML
  - `_base.html`, `home.html`, `about.html`

## 🚀 Requisitos

- Python 3.8+ (recomendado 3.10+)
- pip
- virtualenv (altamente recomendado)

## ⚙️ Instalación 

1. Clonar el repositorio:

```bash
git clone <URL-del-repositorio>
cd home_about
```

2. Crear y activar el entorno virtual (Windows):

```bash
python -m venv .venv
.venv\Scripts\Activate.ps1   # PowerShell
# o .venv\Scripts\activate.bat para cmd
```

3. Instalar dependencias:

```bash
pip install -r requirements.txt
```

4. Migrar base de datos:

```bash
python manage.py migrate
```

5. Ejecutar servidor local:

```bash
python manage.py runserver
```

6. Abrir navegador en: `http://127.0.0.1:8000/`

## 🛣️ Rutas y vistas

- `http://127.0.0.1:8000/` → `home` (vista de inicio)
- `http://127.0.0.1:8000/about/` → `about` (acerca de)

## 🧪 Pruebas

```bash
python manage.py test
```

## 🔧 Desarrollo

- Editar vistas en `pages/views.py`
- Modificar URLs en `pages/urls.py` y `base_project/urls.py`
- Añadir plantillas en `templates/`
- Agregar modelos en `pages/models.py`

## 📌 Buenas prácticas

- Usa `git` para control de versiones.
- Mantén el entorno virtual separado.
- No incluyas credenciales en el código.

## 📄 Licencia

Este proyecto es de ejemplo. Añadir licencia según necesidad (MIT, Apache 2.0, etc.).
