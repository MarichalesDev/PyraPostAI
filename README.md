# PyraPostAI
PyraPost AI | Automatización inteligente de contenido para redes sociales. Genera copys con IA, gestiona publicaciones y entrega reportes de métricas profesionales. Diseñado por PyraStack para potenciar el crecimiento digital de marcas y agencias.
---

## 🛠️ Instalación Rápida (Quick Start)

Sigue estos pasos para tener el proyecto funcionando en menos de 5 minutos.

Creen un archivo llamado requirements.txt en la raíz de la carpeta del proyecto y peguen esto:

Plaintext
fastapi==0.110.0
uvicorn==0.27.1
groq==0.5.0
httpx==0.27.0
python-dotenv==1.0.1

2. Paso a paso para iniciar el proyecto
Sigan este orden exacto para evitar errores de rutas o librerías faltantes:  

Parte A: Backend (El cerebro)
Crear el entorno virtual: python -m venv venv.  

Activar el entorno:

Si usan Git Bash: source venv/Scripts/activate.  

Si usan CMD: venv\Scripts\activate.  

Instalar librerías: pip install -r requirements.txt.  

Encender el servidor: uvicorn app_web:app --reload.  

Parte B: Frontend (La interfaz)
Entrar a la carpeta: cd frontend (o como se llame la carpeta del cliente).  

Instalar Node: npm install.  

Encender la interfaz: npm run dev.  

🧠 3. ¿Por qué hacemos cada cosa?
Aquí les explico la lógica de nuestro flujo de trabajo para que sepan qué estamos tocando:  

Sobre el proceso:
Venv: Lo usamos para que las librerías de este proyecto no se mezclen con otras que tengan en su PC. Es nuestra "burbuja" de desarrollo.  

npm install: Descarga todas las herramientas visuales (Vite, React/Vue) para que la página se vea profesional.  

--reload: Esta bandera en Uvicorn es clave; hace que el servidor se reinicie solo cada vez que guardamos un cambio en el código.  

Sobre las librerías:
FastAPI: Es el framework que recibe las peticiones del frontend. Es súper rápido y fácil de usar.  

Uvicorn: Es el motor que permite que Python corra como un servidor web.  

Groq: Es nuestra conexión directa con la IA para generar los textos e imágenes de los posts en segundos.  

HTTPX: Lo usamos para que nuestro servidor pueda "hablar" con otras APIs externas.  

Python-dotenv: Fundamental para la seguridad; lee nuestras API Keys desde el archivo .env sin exponerlas en el código.  

⚠️ Puntos clave a considerar
Doble terminal: Siempre vamos a tener dos terminales abiertas: una para el backend (puerto 8000) y otra para el frontend (puerto 5173).  

El archivo .env: No olviden pedírmelo o crearlo con sus propias llaves. Sin esto, la IA de Groq no va a responder.  

Node.js: Asegúrense de tener instalado Node.js en su sistema, de lo contrario los comandos npm no funcionarán.  

¡Cualquier duda me avisan y lo revisamos de una!
