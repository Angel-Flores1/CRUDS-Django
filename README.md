# 📋 CRUDS-Django - Guía de Inicio Rápido

## 🧾 Descripción del Proyecto

Una aplicación web desarrollada con Django que permite gestionar registros mediante un sistema CRUD completo. Ideal para administrar datos desde un panel intuitivo en el navegador.

Incluye autenticación, panel administrativo, gestión de tareas y perfiles de usuario.

---

## ✅ Requisitos Previos

- Python 3.10 o superior
- PostgreSQL (instalado y corriendo)
- Git (opcional, pero recomendado)
- Conexión a Internet para descargar dependencias

---

## 🚀 Guía de Instalación

### 1. Clonar o descargar el proyecto

**Opción A: Clonar el repositorio con Git**

```bash
git clone https://github.com/Angel-Flores1/CRUDS-Django.git
cd CRUDS-Django
Opción B: Descargar como ZIP

    Pulsa el botón verde "Code" → "Download ZIP"

    Extrae el archivo y abre una terminal dentro de la carpeta extraída

2. Crear y activar entorno virtual

python -m venv entorno_django

Activar entorno:

    Windows: entorno_django\Scripts\activate

    macOS/Linux: source entorno_django/bin/activate

3. Instalar dependencias

pip install -r requirements.txt

4. Configurar base de datos PostgreSQL

Asegúrate de tener PostgreSQL instalado y un usuario configurado. Luego edita el archivo .env (o configura tus variables de entorno) con estos datos:

DB_NAME=snake
DB_USER=postgres
DB_PASSWORD=postgres
DB_HOST=localhost
DB_PORT=5432

5. Aplicar migraciones

python manage.py migrate

6. Crear superusuario (opcional)

python manage.py createsuperuser

Sigue las instrucciones para asignar nombre de usuario, correo y contraseña.
7. Ejecutar el servidor de desarrollo

python manage.py runserver 9090

🌐 Acceso a la Aplicación

    Aplicación principal: http://localhost:9090/

    Panel administrativo: http://localhost:9090/admin/

🛑 Para detener el servidor

Presiona Ctrl + C en la terminal.
⚠️ Solución a problemas comunes
❌ ModuleNotFoundError: No module named 'django'

    Asegúrate de tener activado el entorno virtual.

    Ejecuta pip install -r requirements.txt.

❌ OperationalError: could not connect to server

    PostgreSQL no está corriendo. Inícialo con: sudo systemctl start postgresql

    Verifica que la IP/puerto en DB_HOST y DB_PORT sean correctos.

❌ python no se reconoce como comando

    Asegúrate de marcar "Add Python to PATH" durante la instalación de Python.

    O usa python3 si estás en Linux/macOS.

🧠 Nota final

Este proyecto ya está configurado para usar PostgreSQL. Si prefieres SQLite para desarrollo rápido, puedes cambiar el ENGINE y NAME en settings.py.
🤝 Contribuciones

¡Las contribuciones son bienvenidas! Puedes abrir un issue o enviar un pull request.
