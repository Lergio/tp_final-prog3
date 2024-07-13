# tp_final

## Requerimientos del Proyecto

El proyecto deberá cumplir con los siguientes requerimientos mínimos:

0. General
  * Utilizar ReactJS para el desarrollo de la aplicación web.
  * Consumir una API RESTful para obtener y manipular datos. La API puede ser proporcionada por la cátedra o ser propia/pública, siempre y cuando cumpla con ciertos requisitos mínimos. Si la API es propia, esta debe implementar autenticación mediante alguno de los mecanismos vistos en clase (por ejemplo, JWT, OAuth, Basic Auth, Session Auth, etc.).
  * Utilizar Git para el control de versiones del código fuente. Cada integrante del grupo deberá realizar aportes al proyecto y mantener un historial de cambios en un repositorio de GitHub, GitLab o Bitbucket.
  * El proyecto debe ser desarrollado en un entorno de desarrollo local y desplegado en un servidor de producción. Se recomienda utilizar Vercel, Netlify, Glitch o cualquier otro servicio de hosting para desplegar la aplicación (recomendamos que sea un servicio gratuito).

1. Autenticación y Autorización
  * Implementar autenticación y manejo de sesiones utilizando JWT proporcionados por la API, o cualquier otro mecanismo de autenticación que la API requiera.
  * Asegurar que todas las solicitudes a la API estén autenticadas.

2. UI e Implementación de Componentes
  * El desarrollo de la interfaz de usuario debe ser sobre todo funcional y fácilEl desarrollo de la interfaz de usuario debe ser sobre todo funcional y fácil de usar. Se valorará la creatividad y originalidad en el diseño de la interfaz.
  * El desarrollo de la interfaz de usuario debe ser sobre todo funcional y fácilUtilizar componentes de React para manejar eficientemente el estado y el ciclo de vida de la aplicación.
  * El desarrollo de la interfaz de usuario debe ser sobre todo funcional y fácilDebe emplearse al menos un contexto para compartir información entre componentes de la aplicación, como el estado de autenticación del usuario, temas, etc.  * El desarrollo de la interfaz de usuario debe ser sobre todo funcional y fácil
  * Se recomienda utilizar los hooks de React vistos en clases para manejar el estado y el ciclo de vida de los componentes, como useState, useEffect, useContext, etc. Pero se valora el uso de hooks personalizados y el manejo de estados complejos. Pueden emplearse librerías de gestión de estados como Redux, MobX, Context API, etc. si se considera necesario, o si tienen experiencia previa con ellas.
  *  - No es necesario utilizar un framework de estilos como Bootstrap, Bulma o Tailwind CSS, pero su uso es recomendado para acelerar el desarrollo de la interfaz de usuario. Sin embargo, los alumnos pueden optar por utilizar CSS puro si lo prefieren.
     
3. Consumo de la API
  * Consumir múltiples endpoints de la API proporcionada para realizar operaciones CRUD (Create, Read, Update, Delete). Por ejemplo, si el tema seleccionado es la aplicación de música, los alumnos podrían consumir los endpoints de HarmonyHub para obtener información sobre las canciones, artistas, álbumes, géneros, etc.
  * Manejar errores de API de forma adecuada y mostrar mensajes de error informativos al usuario mediante componentes de React que representen notificaciones o alertas. Por ejemplo, si una petición POST a la API falla, mostrará una alerta con el mensaje de error correspondiente.

4. Enrutamiento
Utilizar un mecanismo de enrutamiento para navegar entre las diferentes secciones de la aplicación, como React Router. Como mínimo, se deben implementar las siguientes rutas:
  * / - Página de inicio de la aplicación. Dependiendo del tema seleccionado, esta página podría mostrar una lista de elementos (por ejemplo, canciones, películas, recetas, etc.).
  *  /login - Página de inicio de sesión. Esta página debe contener un formulario para que el usuario pueda ingresar su nombre de usuario y contraseña.
  *  /profile - Página de perfil de usuario. Esta página debe mostrar información sobre el usuario autenticado, como su nombre, correo electrónico, etc.
  *  /<resource>/ - Página de detalle de un recurso específico. Por ejemplo, si el tema seleccionado es la aplicación de música y el recurso es una canción, la ruta podría ser /songs/ y mostrar información sobre cada canción.

La creación de nuevas canciones, la edición y eliminación de canciones también se pueden realizar en esta página mediante formularios emergentes o modales.

Sin embargo, si se prefiere, se pueden implementar rutas adicionales para estas operaciones, como /songs/new, /songs/edit/:id, /songs/delete/:id, etc. Dejamos a criterio de los alumnos la implementación de estas rutas adicionales.
Además, debe incluirse al menos una ruta protegida que requiera autenticación para acceder a ella. Por ejemplo, la página de perfil de usuario solo debe ser accesible para usuarios autenticados. Por el contrario, la página principal de la aplicación debe ser accesible para todos los usuarios, incluso si no están autenticados.

Implementar un componente de navegación que muestre enlaces a las diferentes rutas de la aplicación. Este componente debe actualizarse automáticamente según el estado de autenticación del usuario.

Por último, se debe implementar al menos un componente para manejar errores, como una página 404 para rutas no encontradas.

5. Documentación
  * Documentar el código fuente de manera clara y concisa.
  * Preparar una presentación que resuma el proyecto, la arquitectura utilizada y las decisiones de diseño tomadas.
