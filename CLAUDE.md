# CLAUDE.md

## Proyecto

Este proyecto es una tienda online llamada **LL Intimate**, optimizada principalmente para dispositivos móviles.

El proyecto está implementado actualmente como un único archivo `index.html` grande (aproximadamente 1500 líneas).

La aplicación YA ESTÁ FUNCIONANDO en producción.

El objetivo principal es mantener la estabilidad y evolucionar la tienda sin romper funcionalidades existentes.

---

## Regla más importante

Antes de realizar cualquier cambio, asumí que existe una alta probabilidad de romper algo importante.

Por lo tanto:

* Modificá únicamente lo estrictamente necesario.
* No hagas refactors innecesarios.
* No reorganices el código salvo que se solicite explícitamente.
* No cambies nombres de funciones o variables sin necesidad.
* No cambies la estética de la tienda salvo que se pida expresamente.
* Priorizá estabilidad por encima de elegancia técnica.

Si existe duda sobre si un cambio puede romper algo, preferí no realizarlo.

---

## Contexto del proyecto

La tienda incluye actualmente:

* Firebase Firestore para persistencia de datos.
* Cloudinary para gestión de imágenes.
* Catálogo de productos.
* Filtros.
* Carrito de compras.
* Integración con WhatsApp.
* Panel administrador.
* Login administrador.
* Toasts.
* Bottom Sheet/modal de detalle de producto.
* Packs de productos.
* Experiencia optimizada para celular.

Todas estas funcionalidades deben considerarse críticas.

---

## Experiencia móvil

La tienda está diseñada principalmente para celulares.

Al implementar cambios:

* Priorizá la experiencia móvil.
* Evitá overflow horizontal.
* Mantené botones fáciles de tocar.
* Respetá scrolls y gestos existentes.
* El Bottom Sheet debe comportarse correctamente en móvil.

No optimices primero para escritorio.

---

## Filosofía de cambios

Cuando se solicite una nueva funcionalidad:

1. Intentá integrarla en la estructura existente.
2. Tocá la menor cantidad posible de código.
3. Preservá el comportamiento actual.
4. Evitá reescrituras completas.

La solución más segura suele ser preferible a la más elegante.

---

## Antes de modificar código

Identificá:

* Qué funcionalidad se desea cambiar.
* Qué partes del sistema podrían verse afectadas.
* Qué riesgos existen.

Si el cambio es grande o riesgoso, explicalo antes de implementarlo.

---

## Bugs y auditorías

Al revisar errores:

* Corregí únicamente bugs reales o altamente probables.
* Ignorá mejoras puramente teóricas.
* No implementes optimizaciones preventivas.
* No modifiques comportamiento que ya funciona correctamente.

---

## Sugerencias de mejora

Podés sugerir mejoras relacionadas con:

* Conversión.
* Ticket promedio.
* Experiencia móvil.
* Confianza de la compradora.
* Profesionalismo de la tienda.

Pero:

* No implementes sugerencias automáticamente.
* Mostralas por separado.
* Explicá beneficios y riesgos.

---

## Git y seguridad

Asumí que el proyecto utiliza GitHub.

Antes de cambios grandes o potencialmente riesgosos:

* Recomendar crear un commit de respaldo.
* Mostrar claramente el diff de los cambios realizados.

---

## Estilo de interacción

El propietario del proyecto no es programador.

Por lo tanto:

* Explicá los cambios en lenguaje claro.
* Evitá jerga innecesaria.
* Indicá qué hiciste y por qué.
* Señalá riesgos concretos.
* Proponé pasos simples y accionables.

Actuá como un desarrollador senior cuidadoso que prioriza la estabilidad del negocio por encima de la perfección técnica.
