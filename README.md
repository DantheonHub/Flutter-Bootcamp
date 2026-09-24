# Bootcamp de Desarrollo de Apps Móviles con Flutter

Este repositorio contiene mis apuntes y prácticas del **Bootcamp de Desarrollo de Apps Móviles con Flutter**, dictado en **vivo** por **Código Facilito**.

El contenido está organizado como una **biblioteca de conceptos**: un archivo `conceptos.md` por tema/tecnología, que funciona como fuente de verdad y guía de consulta permanente, independiente del orden cronológico en que se fue viendo en las clases en vivo.

## Contenido cubierto hasta el momento

- **Fundamentos de desarrollo móvil** *(contenido teórico, sin código aún)*: arquitectura de Android e iOS, niveles de API y fragmentación, privacidad, tamaño/resolución/densidad de pantalla, unidades `dp`/`sp`/`pt`, evolución del diseño de interfaces (skeuomorfismo, flat design, glassmorfismo), SDKs y frameworks nativos, tipos de almacenamiento, tipos de desarrollo de apps (nativo, híbrido, multiplataforma).
- **Módulo 2 — Dart**: cubierto a través del [**Curso profesional de Dart**](https://github.com/DantheonHub/Curso-de-Dart), tomado como material complementario del bootcamp. Ese repositorio funciona como la biblioteca de conceptos de Dart para todo el bootcamp — acá solo se registra en la bitácora qué se vio en cada clase en vivo relacionada.
- **Módulo 3 — Flutter**: widgets fundamentales (`Card`, `Container`, `ListTile`, menús, ventanas flotantes), árbol de widgets, `StatelessWidget`/`StatefulWidget` y manejo básico de estado.
- **Módulo 4 — Listas y formularios** *(en curso)*: `TextFormField` y validaciones, `Form`, selección (`Radio`/`Checkbox`/`Switch`, `Dropdown`), `ListView`, `GridView`, listas anidadas, CRUD en memoria con `setState`, y temas globales (colores por rol con `ColorScheme`, modo claro/oscuro, tipografía y temas de componentes).

*(Esta sección se irá ampliando a medida que avancen los módulos de Flutter, arquitectura y manejo de estado, persistencia con SQLite y consumo de APIs.)*

## Estructura del repositorio

```
📁 fundamentos/
   📄 conceptos.md
📁 flutter/
   📄 conceptos.md
📄 bitacora.md
📄 README.md
```

- Cada carpeta corresponde a un área temática del bootcamp (no a un módulo puntual del calendario), y contiene su propio `conceptos.md` con índice interno.
- Al final de cada archivo se agregan los **ejemplos prácticos**: el código de cada práctica aprobada junto con los conceptos nuevos que aplica.
- `bitacora.md` resume, clase por clase y sin entrar en detalle técnico, qué se vio en cada una — el detalle completo está en el `conceptos.md` de cada tema (o, en el caso de Dart, en el repo [`Curso-de-Dart`](https://github.com/DantheonHub/Curso-de-Dart)).
- A medida que avance el bootcamp se irán sumando nuevas carpetas (Flutter, arquitectura y estado, datos y APIs, proyecto final), siguiendo siempre esta misma convención: `carpeta-tema/conceptos.md`.

## Sobre el bootcamp

El bootcamp cubre el desarrollo de apps móviles con Flutter de punta a punta: fundamentos de desarrollo móvil, el lenguaje Dart, Flutter (widgets, diseño, navegación), patrones arquitectónicos y manejo de estado, persistencia de datos con SQLite, consumo de servicios web, y publicación de la app en Google Play Store.

---

**Autor:** Dante Chara — [@DantheonHub](https://github.com/DantheonHub)