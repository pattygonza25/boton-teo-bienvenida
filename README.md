# Bot-On TEO · Landing Bienvenida Beta

Landing page de bienvenida para usuarios beta de Bot-On TEO. Presenta el producto, agradece a los primeros usuarios y recopila feedback a través de un formulario integrado.

---

## Sobre esta página

Esta página fue creada para los usuarios beta de Bot-On TEO, el producto de entrenamiento cognitivo de Bot-On que opera 100% por WhatsApp.

La página cumple tres funciones principales: presenta TEO a usuarios que aún no lo conocen, les agradece por ser parte del programa beta y recopila su experiencia a través de un formulario de Tally integrado directamente en la página. Todo el contenido está optimizado para mobile-first, dado que el perfil del usuario beta llega principalmente desde dispositivos móviles.

---

## Personalización por nombre

La página soporta personalización del nombre del usuario a través de un parámetro en la URL. Esto permite generar links únicos para cada beta tester sin necesidad de infraestructura adicional.

**URL sin nombre:**
```
https://pattygonza25.github.io/boton-teo-bienvenida
```
Muestra: `Hola. Conoce a TEO.`

**URL con nombre:**
```
https://pattygonza25.github.io/boton-teo-bienvenida?nombre=Carolina
```
Muestra: `Hola Carolina. Conoce a TEO.`

Cuando se incluye el parámetro `nombre`, la página lo lee desde la URL con JavaScript vanilla y lo inyecta en el headline principal, generando una experiencia personalizada sin necesidad de backend ni base de datos.

---

## Estructura de la página

1. **Header fijo** con logo Bot-On
2. **Bienvenida** con headline dinámico personalizado por nombre
3. **Qué hace TEO**, tres tarjetas con los beneficios principales
4. **Por qué estás aquí**, llamado al feedback
5. **Formulario de feedback** integrado con Tally
6. **Cierre**
7. **Footer** con disclaimer

---

## Tecnologías

- HTML5, CSS3 y JavaScript vanilla
- Sin frameworks ni dependencias externas
- [Google Fonts, Ubuntu](https://fonts.google.com/specimen/Ubuntu) para la tipografía
- [Tally](https://tally.so) para el formulario de feedback embebido
- [GitHub Pages](https://pages.github.com) para el hosting

---

## Brand System

| Color | Hex | Uso |
|---|---|---|
| Azul claro | `#6AB7EA` | Fondos dominantes |
| Azul primario | `#008bdb` | Botones y acentos |
| Navy | `#1a1f5e` | Header y footer |
| Navy profundo | `#12174a` | Footer |
| Blanco | `#ffffff` | Fondos |
| Gris claro | `#f0f4f8` | Fondos de secciones |

Tipografía: **Ubuntu** (pesos 300, 400, 500, 700). Botones con `border-radius: 100px`.

---

## Cómo generar links para usuarios beta

Para distribuir links personalizados a cada usuario beta se puede usar una hoja de cálculo de Google Sheets o Excel. En la columna A se listan los nombres y en la columna B se aplica la siguiente fórmula:

```
="https://pattygonza25.github.io/boton-teo-bienvenida?nombre="&A2
```

Donde `A2` contiene el nombre del usuario. Esto genera un link único por persona que puede enviarse directamente por WhatsApp, email o cualquier canal de comunicación.

---

## Deployment

La página está desplegada en GitHub Pages y se actualiza automáticamente con cada push a la rama `main`. No requiere proceso de build.

**URL de producción:**
```
https://pattygonza25.github.io/boton-teo-bienvenida
```

---

## Parte del ecosistema Bot-On

Esta landing es parte del ecosistema de productos de Bot-On, empresa de inteligencia artificial aplicada al bienestar cognitivo.

| Producto | Perfil | Canal |
|---|---|---|
| **Bot-On NORA** | Adultos mayores | WhatsApp |
| **Bot-On TEO** | Profesionales y adultos activos | WhatsApp |

Ambos productos operan 100% por WhatsApp, sin necesidad de descargar aplicaciones ni crear cuentas adicionales.

---

© 2026 Bot-On. Confidencial.
