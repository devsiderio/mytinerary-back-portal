
# MyTinerary API ⚙️

API REST desarrollada para gestionar la lógica de negocio, autenticación y persistencia de datos de MyTinerary.

**🔗 Frontend asociado:** [https://github.com/devsiderio/mytinerary-portal](https://github.com/devsiderio/mytinerary-portal)  
**🔗 Demo:** [https://mytinerary-portal.vercel.app](https://mytinerary-portal.vercel.app)

---

## 🚀 Tecnologías

- **Node.js** + **Express** — Servidor rápido y escalable
- **MongoDB** + **Mongoose** — Base de datos NoSQL con modelado robusto
- **Passport.js** — Estrategia de autenticación JWT
- **Bcrypt** — Encriptación segura de contraseñas
- **JOI** — Validación de datos de entrada
- **CORS** — Configuración segura de orígenes cruzados
- **Dotenv** — Gestión de variables de entorno

---

## 📋 Modelos de datos

| Recurso | Descripción |
|---------|-------------|
| **User** | Autenticación, roles (user/admin), datos de perfil |
| **City** | Destinos turísticos con foto, país y descripción |
| **Itinerary** | Planes de viaje (precio, duración, likes, tags, autor) |
| **Activity** | Actividades específicas dentro de cada itinerario |
| **Comment** | Comentarios anidados de usuarios en itinerarios |

---

## 🔐 Features de seguridad

- Autenticación JWT (Bearer token)
- Middleware de autorización por roles (user/admin)
- Validación estricta de inputs con JOI
- Hasheo de passwords con bcrypt
- Protección de rutas sensibles

---

## 🛠️ Instalación local

```bash
# Clonar repositorio
git clone https://github.com/devsiderio/mytinerary-back-portal.git

# Entrar a la carpeta descargada
cd mytinerary-back-portal

# Instalar dependencias
npm install

# Configurar variables de entorno
crear manualmente el archivo .env

```

## Configuración del archivo .env:

```
PORT=8080
LINK_DB=mongodb+srv://usuario:password@cluster.mongodb.net/mytinerary-db
SECRET_KEY=tu_clave_secreta_segura
```

## Bash
```
npm run dev
```
## Autor

- Mariano J. Portal [@devsiderio](https://github.com/devsiderio)

