# 1. ¿Qué son los Encabezados HTTP? (2 puntos)

*Son los parámetros que se envían en una petición o respuesta HTTP al cliente o al servidor para proporcionar información sobre la transacción en curso.*

# 2. ¿A qué se asemejan los encabezados HTTP en la analogía de la "casa"? (2 puntos)

*La Casa (Servidor): El servidor es como una casa a la que se quiere acceder. Esta casa tiene varias habitaciones (recursos) que se desea visitar, como una sala de estar (página principal), un cuarto de baño (formulario de contacto), etc.*

*La Puerta (Solicitudes): Cuando quieres entrar a la casa, necesitas tocar la puerta (hacer una solicitud HTTP). La puerta está protegida y tiene un sistema de seguridad, así que debes usar la llave correcta (usar el método HTTP correcto, como GET o POST) para entrar.*

*Los Encabezados (Cartas de Presentación): Antes de poder entrar, también se necesita entregar unas cartas de presentación (encabezados HTTP). Estas cartas incluyen información importante sobre quien desea tener acceso y su propósito:*

*Las Reglas de la Casa (Políticas de Seguridad): La casa tiene reglas y políticas a seguir, como por ejemplo:*
*Cierre de puertas (CORS - Cross-Origin Resource Sharing).*
*No entrar en ciertas habitaciones (Content Security Policy)*

*Las Respuestas (Recibir Permiso): Después de presentar las cartas, el dueño de la casa (servidor) decide si da el acceso. Responde con un mensaje (código de estado HTTP):*

*200 OK: Todo está bien, puedes entrar.*

*403 Forbidden: No tienes permiso para entrar aquí.*

*404 Not Found: Esa habitación no existe.*


*Las Acciones Dentro de la Casa (Manipulación de Recursos): Una vez dentro, se pueden hacer varias cosas: ver, modificar o agregar información (hacer solicitudes GET, POST, PUT o DELETE). Todo esto también se refleja en el intercambio de cartas (encabezados) mientras se mueve de habitación en habitación.*

# 3. ¿Qué tipo de información se envía a los servidores web cuando se realiza un proceso de registro o inicio de sesión? (3 puntos)

*Cuando se realiza un proceso de registro o inicio de sesión en un sitio web, generalmente se envía la siguiente información al servidor web:*

*Datos de autenticación: Tales como Nombre de usuario o dirección de correo electrónico, contraseña, etc*

*Datos personales (en registro): Durante el proceso de registro, es común que se soliciten datos adicionales, como: Nombre completo, Fecha de nacimiento, Dirección o ubicación, Número de teléfono, etc.*

*Token de autenticación (en algunos casos de inicio de sesión): Cuando el usuario ya ha iniciado sesión previamente y se quiere verificar su identidad sin pedir una nueva autenticación, se puede enviar un token, como un JWT (JSON Web Token), que almacena información codificada sobre la sesión.*

*Cookies y datos de sesión: Pueden incluir identificadores de sesión, cookies específicas que permitan al servidor reconocer al usuario en posteriores visitas o validar su autenticación actual.*

*Información del dispositivo y navegador (User-Agent): Los navegadores envían automáticamente información sobre el tipo de dispositivo, navegador y sistema operativo que se está utilizando. Esto puede ser utilizado para verificar compatibilidad, analizar patrones de uso o, en algunos casos, para implementar medidas de seguridad adicionales.*

*Dirección IP: Aunque no siempre es enviada explícitamente como un campo, el servidor generalmente tiene acceso a la dirección IP desde la que se realiza la solicitud. Esto puede ser usado para fines de seguridad, como detectar intentos de acceso no autorizados o crear restricciones geográficas.*

*Datos adicionales (como CAPTCHA): Si hay mecanismos de seguridad adicionales como CAPTCHA para evitar bots, la validación de estas herramientas también se envía como parte del proceso de autenticación.*


