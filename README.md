# 📝 Evaluación Práctica: JavaScript — Web 1

¡Bienvenidos a la evaluación práctica del curso **Web 1**!  
En esta actividad pondrás a prueba tus conocimientos fundamentales de **JavaScript** y el manejo del flujo de trabajo con **Git y GitHub**.

---

## 🎯 Objetivo
Desarrollar la solución al ejercicio asignado en JavaScript, integrándolo en una estructura web básica y gestionando las versiones del código mediante buenas prácticas con Git.

> [!NOTE]
> Cada estudiante tiene un ejercicio específico asignado según su documento de identidad. Consulta la sección [📚 Asignación de Ejercicios](#-asignación-de-ejercicios) en este documento.

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

1. Crea una carpeta nombrada con tu **documento + guion + nombre y apellido** (en minúsculas y separado por guion, por ejemplo: `1014293362-jaime-zapata`).
2. Entra a tu carpeta y crea los siguientes dos archivos:
   - `index.html`: Estructura base HTML5 donde se visualizará o interactuará con el ejercicio.
   - `app.js` (o `index.js`): Código JavaScript donde implementarás la solución al ejercicio.

#### Estructura de carpetas esperada:
```text
evidencia-web-uno/
├── README.md
└── documento-nombre-apellido/          <-- Tu carpeta personal
    ├── index.html            <-- Estructura HTML vinculada al script
    └── app.js                <-- Tu lógica de JavaScript
```

3. Asegúrate de enlazar tu archivo JavaScript en el `index.html` antes de cerrar la etiqueta `</body>`:
   ```html
   <script src="app.js"></script>
   ```

---

### 5. Desarrollar la Solución
- Busca tu número de documento de identidad en la **Tabla de Asignación de Ejercicios** ubicada a continuación.
- Abre y lee detenidamente el archivo `.md` del ejercicio que te fue asignado.
- Resuelve el ejercicio en tu archivo `app.js` cumpliendo con todos los requerimientos y restricciones técnicas indicadas en su respectivo enunciado.
- Comprueba el correcto funcionamiento abriendo tu archivo `index.html` en el navegador y verificando la consola de desarrollador (`F12`).

---

## 📚 Asignación de Ejercicios

### 🔗 Enunciados Disponibles
- **Ejercicio 1:** [EJERCICIO_1_CINE.md](EJERCICIO_1_CINE.md) — *Taquilla de Cine "CineStar"*
- **Ejercicio 2:** [EJERCICIO_2_PARQUE.md](EJERCICIO_2_PARQUE.md) — *Parque de Diversiones "Aventura Park"*
- **Ejercicio 3:** [EJERCICIO_3_MASCOTAS.md](EJERCICIO_3_MASCOTAS.md) — *Tienda de Mascotas "Pet Center"*
- **Ejercicio 4:** [EJERCICIO_4_GIMNASIO.md](EJERCICIO_4_GIMNASIO.md) — *Centro Fitness "FitZone Club"*

---

### 📋 Tabla de Asignación por Documento

| Documento | Ejercicio Asignado | Enunciado |
| :---: | :---: | :--- |
| **1036449813** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **1037596269** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |
| **1035866185** | 3 | [Ver Ejercicio 3](EJERCICIO_3_MASCOTAS.md) |
| **1035857735** | 4 | [Ver Ejercicio 4](EJERCICIO_4_GIMNASIO.md) |
| **1021804625** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **1037607011** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |
| **1001588913** | 3 | [Ver Ejercicio 3](EJERCICIO_3_MASCOTAS.md) |
| **1007239276** | 4 | [Ver Ejercicio 4](EJERCICIO_4_GIMNASIO.md) |
| **1214743083** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **4903282** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |
| **1095801952** | 3 | [Ver Ejercicio 3](EJERCICIO_3_MASCOTAS.md) |
| **1000442275** | 4 | [Ver Ejercicio 4](EJERCICIO_4_GIMNASIO.md) |
| **1026141847** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **1020436045** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |
| **1001014162** | 3 | [Ver Ejercicio 3](EJERCICIO_3_MASCOTAS.md) |
| **1020419234** | 4 | [Ver Ejercicio 4](EJERCICIO_4_GIMNASIO.md) |
| **1007238587** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **1001011043** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |
| **1000570133** | 3 | [Ver Ejercicio 3](EJERCICIO_3_MASCOTAS.md) |
| **1036956502** | 4 | [Ver Ejercicio 4](EJERCICIO_4_GIMNASIO.md) |
| **1017192554** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **1019054366** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |
| **91506744** | 3 | [Ver Ejercicio 3](EJERCICIO_3_MASCOTAS.md) |
| **1036674924** | 4 | [Ver Ejercicio 4](EJERCICIO_4_GIMNASIO.md) |
| **1003082810** | 1 | [Ver Ejercicio 1](EJERCICIO_1_CINE.md) |
| **1013344035** | 2 | [Ver Ejercicio 2](EJERCICIO_2_PARQUE.md) |

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
