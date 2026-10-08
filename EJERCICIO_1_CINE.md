# 📌 Planteamiento del Problema: Taquilla de Cine "CineStar"

## Contexto y Planteamiento del Problema
La cadena de cines **"CineStar"** necesita un programa en JavaScript para automatizar el punto de venta de taquilla y confitería. El sistema debe permitir atender a múltiples clientes durante el turno, registrar boletos para funciones, snacks y combos especiales, calculando el total a pagar de cada cliente y el balance general de ventas al finalizar la jornada.

Para evaluar el razonamiento lógico básico, **queda estrictamente prohibido el uso de arreglos (arrays) y objetos**. Todo el sistema debe gestionarse utilizando variables primitivas (`number`, `string`, `boolean`), funciones, condicionales y ciclos anidados.

---

## Requerimientos del Sistema

### 1. Estructura de Menús (3 Ciclos Anidados)
El sistema debe estar estructurado obligatoriamente mediante **tres niveles de ciclos anidados**:

- **Nivel 1 — Menú Principal (Ciclo 1):**  
  Debe repetirse hasta que se elija cerrar la taquilla:
  1. Atender cliente
  2. Ver balance de la jornada
  3. Salir del sistema

- **Nivel 2 — Menú de Áreas de Venta (Ciclo 2):**  
  Se ejecuta al atender un cliente y se repite hasta que el cliente finalice su compra:
  1. Entradas de Cine
  2. Confitería y Snacks
  3. Combos Especiales
  4. Finalizar compra y facturar

- **Nivel 3 — Menú de Productos y Cantidades (Ciclo 3):**  
  Permite al cliente agregar uno o varios ítems de la categoría seleccionada indicando la cantidad (debe ser mayor a 0). Se repite hasta que elija volver al menú de áreas:
  - **Entradas de Cine:**
    - 1. Entrada General 2D: $12.000
    - 2. Entrada Sala 3D: $16.000
    - 3. Entrada VIP / IMAX: $22.000
    - 4. Volver al menú de áreas
  - **Confitería y Snacks:**
    - 1. Crispetas / Palomitas Grandes: $10.000
    - 2. Gaseosa Grande: $6.000
    - 3. Perro Caliente / Hot Dog: $8.500
    - 4. Volver al menú de áreas
  - **Combos Especiales:**
    - 1. Combo Personal (Crispeta Mediana + Gaseosa): $13.500
    - 2. Combo Pareja (Crispeta Grande + 2 Gaseosas + Dulce): $24.000
    - 3. Combo Familiar (2 Crispetas Grandes + 3 Gaseosas + 2 Perros): $38.000
    - 4. Volver al menú de áreas

---

### 2. Cálculos y Facturación por Cliente
Al seleccionar la opción **Finalizar compra y facturar** en el Menú de Áreas:
1. **Descuento por Membresía / Medio de pago:**
   - Preguntar si el cliente tiene **Tarjeta CineStar Club**:
     - Si tiene tarjeta: aplica un **15% de descuento** sobre el subtotal.
     - Si no tiene tarjeta, pero paga en **Efectivo** y su subtotal supera los **$30.000**: aplica un **5% de descuento**.
     - En cualquier otro caso: no aplica descuento.
2. **Recargo por Donación Cultural Voluntaria:**
   - Preguntar si desea donar **$2.000** para el fondo de fomento cinematográfico nacional.
3. **Total:**
   - $\text{Total a Pagar} = \text{Subtotal} - \text{Descuento} + \text{Donación}$.
   - Mostrar el resumen al cliente: subtotal, descuento aplicado, donación y total a pagar.

---

### 3. Estadísticas de la Jornada
En el Menú Principal, la opción **Ver balance de la jornada** debe mostrar los acumulados globales:
- Total de clientes atendidos en el turno.
- Total de dinero recaudado en taquilla.
- Total de entradas y productos vendidos en total.
- Promedio de gasto por cliente ($\text{Total recaudado} / \text{Clientes atendidos}$).

---

## Restricciones Técnicas
1. **NO usar arreglos (`[]`, `Array`) ni objetos (`{}`, `Object`).**
2. Se debe trabajar únicamente con variables primitivas, contadores y acumuladores.
3. Se deben implementar **funciones** para modularizar el código (por ejemplo: para mostrar menús, calcular descuentos y calcular totales).
4. Usar condicionales (`if/else` o `switch`) para controlar las opciones y validaciones.