# 4. ¿Qué son los "Response Headers"? (3 puntos)

*Los Response Headers son un tipo de Encabezado HTTP que se puede utilizar en una respuesta HTTP y que no está relacionado con el contenido del mensaje.*

# 5. ¿Cuál es la importancia de los "Response Headers"? (3 puntos)

*Nos ofrecen una capa básica de proteccióna la información, para que la misma viaje de forma segura entre el usuario y el servidor.*

# 6. ¿Qué es la "pestaña Network" en las herramientas para desarrolladores? (2 puntos)

*La pestaña "Network" en las herramientas para desarrolladores de los navegadores web es una sección que permite ver y analizar las solicitudes y respuestas de red que se realizan cuando un sitio web se carga o interactúa con un servidor. Es una herramienta esencial para los desarrolladores web, ya que proporciona detalles sobre cómo el navegador y el servidor se comunican, lo que puede ser útil para depurar, optimizar el rendimiento y resolver problemas de red o de recursos.*

# 7. ¿Cuál es el principal objetivo de los Encabezados HTTP en términos de seguridad? (3 puntos)

*El principal objetivo de los Encabezados HTTP en términos de seguridad es proteger la comunicación entre el cliente (como el navegador web) y el servidor, asegurando que los datos se transmitan y se procesen de manera segura. Los encabezados de seguridad ayudan a mitigar diversas amenazas, como la suplantación de contenido, los ataques de tipo cross-site scripting (XSS), ataques de clickjacking, e incluso el uso de recursos no seguros.*

# 8. ¿Qué tipos de Encabezados HTTP existen para proteger la información? (3 puntos)

*Entre los Encabezados HTTP más comunes utilizados para proteger la información se encuentran:*
*1. Content-Security-Policy (CSP)*
*2. Strict-Transport-Security (HSTS)*
*3. X-Content-Type-Options*

# 9. ¿Qué es la encriptación y cómo se relaciona con los Encabezados HTTP en la seguridad web? (3 puntos)

*La encriptación es el proceso de convertir datos legibles (texto plano) en un formato codificado (texto cifrado) para que solo personas o sistemas autorizados puedan descifrarlos y acceder a la información original. En términos simples, la encriptación asegura que los datos transmitidos a través de una red, como la web, sean ilegibles para cualquier persona que no tenga la clave correcta para descifrarlos, lo que protege la información de ser interceptada, manipulada o robada.*
*En conjunto, la encriptación y los encabezados HTTP proporcionan un enfoque integral de seguridad, asegurando que los datos viajen de manera segura y que las aplicaciones web sean más resistentes a diversos tipos de ataques.*

# 10. ¿Cuál es el nombre de la página web oficial de Mozilla con documentación sobre Encabezados HTTP? (1 punto)

*MDN Web Docs*

# 11. ¿Cuáles son algunos ejemplos de Encabezados HTTP utilizados para la autenticación? (3 puntos)

*Algunos de los ejemplos de Encabezados HTTP utilizados para la autenticación son:*

**WWW-Authenticate:**
*Define el método de autenticación que debería ser usado para tener acceso al contenido.*

**Authorization:**
*Contiene las credenciales para autenticar a un usuario con un servidor.*

**Proxy-Authenticate:**
*Define el método de autenticación que debería ser usado para tener acceso a un recurso que se encuentre tras un servidor proxy.*

**Proxy-Authorization:**
*Contiene las credenciales para autenticar a un usuario con un servidor proxy.*

# 12. ¿Qué son las cookies y qué función cumplen? (3 puntos)

*Una cookie HTTP, cookie web o cookie de navegador es una pequeña pieza de datos que un servidor envía a el navegador web del usuario. El navegador guarda estos datos y los envía de regreso junto con la nueva petición al mismo servidor. Las cookies se usan generalmente para decirle al servidor que dos peticiones tienen su origen en el mismo navegador web lo que permite, por ejemplo, mantener la sesión de un usuario abierta. Las cookies permiten recordar la información de estado en vista a que el protocolo HTTP es un protocolo sin estado.*

