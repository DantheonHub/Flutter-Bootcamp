# Bitácora de clases — Bootcamp de Desarrollo de Apps Móviles con Flutter

Una línea por clase real, en el orden en que se dictaron. El detalle técnico de cada tema vive en `conceptos.md`.

## Módulo 1: Introducción

* **Clase 1 — Inauguración: fundamentos de desarrollo móvil**
  - **Contenido:** clase teórica introductoria sobre los fundamentos del desarrollo de apps móviles.

  → Detalle completo en [`fundamentos/conceptos.md`](./fundamentos/conceptos.md)

* **Clase 2 — Instalación de herramientas de desarrollo**
  - **Contenido:** instalación y configuración del entorno de trabajo (Flutter SDK, Android Studio y plugins). Sin contenido conceptual nuevo.

## Módulo 2: Introducción a Dart

* **Clase 3 — Repaso de Dart y ejercicios prácticos**
  - **Contenido:** repaso general de los conceptos básicos de Dart y práctica guiada resolviendo ejercicios en una plataforma en vivo.

  → Detalle completo en [`Curso-de-Dart/conceptos-dart.md`](https://github.com/DantheonHub/Curso-de-Dart/blob/main/conceptos-dart.md)

  - **Actividades asignadas:** continuar resolviendo por cuenta propia los ejercicios de repaso pendientes (carpeta de "primeros pasos" del curso).

  > Recordatorio de instalar los plugins de Dart y Flutter en Android Studio para quien no lo haya hecho en la Clase 2.

* **Clase 4 — Programación asíncrona con Dart**
  - **Contenido:** repaso breve de POO y programación asíncrona en Dart (`Future`, `async`/`await`, `Stream`, concurrencia vs. paralelismo, isolates). Contenido de Dart puro — el detalle completo está en [`Curso-de-Dart/conceptos-dart.md`](https://github.com/DantheonHub/Curso-de-Dart/blob/main/conceptos-dart.md), sección "Programación asíncrona".
  - **Actividades asignadas:** practicar simulando la descarga de datos con un `Future`, generando un `Stream` propio y filtrándolo con `where`.

## Módulo 3: Introducción a Flutter

* **Clase 5 — Introducción a Flutter (Parte 1)**
  - **Contenido:** primeros pasos con Flutter — qué es un widget, jerarquía y árbol de widgets, `BuildContext`, `Key`, diferencia entre `StatelessWidget` y `StatefulWidget`, `Scaffold`/`AppBar`, widgets Material y Cupertino, widgets básicos de texto e íconos.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

* **Clase 6 — Introducción a Flutter (Parte 2)**
  - **Contenido:** widgets `Card` y `Container` en profundidad (decoración, bordes, degradados, imagen de fondo), interactividad (`InkWell`/`GestureDetector`), `ListTile`, menús de navegación (`Drawer` y `BottomNavigationBar`) y ventanas flotantes (`AlertDialog` y `showModalBottomSheet`).

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** recrear un diseño de tarjeta (`Card`) tipo "credit card" y un `Container` tipo "plan" con degradado, borde, sombra, `Divider` y `ListTile` — enunciados en las diapositivas de la clase.