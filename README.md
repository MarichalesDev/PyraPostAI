## PyraPostAI
PyraPost AI | Automatización inteligente de contenido para redes sociales. Genera copys con IA, gestiona publicaciones y entrega reportes de métricas profesionales. Diseñado por PyraStack para potenciar el crecimiento digital de marcas y agencias.
---

### 1. 🛠️ Preparación del Entorno (Dependencias)
Creen un archivo llamado requirements.txt en la raíz y peguen esto:

```text
fastapi==0.110.0
uvicorn==0.27.1
groq==0.5.0
httpx==0.27.0
python-dotenv==1.0.1
```

***Parte A: Backend (Python)
Crear entorno virtual:*** ``` python -m venv venv ```

Activar entorno:

***Git Bash***: ``` source venv/Scripts/activate ```
 O para 
***CMD***: ``` venv\Scripts\activate ```

***Instalar librerías***: ``` pip install -r requirements.txt ```

***Parte B: Frontend (Node.js)
Entrar a la carpeta:*** ``` cd frontend ```

***Instalar dependencias:*** ``` npm install ```

## 2. 🔐 Configuración de Variables (.env)
***IMPORTANTE: Hagan esto antes de encender los servidores. Necesitan crear dos archivos manuales basándose en los (.env.example)***.

***A. Backend (/.env en la raíz)
Por privado les mando las keys/id's para no subir .env directamente al repo*** :

### Meta Centralizado (Cuentas de la agencia)

```text
FB_APP_ID=ID_PASADO_POR_JULIO
FB_APP_SECRET=SECRET_PASADO_POR_JULIO
INSTAGRAM_ACCOUNT_ID=IG_ID_PASADO_POR_JULIO
FB_ACCESS_TOKEN=TOKEN_PASADO_POR_JULIO
GROQ_API_KEY=TU_PROPIA_KEY
--------------------------------------------------------------------------
Tu llave de Groq: Entra a Groq Cloud, crea una API Key y pégala en tu .env.
```

***B. Frontend (/frontend/.env)***

``` VITE_FB_APP_ID=ID_DE_APP_JULIO ```

## 3. 🚀 Accesos y Permisos (Solo una vez)


### PASO MUY IMPORTANTE PARA TRABAJAR CON LA API DE INSTAGRAM Y FACEBOOK
<img width="905" height="416" alt="image" src="https://github.com/user-attachments/assets/59755d12-4274-4925-b2c6-c1e1d366feda" />

***Tester en app de Meta***: Revisen su correo o entren a ``` developers.facebook.com/requests ``` y acepten la invitación de PyraPost AI. Sin esto, el login les dará error de permisos.

## 4. ⚡ Ejecución del Proyecto
Siempre usaremos dos terminales abiertas simultáneamente:

***Terminal 1 (Backend):*** ``` uvicorn app_web:app --reload (Puerto 8000) ```

***Terminal 2 (Frontend):*** ``` cd frontend -> npm run dev (Puerto 5173) ```

## 5. 📚 Glosario Rápido (¿Por qué hacemos esto?)
***venv:*** Nuestra "burbuja" para que las librerías no choquen con otros proyectos.

***--reload:*** El servidor se reinicia solo al guardar cambios. Útil para desarrollo ágil.

***FastAPI & Uvicorn:*** El cerebro que recibe las peticiones y el motor que lo hace correr.

***Groq:*** Conexión con la IA para generar los copys en segundos.

***dotenv:*** Mantiene nuestras llaves seguras y fuera del código público.

### 💡 Nota rápida: Usaremos las cuentas de Instagram y Facebook que creé específicamente para el modo de desarrollo de PyraPost AI. Esto nos permite probar todas las funciones de Meta (hacer posts, programar, etc.) sin que cada uno pierda tiempo configurando cuentas profesionales desde cero.

¡Cualquier duda me avisan y lo revisamos de una!