# 13. ¿Cuales son los 2 tipos de Encabezados HTTP se utilizan para la protección de contenido web? (3 puntos)

*1 Response Headers.*
*2 Request Headers*

# 14. ¿Qué función cumple el Content Security Policy (CSP)? (3 puntos)

*La Política de seguridad de contenido (CSP) es una función que ayuda a prevenir o minimizar el riesgo de ciertos tipos de amenazas de seguridad. Consiste en una serie de instrucciones que un sitio web envía a un navegador y que le indican que debe imponer restricciones sobre las acciones que el código que compone el sitio puede realizar*

*El principal caso de uso de CSP es controlar qué recursos, en particular recursos JavaScript, puede cargar un documento. Esto se utiliza principalmente como defensa contra ataques de secuencias de comandos entre sitios, en los que un atacante puede inyectar código malicioso en el sitio de la víctima.*

*Un CSP también puede tener otros propósitos, entre ellos defenderse contra el clickjacking y ayudar a garantizar que las páginas de un sitio se carguen mediante HTTPS.*

# 15. ¿Qué es el "XSS" y cómo se relaciona con los Encabezados HTTP? (4 puntos)

*Cross-site scripting (XSS) es un exploit de seguridad que permite a un atacante inyectar en un sitio web código malicioso del lado del cliente. Este código es ejecutado por las víctimas y permite a los atacantes eludir los controles de acceso y hacerse pasar por usuarios.*

# 16. (*) ¿Qué encabezado ayuda al rendimiento de una página web? (3 puntos)

*El encabezado Cache-Control es uno de los principales encabezados HTTP que ayuda al rendimiento de una página web. Este encabezado permite a los desarrolladores y servidores controlar cómo los recursos de una página web se almacenan en caché por el navegador y otros intermediarios (como proxies o sistemas de CDN), lo que puede reducir el tiempo de carga y mejorar el rendimiento general.*

# 17. ¿Cómo se identifican los Encabezados HTTP antes del 2012? (2 puntos)

*Antes del 2012, los Encabezados HTTP que no eran oficialmente estándar en el protocolo pero que aportaban funcionalidad adicional se identificaban frecuentemente mediante el prefijo X-. Este prefijo "X-" indicaba que se trataba de un encabezado personalizado o experimental, desarrollado para ofrecer nuevas capacidades antes de ser considerados estándares oficiales en el protocolo HTTP. Estos encabezados se conocían como "encabezados no estándar" o "encabezados personalizados".*

# 18. (*) ¿Qué es SEO en el contexto de la web? (2 puntos)

*SEO (Search Engine Optimization), o Optimización para Motores de Búsqueda, es el proceso de mejorar la visibilidad y el posicionamiento de un sitio web en los resultados orgánicos (no pagados) de los motores de búsqueda como Google, Bing o Yahoo. El objetivo principal de SEO es atraer más tráfico de calidad a un sitio web al hacer que sea más "visible" y relevante para las búsquedas de los usuarios relacionadas con su contenido o servicios.*

# 19. ¿Cuál es el atajo del teclado (shortcut) para acceder al inspector de elementos en el navegador? (1 punto)

*Presionar tecla F12*

# 20. ¿Qué significa "HTTP" en las siglas de Encabezados HTTP? (1 punto)

*HTTP significa "HyperText Transfer Protocol" o "Protocolo de Transferencia de Hipertexto".*

# 21. (*) ¿Cuál es la diferencia entre los encabezados HTTP y los encabezados HTTPS? (4 puntos)

*HTTP y HTTPS utilizan los mismos encabezados en cuanto a formato y función general, pero la gran diferencia es que HTTPS proporciona un canal de comunicación seguro mediante la encriptación de los datos. Esto convierte a HTTPS en una opción preferida para cualquier comunicación web que requiera confidencialidad, seguridad y autenticación del servidor.*

