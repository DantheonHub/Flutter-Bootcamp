# Bitácora de clases — Bootcamp de Desarrollo de Apps Móviles con Flutter

Una línea por clase real, en el orden en que se dictaron. El detalle técnico de cada tema vive en `conceptos.md`.

## Módulo 1: Introducción

* **Clase 1 — Inauguración: fundamentos de desarrollo móvil**
  - **Contenido:** fundamentos de desarrollo móvil.

  → Detalle completo en [`fundamentos/conceptos.md`](./fundamentos/conceptos.md)

* **Clase 2 — Instalación de herramientas de desarrollo**
  - **Contenido:** instalación de Flutter SDK, Android Studio y plugins. Sin contenido conceptual nuevo.

## Módulo 2: Introducción a Dart

* **Clase 3 — Repaso de Dart y ejercicios prácticos**
  - **Contenido:** repaso de Dart y ejercicios en una plataforma en vivo.

  → Detalle completo en [`Curso-de-Dart/conceptos-dart.md`](https://github.com/DantheonHub/Curso-de-Dart/blob/main/conceptos-dart.md)

  - **Actividades asignadas:** ejercicios de repaso pendientes (carpeta "primeros pasos" del curso).

  > Instalar los plugins de Dart y Flutter en Android Studio para quien no lo haya hecho en la Clase 2.

* **Clase 4 — Programación asíncrona con Dart**
  - **Contenido:** POO (repaso) y programación asíncrona (`Future`, `async`/`await`, `Stream`, concurrencia vs. paralelismo, isolates).

  → Detalle completo en [`Curso-de-Dart/conceptos-dart.md`](https://github.com/DantheonHub/Curso-de-Dart/blob/main/conceptos-dart.md), sección "Programación asíncrona"

  - **Actividades asignadas:** simular una descarga con `Future`, generar un `Stream` propio y filtrarlo con `where`.

## Módulo 3: Introducción a Flutter

* **Clase 5 — Introducción a Flutter (Parte 1)**
  - **Contenido:** widgets, árbol de widgets, `BuildContext`, `Key`, `StatelessWidget` vs. `StatefulWidget`, `Scaffold`/`AppBar`, Material vs. Cupertino, texto e íconos.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

* **Clase 6 — Introducción a Flutter (Parte 2)**
  - **Contenido:** `Card` y `Container` (decoración, bordes, degradados, imagen de fondo), `InkWell`/`GestureDetector`, `ListTile`, `Drawer`, `BottomNavigationBar`, `AlertDialog`, `showModalBottomSheet`.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** recrear un `Card` tipo "credit card" y un `Container` tipo "plan" (degradado, borde, sombra, `Divider`, `ListTile`) — diapositivas de la clase.

  > Mencionado en clase, para más adelante (al ver MVVM/Clean Architecture): separar en carpetas distintas los widgets reutilizables de las pages.

## Módulo 4: Listas y formularios

* **Clase 7 — Widgets mutables: crear un formulario y validar**
  - **Contenido:** `TextEditingController` y atributos de `TextFormField` (`decoration`, `keyboardType`, `textInputAction`/`onFieldSubmitted`, `obscureText`, `enabled`, `maxLength`, `maxLines`, `onChanged`); `inputFormatters` (forzar mayúsculas, permitir/denegar caracteres con expresiones regulares); `Form` + `GlobalKey<FormState>` + `validate()`; `validator` por campo, incluida comparación entre dos campos (contraseña/repetir contraseña); `onSaved`; selección con `RadioListTile`, `CheckboxListTile` y `SwitchListTile`; `DropdownButtonFormField`. Quiz en vivo sobre los atributos de `TextFormField` (quedaron marcados como tema de examen en `conceptos.md`). Se mencionaron `Stepper` y `AutofillGroup` sin desarrollarlos en profundidad por tiempo — código para revisar por cuenta propia. Arranca Módulo 4 — queda pendiente su segunda clase.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** revisar por cuenta propia el código completo compartido por la cátedra (formulario con todos los atributos comentados, y los widgets de `Stepper`/`AutofillGroup`).

  > Se recomienda repasar la grabación de la clase antes del examen, especialmente la parte de validaciones. Dudas puntuales, por el canal de Telegram del bootcamp.

* **Clase 8 — Trabajando con arreglos y componentes de listas**
  - **Contenido:** `ListView` estático, `ListView.builder` (`itemCount`/`itemBuilder`) y `ListView.separated` (`separatorBuilder`); atributos `padding`, `itemExtent`, `reverse`, `physics` (`BouncingScrollPhysics`, `ClampingScrollPhysics`, `NeverScrollableScrollPhysics`, `AlwaysScrollableScrollPhysics`) y `shrinkWrap`; lista horizontal con `scrollDirection`; listas dentro de listas (`shrinkWrap` + `NeverScrollableScrollPhysics`); `GridView.count` y `GridView.builder` (`SliverGridDelegateWithFixedCrossAxisCount`, `crossAxisSpacing`/`mainAxisSpacing`); modelo `User` con `copyWith`, lista de objetos y CRUD en memoria (`add`, `remove`, `indexWhere`, `setState`), con un único método `saveUser` para crear/editar y formulario reutilizable en un `AlertDialog` (`null` = crear); manejo de nulos (`?`, `!`, `late`) y convención `snake_case` para archivos. Quiz en vivo sobre los atributos de `ListView` (quedaron marcados como tema de examen en `conceptos.md`). El CRUD (guardar, editar, eliminar) se retoma más adelante con base de datos y consumo de servicios web.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** replicar un diseño con una lista padre que contiene un `GridView` de 4 columnas, una lista horizontal y una lista vertical; y un `ListView.builder` simple. Código del CRUD compartido por la cátedra para practicar.

  > El quiz se puede repetir las veces que se quiera. Diapositivas, quiz y código de la clase en el repo de la profesora ([`Marines0210/bootcamp_flutter`](https://github.com/Marines0210/bootcamp_flutter)).
  >
  > Mencionado en clase, para más adelante: CRUD genérico con abstracción y polimorfismo (al ver patrones arquitectónicos) y cantidad de columnas del `GridView` según dispositivo (al ver app responsiva).

* **Clase 9 — Manejo de temas, colores y estilos**
  - **Contenido:** colores con `Colors` (tonos 50 a 900), hexadecimal (prefijo `0xFF`) y RGB (`Color.fromARGB`); centralización de colores y por qué usar roles semánticos en vez de nombres de color; `ColorScheme` (`primary`, `secondary`, `tertiary`, `surface`, `error` y sus pares `on…`; `background` reemplazado por `surface`), `ColorScheme.light`/`dark` y `ColorScheme.fromSeed`; generadores de paleta (Material Theme Builder y Material 3 Color Generator); `ThemeData` en una clase `AppTema` (carpeta `tema/`), con `theme`/`darkTheme`/`themeMode` en `MaterialApp` y botón en el `AppBar` para alternar claro/oscuro con `setState`; restricción de acceso a la paleta con `_`, `part` y `part of`; consulta de colores con `Theme.of(context)`; tipografía de Material 3 (`display`, `headline`, `title`, `body`, `label`), `textTheme` con `google_fonts`, `copyWith` y `apply`; temas de componentes (`elevatedButtonTheme`, `cardTheme`, `appBarTheme`). Quiz en vivo de 10 preguntas sobre los atributos vistos (quedaron marcados como tema de examen en `conceptos.md`).

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** hacer el quiz de la clase (se puede repetir las veces que se quiera) y practicar generando una paleta propia con alguno de los dos generadores, o usando la paleta de ejemplo de la clase, para aplicarla en el proyecto.

  > Diapositivas, PDF con los colores de ejemplo y código de la clase en el repo de la profesora ([`Marines0210/bootcamp_flutter`](https://github.com/Marines0210/bootcamp_flutter)). Dudas y resultados del quiz, por el canal de Telegram del bootcamp.

* **Clase 10 — Responsividad móvil y web, y app multidioma**
  - **Contenido:** widgets de distribución flexible (`Expanded`, `Flexible` con `flex`/`fit`, `Wrap`, `FractionallySizedBox`, `AspectRatio`, `FittedBox`) y el error `RenderFlex overflowed`; medición con `MediaQuery` (tamaño y orientación) y `LayoutBuilder` (restricciones del padre); puntos de quiebre (móvil/tablet/escritorio/web) definidos como constantes y una clase `Responsive`; patrones adaptativos (Master-Detail, Reflow, Shift Data, Disconnect, Expand/Stretch); paquete `flutter_screenutil_plus` (`ScreenUtilPlusInit`, `designSize`, extensiones `.w`/`.h`/`.r`/`.sp`, `ResponsiveBuilder` con breakpoints `xs`/`sm`/`md`/`lg`/`xl`) como alternativa empaquetada a la implementación manual. Quiz en vivo sobre la característica principal de cada widget de distribución flexible (quedó marcado como tema de examen en `conceptos.md`). No se llegó al tema de apps multidioma anunciado en el título de la clase.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** actividad de Master-Detail escalable con `flutter_screenutil_plus` (mostrar una lista si es móvil o tablet, y un master-detail si es escritorio o web; usar `.sp` para los textos y `.w`/`.h` para los contenedores) — resuelta por cuenta propia, sin subir al repo.

  > Diapositivas y código de la clase en el repo de la profesora ([`Marines0210/bootcamp_flutter`](https://github.com/Marines0210/bootcamp_flutter)). Sin clase la semana siguiente; próxima clase el martes 22.