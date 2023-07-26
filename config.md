# Config 
El comando git config es una función útil que sirve para definir valores de configuración de Git a nivel de un proyecto global o local. Estos niveles de configuración se corresponden con archivos de texto .gitconfig. Al ejecutar git config, se modificará un archivo de texto de configuración. Analizaremos los ajustes de configuración comunes como, por ejemplo, el correo electrónico, el nombre de usuario y el editor. Explicaremos los alias de Git, que te permiten crear atajos para las operaciones de Git utilizadas con frecuencia. Familiarizarte con git config y los diversos ajustes de configuración de Git te ayudará a crear un flujo de trabajo de Git potente y personalizado.

### Uso 

El caso práctico más básico de git config es invocarlo con un nombre de configuración, que mostrará el valor definido con ese nombre. Los nombres de configuración son cadenas delimitadas por puntos que se componen de una "sección" y una "clave" en función de su jerarquía. Por ejemplo: user.email.

 `git config user.email`
 
 En este ejemplo, "email" es una propiedad secundaria del bloque de configuración del usuario. Devolverá la dirección de correo electrónico configurada, si la hay, que Git asociará con las confirmaciones creadas localmente.
 
 ### Niveles y archivos de git config 
 
 Antes de analizar en más detalle el uso de git config, vamos a pararnos un momento a hablar de los niveles de configuración. El comando git config puede aceptar argumentos para especificar en qué nivel de configuración debe operar. Dispones de los siguientes niveles de configuración:
 `--local`
 
 De manera predeterminada, git config escribirá en un nivel local si no se pasa ninguna opción de configuración. La configuración de nivel local se aplica al repositorio de contexto en el que se invoca git config. Los valores de configuración locales se almacenan en un archivo que se puede encontrar en el directorio .git del repositorio: .git/config
 `--global`
 
 La configuración de nivel global es específica del usuario, lo que significa que se aplica al usuario de un sistema operativo. Los valores de configuración globales se almacenan en un archivo que se encuentra en el directorio principal de un usuario. ~ /.gitconfig en sistemas unix y C:\\.gitconfig en Windows.
 `--system`
 
 La configuración de nivel de sistema se aplica a toda una máquina. Afecta a todos los usuarios de un sistema operativo y a todos los repositorios. El archivo de configuración de nivel de sistema se encuentra en un archivo gitconfig fuera de la ruta raíz del sistema. $(prefix)/etc/gitconfig en sistemas Unix. En Windows, este archivo se encuentra en C:\Documents and Settings\Todos los usuarios\Datos de programa\Git\config en Windows XP, y en C:\ProgramData\Git\config en Windows Vista y las versiones más recientes.

Por lo tanto, el nivel de prioridad para los niveles de configuración es el siguiente: local, global y sistema. Esto significa que, cuando se busque un valor de configuración, Git empezará en el nivel local e irá subiendo hasta el nivel de sistema.

### Resumen 

En este artículo, hemos analizado el uso del comando git config. Hemos explicado cómo el comando es un método práctico para editar archivos de git config sin procesar en el sistema de archivos. Hemos visto operaciones básicas de lectura y escritura para las opciones de configuración. Hemos echado un vistazo a los patrones de configuración comunes:

Cómo configurar el editor de Git
Cómo sobrescribir los niveles de configuración
Cómo restablecer los valores predeterminados de configuración
Cómo personalizar los colores de Git
En general, git config es una herramienta auxiliar que proporciona un acceso rápido para editar archivos git config sin procesar en el disco. Se han tratado en profundidad las opciones de personalización. Es necesario tener conocimientos básicos sobre las opciones de configuración de git si se desea configurar un repositorio. Consulta nuestra guía y observa una demostración de los aspectos básicos en ella.