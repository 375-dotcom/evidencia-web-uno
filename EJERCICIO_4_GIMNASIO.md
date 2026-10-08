# 📌 Planteamiento del Problema: Centro Fitness "FitZone Club"

## Contexto y Planteamiento del Problema
El centro deportivo y gimnasio **"FitZone Club"** requiere un software en JavaScript para el módulo de recepción y ventas. El sistema debe permitir atender a los usuarios, registrar la compra de mensualidades, sesiones de entrenamiento personalizado y suplementos nutricionales, liquidando el total con descuentos y llevando el control financiero diario.

Para evaluar el razonamiento lógico básico, **queda estrictamente prohibido el uso de arreglos (arrays) y objetos**. Todo el sistema debe gestionarse utilizando variables primitivas (`number`, `string`, `boolean`), funciones, condicionales y ciclos anidados.

---

## Requerimientos del Sistema

### 1. Estructura de Menús (3 Ciclos Anidados)
El sistema debe estar estructurado obligatoriamente mediante **tres niveles de ciclos anidados**:

- **Nivel 1 — Menú Principal (Ciclo 1):**  
  Debe repetirse hasta que se cierre la recepción:
  1. Atender socio / nuevo usuario
  2. Ver balance de caja del día
  3. Salir del sistema

- **Nivel 2 — Menú de Servicios y Tienda (Ciclo 2):**  
  Se ejecuta al atender un usuario y se repite hasta que el usuario decida pagar:
  1. Planes de Membresía
  2. Clases y Entrenador Personalizado
  3. Tienda Fitness y Suplementos
  4. Finalizar compra y facturar

- **Nivel 3 — Menú de Opciones y Cantidades (Ciclo 3):**  
  Permite al usuario seleccionar el plan o artículo e indicar la cantidad o meses deseados (debe ser mayor a 0). Se repite hasta que elija volver al menú de servicios:
  - **Planes de Membresía:**
    - 1. Pase Diario / Tiquetera 1 día: $15.000
    - 2. Mensualidad Básica (Área de pesas y cardio): $80.000
    - 3. Mensualidad VIP (Acceso total + Zona húmeda): $120.000
    - 4. Volver al menú de servicios
  - **Clases y Entrenador Personalizado:**
    - 1. Clase de Spinning / Indoor Cycling: $18.000
    - 2. Sesión con Entrenador Personal (1 hora): $35.000
    - 3. Paquete Clase de Funcional / Cross: $20.000
    - 4. Volver al menú de servicios
  - **Tienda Fitness y Suplementos:**
    - 1. Bebida Hidratante / Energizante: $7.000
    - 2. Barra de Proteína: $9.000
    - 3. Termo Deportivo Oficial: $25.000
    - 4. Volver al menú de servicios

---

### 2. Cálculos y Facturación por Usuario
Al seleccionar la opción **Finalizar compra y facturar** en el Menú de Servicios:
1. **Descuento por Medio de Pago o Volumen:**
   - Si el usuario paga en **Efectivo** y el subtotal supera los **$100.000**, recibe un **10% de descuento**.
   - Si el usuario es **Estudiante** (presenta carné válido), recibe un **8% de descuento** sin importar el medio de pago (los descuentos no son acumulables; aplica el mayor).
   - En caso contrario, no aplica descuento.
2. **Seguro Deportivo Contra Lesiones (Opcional):**
   - Preguntar si desea incluir la póliza de cobertura médica deportiva por un valor adicional fijo de **$6.000**.
3. **Total:**
   - $\text{Total a Pagar} = \text{Subtotal} - \text{Descuento} + \text{Seguro}$.
   - Mostrar el resumen al socio: subtotal, descuento aplicado, seguro médico y total final.

---

### 3. Estadísticas de la Jornada
En el Menú Principal, la opción **Ver balance de caja del día** debe mostrar los acumulados globales:
- Total de usuarios o clientes atendidos.
- Total de dinero recaudado en la recepción.
- Total de servicios, meses y productos facturados en total.
- Promedio de compra por usuario ($\text{Total recaudado} / \text{Usuarios atendidos}$).

---

## Restricciones Técnicas
1. **NO usar arreglos (`[]`, `Array`) ni objetos (`{}`, `Object`).**
2. Se debe trabajar únicamente con variables primitivas, contadores y acumuladores.
3. Se deben implementar **funciones** para modularizar el código (por ejemplo: para mostrar menús, calcular descuentos y calcular totales).
4. Usar condicionales (`if/else` o `switch`) para controlar las opciones y validaciones.
