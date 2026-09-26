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

* **Clase 11 — Lineamientos de proyecto final**
  - **Contenido:** clase sin material técnico nuevo; requisitos y entregables del proyecto final del bootcamp (fecha de entrega, criterios de evaluación y opciones sugeridas), a mitad de la cursada. Se evalúan cinco puntos:
    1. **Idea:** una app que resuelva una necesidad específica; no hace falta que sea grande (alcanza, por ejemplo, con una app de notas). Puede usarse IA para generar código, pero hay que poder explicarlo o modificarlo directamente.
    2. **Patrón arquitectónico y patrón de diseño:** se ven en las próximas dos clases (entre ellos, Clean Architecture, la recomendación oficial de Flutter).
    3. **Almacenamiento:** a elección, local con `sqlite` (con CRUD completo: crear, consultar, actualizar, eliminar) o consumo de un API REST (alcanza con consumir y mostrar los datos correctamente). La cátedra ofrece un repositorio con un API "fake" que simula guardar/editar/eliminar sin persistir de verdad, para quien no tenga un API propio.
    4. **Manejador de estado:** a elección entre Provider, Riverpod, BLoC o GetX; se verá un ejemplo de cada uno en próximas clases antes de decidir.
    5. **Diseño adaptable:** `flutter_screenutil_plus` (clase 10), rutas de navegación organizadas (próxima clase), colores y temas aplicados (clase 9); multidioma es opcional.
  - **Niveles de proyecto sugeridos** (con diseños en Figma que la cátedra comparte, para quien no tenga una idea propia):
    - *Fácil:* app de notas (lista con crear, editar y eliminar).
    - *Medio:* tienda de hamburguesas (solo diseño a replicar); login/registro/recuperar contraseña + lista consumiendo la API pública de Rick and Morty; o un juego de memoria (lógica con arreglos y almacenamiento local).
    - *Difícil:* e-commerce de zapatos, con selector de tipografía y tamaño de texto; juego 2D con el paquete Flame (curso propio de Código Facilito, algo desactualizado pero con la misma lógica de base); app de cafetería. Reto opcional con premio (un mes premium de Código Facilito): álbum de cartas de Código Facilito, consumiendo su API y marcando cada carta como obtenida o no, con alguna animación.
  - **Entregables:** PDF con manual técnico (capturas del flujo de navegación entre pantallas, paleta de colores y tipografías usadas) + link a un repositorio de GitHub público y bien documentado (README con imágenes, descripción y formato markdown — funciona como portafolio). Opcional: publicar en Play Store (requiere la licencia paga única de Google Play; la profesora recomienda pagarla solo si se planea seguir publicando apps a futuro).
  - **Organización sugerida mientras tanto:** una carpeta `view` con una subcarpeta por pantalla o funcionalidad (por ejemplo `productos`, `categorias`), para ir armando el diseño; la lógica se conecta más adelante, al ver patrones arquitectónicos.

  > **Fecha de entrega: 30 de noviembre de 2026.** A partir de esa fecha empieza la corrección; la profesora estará de vacaciones desde el 30 de octubre y pide entregar antes para poder revisar a tiempo. Dudas y revisión de errores del proyecto, por Telegram. Clase movida de jueves a lunes por un evento (Flutter Conf, Cancún); próxima clase: patrones de diseño y arquitectónicos.

* **Clase 12 — Navegación**
  - **Contenido:** `Navigator` nativo (pila de ventanas, `push`/`pop`, `pushReplacement`, `pushAndRemoveUntil`) y rutas por nombre centralizadas en una clase `Router` (`onGenerateRoute`, `RouteSettings`, ruta por defecto ante un nombre no encontrado); organización de la carpeta `view` con una pantalla por carpeta; introducción a MVVM (Model/View/ViewModel) como primer patrón arquitectónico, frente a Clean Architecture para proyectos grandes; internacionalización con `flutter_localizations` + `intl`, `l10n.yaml`, archivos `.arb` por idioma, `AppLocalizations` generado automáticamente y selector de idioma manual; paquete `go_router` para que la web tenga URLs identificables por pantalla (`GoRouter`, `GoRoute`, rutas anidadas, `context.push`/`context.go`), parámetros de ruta (`state.pathParameters`, pasar solo el `id` y volver a consultar el dato completo) y `extra` para compartir un objeto completo (no persiste al recargar la página); transiciones personalizadas con `CustomTransitionPage` (`transitionsBuilder`, `Curves`, `FadeTransition` y otras). Quedaron pendientes para la próxima clase algunos errores de `go_router` con `pushNamed` en web que la profesora no llegó a resolver en vivo.

  → Detalle completo en [`flutter/conceptos.md`](./flutter/conceptos.md)

  - **Actividades asignadas:** ninguna asignada puntualmente; se retoma el proyecto final (clase 11) aplicando la navegación y, opcionalmente, el multidioma vistos hoy.

  > Diapositivas y código de la clase en el repo de la profesora ([`Marines0210/bootcamp_flutter`](https://github.com/Marines0210/bootcamp_flutter)). Dudas por Telegram; el problema de `go_router` en web quedó para revisar y comentar en la próxima clase. Próxima clase: gestión de estado y patrones arquitectónicos.