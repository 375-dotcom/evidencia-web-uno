# 📝 Evaluación Práctica: JavaScript — Web 1

¡Bienvenidos a la evaluación práctica del curso **Web 1**!  
En esta actividad pondrás a prueba tus conocimientos fundamentales de **JavaScript** y el manejo del flujo de trabajo con **Git y GitHub**.

---

## 🎯 Objetivo
Desarrollar la solución al ejercicio asignado en JavaScript, integrándolo en una estructura web básica y gestionando las versiones del código mediante buenas prácticas con Git.

> [!NOTE]
> La consigna o enunciado específico con el ejercicio asignado para cada estudiante se entregará en un documento/archivo independiente.

---

## 📋 Requisitos Previos
- Tener instalado [Git](https://git-scm.com/) en tu equipo.
- Contar con una cuenta activa en [GitHub](https://github.com/).
- Editor de código recomendado: [Visual Studio Code](https://code.visualstudio.com/).
- Navegador web moderno (Chrome, Firefox, Edge, etc.).

---

## 🚀 Instrucciones Paso a Paso

### 1. Hacer Fork del Repositorio
1. En la parte superior derecha de este repositorio en GitHub, haz clic en el botón **Fork**.
2. ⚠️ **MUY IMPORTANTE**: En la ventana de configuración del fork, **desmarca** la casilla:
   > `[ ] Copy the main branch only` *(Copiar solo la rama principal)*  
   Esto es indispensable para que tu fork incluya también la rama **`develop`**.
3. Haz clic en **Create fork**.

---

### 2. Clonar tu Repositorio Forkeado
Abre tu terminal (Git Bash, PowerShell o terminal de tu preferencia) y clona **tu propio fork** (no el repositorio original):

```bash
git clone https://github.com/TU-USUARIO/evidencia-web-uno.git
```

Luego entra a la carpeta del proyecto:

```bash
cd evidencia-web-uno
```

---

### 3. Pasarse a la Rama `develop`
Todas las modificaciones y entregas deben realizarse sobre la rama `develop`:

```bash
git checkout develop
```
*(O si usas versiones recientes de Git: `git switch develop`)*

Para comprobar que estás en la rama correcta:
```bash
git branch
```
*(Deberás ver un asterisco al lado de `* develop`)*.

---

### 4. Crear tu Carpeta y Archivos de Trabajo
Estando ubicado en la raíz del proyecto y en la rama `develop`:

1. Crea una carpeta nombrada con tu **nombre y apellido** (en minúsculas y separado por guion, por ejemplo: `juan-perez`).
2. Entra a tu carpeta y crea los siguientes dos archivos:
   - `index.html`: Estructura base HTML5 donde se visualizará o interactuará con el ejercicio.
   - `app.js` (o `index.js`): Código JavaScript donde implementarás la solución al ejercicio.

#### Estructura de carpetas esperada:
```text
evidencia-web-uno/
├── README.md
└── nombre-apellido/          <-- Tu carpeta personal
    ├── index.html            <-- Estructura HTML vinculada al script
    └── app.js                <-- Tu lógica de JavaScript
```

3. Asegúrate de enlazar tu archivo JavaScript en el `index.html` antes de cerrar la etiqueta `</body>`:
   ```html
   <script src="app.js"></script>
   ```

---

### 5. Desarrollar la Solución
- Resuelve el ejercicio asignado según las instrucciones del documento adjunto provisto por el docente.
- Asegúrate de comprobar el correcto funcionamiento abriendo el archivo `index.html` en el navegador y verificando la consola de desarrollador (`F12`).

---

### 6. Guardar y Subir los Cambios
Una vez finalizado y probado tu ejercicio, registra tus cambios y súbelos a tu repositorio:

```bash
# 1. Verifica los archivos modificados
git status

# 2. Agrega los cambios de tu carpeta
git add .

# 3. Realiza el commit con un mensaje descriptivo
git commit -m "feat: solucion evaluacion JavaScript - Nombre Apellido"

# 4. Sube los cambios a la rama develop de tu fork
git push origin develop
```

---

## 📤 Entrega
Para finalizar la entrega:
1. Asegúrate de que los cambios estén visibles en tu repositorio en GitHub dentro de la rama `develop`.
2. *(Opcional / Según indique el docente)* Crea un **Pull Request** desde la rama `develop` de tu fork hacia la rama `develop` del repositorio original, o envía el enlace de tu repositorio/fork por el medio asignado.

---

## 💡 Criterios a tener en cuenta
- **Estructura correcta de Git:** Trabajo realizado exclusivamente en la rama `develop`.
- **Organización de archivos:** Todo tu trabajo debe estar estrictamente dentro de tu carpeta personal sin modificar archivos ajenos.
- **Calidad del código:** Uso de nombres claros para variables y funciones, código ordenado, buenas prácticas y comentarios explicativos cuando sea necesario.