# 22. (*) ¿Cuáles son los tipos de métodos HTTP qué mas se utilizan? (mencione al menos 5) (4 puntos)

*Entre los tipos de métodos HTTP más comunes están:*

*GET: Obtener datos.*

*POST: Crear nuevos datos o recursos.*

*PUT: Actualizar o reemplazar completamente un recurso.*

*DELETE: Eliminar un recurso.*

*PATCH: Modificar parcialmente un recurso existente.*

# 23. (*) ¿Qué permiten hacer las herramientas de desarrollo del navegador con respecto a los encabezados HTTP? (4 puntos)

*Las herramientas de desarrollo del navegador, también conocidas como DevTools, permiten a los desarrolladores inspeccionar y analizar en detalle el comportamiento de los encabezados HTTP de las solicitudes y respuestas entre el navegador y el servidor. Estas herramientas proporcionan una serie de funcionalidades que son clave para depurar, optimizar y mejorar la seguridad de las aplicaciones web.*

*Entre las funcionalidades que ofrecen están: Inspeccionar las solicitudes y respuestas HTTP; Analizar el rendimiento de las solicitudes; Depurar problemas de seguridad relacionados con encabezados; Modificar y reenviar solicitudes; Analizar cookies y encabezados relacionados; Monitorear peticiones de CORS (Cross-Origin Resource Sharing).*

# 24. (*) ¿Qué es un "Proxy" y cómo se relaciona con los Encabezados HTTP? (4 puntos)

*Un proxy es un servidor intermedio que actúa como intermediario entre un cliente (por ejemplo, un navegador web) y un servidor web. El cliente realiza solicitudes a través del proxy, que luego reenvía esas solicitudes al servidor. A su vez, el servidor responde al proxy, que transmite la respuesta de vuelta al cliente. Los proxies son comúnmente utilizados para mejorar el rendimiento, filtrar contenido, esconder la identidad del usuario o controlar el acceso a ciertos recursos.*

*El proxy actúa como un intermediario entre el cliente y el servidor, y en el proceso, puede modificar, agregar o eliminar encabezados HTTP. Estos encabezados son esenciales para gestionar la comunicación, optimizar el rendimiento, asegurar la privacidad y garantizar que las políticas de acceso y seguridad se cumplan. Por lo tanto, los proxies tienen un impacto directo en la forma en que los encabezados HTTP se manejan en las aplicaciones web.*

# 25. (*) ¿Cómo se pueden usar los Encabezados HTTP para optimizar el SEO de un sitio web? (4 puntos)

*Utilidades de los encabezados HTTP para optimizar el SEO:*

**1- Velocidad de carga:**

- *Cache-Control, Expires y ETag mejoran el tiempo de carga al gestionar la caché.*
- *Accept-Encoding permite la compresión (Gzip/Brotli) para reducir el tamaño de los recursos enviados.*

**2- Seguridad:**

- *Strict-Transport-Security (HSTS) asegura el uso de HTTPS, mejorando la confianza del sitio.*
- *Content-Security-Policy (CSP) y X-Content-Type-Options ayudan a proteger contra ataques web.*

**3- Redirecciones:**

- *301 (permanente) y 302 (temporal) gestionan correctamente los cambios de URL, transfiriendo autoridad y evitando enlaces rotos.*

**4- Control de indexación:**

- *X-Robots-Tag permite controlar la indexación de recursos no HTML.*
- *Políticas de CORS aseguran la accesibilidad de recursos externos.*

**5- Optimización móvil:**

- *Encabezado de viewport asegura una visualización adecuada en dispositivos móviles, mejorando la experiencia del usuario.*

*Estos elementos mejoran la velocidad, seguridad, indexación y accesibilidad del sitio, aspectos clave para un buen posicionamiento SEO.*
