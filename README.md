# Deployment-Interface

Este repositorio contiene el **frontend preparado exclusivamente para el despliegue en Azure**.

---

## 📦 Descripción

Este proyecto es el frontend de [WHS Representaciones](https://github.com/DominidM/whsRepresentaciones), diseñado y organizado para una fácil integración y despliegue en servicios de Azure (Azure Static Web Apps, Azure App Service, etc).

---

## 🚀 Despliegue en Azure

### 1. Requisitos

- Node.js, Bun o el gestor de paquetes correspondiente (según el proyecto).
- Una cuenta de Azure y permisos para desplegar recursos.
- Acceso a este repositorio.

### 2. Pasos Generales

1. **Clona este repositorio:**
   ```sh
   git clone https://github.com/DominidM/frontend.git
   cd frontend
   ```

2. **Instala las dependencias:**
   ```sh
   bun install
   # O si usas npm:
   # npm install
   ```

3. **Genera el build de producción (carpeta dist/build):**
   ```sh
   bun run build
   # O si usas npm:
   # npm run build
   ```

4. **Despliega la carpeta generada (`dist` o `build`) en Azure:**
   - Puedes desplegar desde Azure Portal, Azure CLI, VS Code o configurando un workflow de CI/CD.

---

## ⚙️ Notas importantes

- **NO subas la carpeta `dist` ni `node_modules` al repositorio.** El build se genera en Azure durante el despliegue.
- El repositorio contiene únicamente el código fuente necesario para el frontend.
- Personaliza variables de entorno si tu despliegue lo requiere (consulta la documentación de tu servicio Azure).

---

## 🔗 Proyecto principal

- Repositorio principal: [whsRepresentaciones](https://github.com/DominidM/whsRepresentaciones)

---

## 📝 Licencia

Este proyecto sigue la licencia definida en el repositorio principal.
