# 📌 Planteamiento del Problema: Parque de Diversiones "Aventura Park"

## Contexto y Planteamiento del Problema
El parque temático **"Aventura Park"** requiere un sistema de taquilla en JavaScript para gestionar la venta de pasaportes, atracciones individuales y experiencias interactivas a los visitantes durante el día.

El sistema debe registrar las compras de cada visitante de manera secuencial, permitiéndole armar su paquete según las zonas del parque y la cantidad de pases que requiera. Al finalizar el día, la administración necesita conocer el balance financiero y el flujo total de visitantes.

Para evaluar el razonamiento lógico básico, **queda estrictamente prohibido el uso de arreglos (arrays) y objetos**. Todo el sistema debe gestionarse utilizando variables primitivas (`number`, `string`, `boolean`), funciones, condicionales y ciclos anidados.

---

## Requerimientos del Sistema

### 1. Estructura de Menús (3 Ciclos Anidados)
El sistema debe estar estructurado obligatoriamente mediante **tres niveles de ciclos anidados**:

- **Nivel 1 — Menú Principal (Ciclo 1):**  
  Debe repetirse hasta que se cierre la taquilla del parque:
  1. Registrar visitante / grupo
  2. Ver balance del día
  3. Salir del sistema

- **Nivel 2 — Menú de Zonas del Parque (Ciclo 2):**  
  Se ejecuta al atender un visitante y se repite hasta que decida pagar su entrada:
  1. Zona Extrema (Montañas Rusas)
  2. Zona Familiar e Infantil
  3. Zona Acuática
  4. Finalizar compra y facturar

- **Nivel 3 — Menú de Pases y Atracciones (Ciclo 3):**  
  Permite al visitante seleccionar la atracción o pase deseado e indicar el número de pases/entradas (debe ser mayor a 0). Se repite hasta que elija volver al menú de zonas:
  - **Zona Extrema:**
    - 1. Pase Vértigo (Montaña Rusa Principal): $20.000
    - 2. Caída Libre 60m: $18.000
    - 3. Simulador 4D Extremo: $15.000
    - 4. Volver al menú de zonas
  - **Zona Familiar e Infantil:**
    - 1. Carrusel Clásico: $8.000
    - 2. Carros Chocones: $10.000
    - 3. Rueda de la Fortuna Panorámica: $12.000
    - 4. Volver al menú de zonas
  - **Zona Acuática:**
    - 1. Piscina de Olas: $14.000
    - 2. Tobogán Tornado: $16.000
    - 3. Pase Río Lento: $9.000
    - 4. Volver al menú de zonas

---

### 2. Cálculos y Facturación por Visitante
Al seleccionar la opción **Finalizar compra y facturar** en el Menú de Zonas:
1. **Descuento por Volumen o Grupo:**
   - Si el visitante compra un total acumulado de **5 o más pases** y el subtotal es mayor a **$50.000**, se aplica un **12% de descuento**.
   - En caso contrario, si paga en **Efectivo**, recibe un **5% de descuento** sobre el subtotal.
2. **Seguro Médico de Accidentes (Opcional):**
   - Preguntar si desea agregar el seguro médico por un valor fijo adicional de **$5.000** por visitante.
3. **Total:**
   - $\text{Total a Pagar} = \text{Subtotal} - \text{Descuento} + \text{Seguro}$.
   - Mostrar el resumen al visitante: subtotal, descuento, seguro médico y total a pagar.

---

### 3. Estadísticas de la Jornada
En el Menú Principal, la opción **Ver balance del día** debe mostrar los acumulados globales:
- Total de visitantes/grupos registrados.
- Total de dinero recaudado en la taquilla.
- Total de pases vendidos en todo el parque.
- Promedio de compra por visitante ($\text{Total recaudado} / \text{Visitantes registrados}$).

---

## Restricciones Técnicas
1. **NO usar arreglos (`[]`, `Array`) ni objetos (`{}`, `Object`).**
2. Se debe trabajar únicamente con variables primitivas, contadores y acumuladores.
3. Se deben implementar **funciones** para modularizar el código (por ejemplo: para mostrar menús, calcular descuentos y calcular totales).
4. Usar condicionales (`if/else` o `switch`) para controlar las opciones y validaciones.
