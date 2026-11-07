# SeguroFlash — Laboratorio de probabilidad

Abrí `index.html` directamente en el navegador. Funciona sin Internet, servidor, Node.js ni dependencias. HTML, CSS y JavaScript están incluidos en el mismo archivo.

## Variables editables

- Población observada y personas con al menos un incidente.
- Período observado y horizonte futuro, en meses.
- Probabilidad derivada de los conteos o introducida manualmente.
- Población futura.
- Costo medio total por persona afectada en el horizonte futuro.
- Gastos fijos mensuales, recargo sobre costos y cuota mensual.
- Moneda de presentación (no convierte importes).

## Resultados

Probabilidad proyectada, personas esperadas con y sin incidentes, desviación estándar binomial, intervalo de Wilson del 95 % para la tasa empírica, costos e ingresos esperados, balance, cuota de equilibrio y cuota con recargo. Cada cálculo incluye fórmulas y supuestos.

Guardá hasta 20 escenarios y volvé a cargarlos para comparar. Se conservan en localStorage si el navegador lo permite; en caso contrario quedan durante la sesión. Exportá el escenario actual y los guardados como JSON. La app no importa JSON.

## Límites del modelo

Convertir períodos requiere riesgo constante; el modelo binomial supone personas independientes con la misma probabilidad. Se cuentan personas afectadas, no incidentes repetidos. Los costos iniciales son ejemplos editables, no datos de la práctica. El recargo sobre costos no es un margen sobre ingresos ni una garantía de solvencia. La incertidumbre de los costos no se modela.

## Verificación

Se verificaron sintaxis JavaScript y cálculos de frecuencia, conversión temporal, costos, recargo, intervalos y tasas de 0 % y 100 %. Falta verificación visual en navegador.

## Demostración de conceptos y guion

El panel «Incidentes y condiciones de lluvia» usa una tabla independiente de cuatro conteos editables. Muestra inclusión-exclusión, probabilidad condicional, multiplicación, Bayes y comparación de independencia empírica. Incluye «Ver teoría» y validación de denominadores nulos. Estos datos son ilustrativos y no se sincronizan con la calculadora superior.

`Guion_exposicion_SeguroFlash.docx` vincula cada intervención con los campos y resultados visibles de la aplicación y con los nueve criterios de la rúbrica. La indagación real en DiálogoX y la publicación de un enlace funcional siguen siendo parte de la entrega del estudiante.

## Casos de DiálogoX

Se añadieron cuatro módulos independientes con navegación directa: coberturas mediante inclusión-exclusión, choque condicionado a viajes nocturnos bajo lluvia, producto de carretera rápida y accidente grave, y Bayes para un sensor con sensibilidad y falsos positivos. Todos permiten editar los parámetros, incluyen «Ver teoría» y validan casos imposibles o condicionantes con probabilidad cero.

El guion actualizado contiene los mismos valores de estos módulos y variaciones para la exposición. La tabla del sensor representa conteos esperados; no registros medidos. Sensibilidad y valor predictivo positivo se muestran como conceptos distintos.
# proba-y-estadistica-practica-2
