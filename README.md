# SGVD

# Sistema de control de versiones distribuido
Un sistema de control de versiones distribuido (DVCS) es un sistema de control de versiones que funciona con un principio de hardware distribuido o, en algunos otros sistemas informáticos distribuidos, como una red virtual.

# Sistema de control de versiones distribuido (DVCS)
Los Sistemas de Control de Versiones permiten gestionar los cambios realizados en el código fuente de programas o documentos. En los años 90 la mayoría de VCS era sistemas centralizados, en el que un servidor central guarda toda la información y los clientes se conectan al servidor. En el mundo del software libre, el sistema más popular fue CVS (Concurrent Versions System), sustituido a partir del 2004 por Subversion.

Los primeros sistemas DVCS de código abierto incluyeron Arch , Monotone y Darcs . Sin embargo, los DVCS de código abierto nunca fueron muy populares hasta el lanzamiento de Git y Mercurial .

En el año 2000 apareció BitKeeper, un sistema de control de versiones distribuido, en el que cada cliente mantiene su propia copia completa del repositorio y puede trabajar sin estar conectado al servidor. BitKeeper era un programa comercial, pero permitía su uso en proyectos de software libre. Entre 2002 y 2005, BitKeeper se utilizó en el desarrollo del kernel Linux, pero en 2005 BitKeeper revocó la licencia que había concedido a los programadores del kernel. Aunque para entonces ya había sistemas de control de versiones distribuidos libres (Monotone, darcs), Linus Torvalds decidió crear un nuevo programa, Git, que se publicó en abril de 2005.

La idea esencial de un DVCS es poder rastrear los cambios en archivos o documentos individuales. Las diferentes medidas de seguimiento funcionan de manera diferente para permitir una investigación transparente sobre cómo han cambiado los archivos específicos y cuándo han cambiado. Algunos expertos de TI hablan sobre un proceso **"push / pull"** en el que se intercambia información entre servidores y otros componentes para ayudar a mantener las versiones de archivos en el sistema moderno y consistente.

## Las ventajas de DVCS (en comparación con los sistemas centralizados) incluyen:
- Permite a los usuarios trabajar de forma productiva cuando no están conectados a una red.
- Las operaciones comunes (como confirmaciones, visualización del historial y reversión de cambios) son más rápidas para DVCS, porque no es necesario comunicarse con un - servidor central. [6] Con DVCS, la comunicación solo es necesaria cuando se comparten cambios entre otros pares.
- Permite el trabajo privado, por lo que los usuarios pueden usar sus cambios incluso para los primeros borradores que no desean publicar.
- Las copias de trabajo funcionan eficazmente como copias de seguridad remotas, lo que evita depender de una máquina física como punto único de falla. [6]
- Permite el uso de varios modelos de desarrollo, como el uso de ramas de desarrollo o un modelo de Comandante / Teniente.
- Permite el control centralizado de la "versión de lanzamiento" del proyecto.
- En los proyectos de software FOSS , es mucho más fácil crear una bifurcación de proyecto a partir de un proyecto que está estancado debido a conflictos de liderazgo o desacuerdos de diseño.

## Las desventajas de DVCS (en comparación con los sistemas centralizados) incluyen:
- La verificación inicial de un repositorio es más lenta en comparación con la verificación en un sistema de control de versiones centralizado, porque todas las ramas y el historial de revisiones se copian en la máquina local de forma predeterminada.
- La falta de mecanismos de bloqueo que forma parte de la mayoría de los VCS centralizados y aún juega un papel importante cuando se trata de archivos binarios que no se pueden combinar, como activos gráficos o paquetes binarios o XML de archivos únicos demasiado complejos (por ejemplo, documentos de Office, archivos PowerBI, SQL - - Server Paquetes de BI de herramientas de datos, etc.).
- Se requiere almacenamiento adicional para que cada usuario tenga una copia completa del historial completo de la base de código. [7]
- Mayor exposición de la base del código, ya que cada participante tiene una copia localmente vulnerable. 


# Modelo de trabajo 
El modelo distribuido generalmente es más adecuado para proyectos grandes con desarrolladores parcialmente independientes, como el proyecto del kernel de Linux, porque los desarrolladores pueden trabajar de forma independiente y enviar sus cambios para fusionarlos (o rechazarlos). El modelo distribuido permite adoptar de forma flexible flujos de trabajo de contribución de código fuente personalizados. El flujo de trabajo del integrador es el más utilizado. En el modelo centralizado, los desarrolladores deben serializar su trabajo, para evitar problemas con diferentes versiones.

# Repositorios centrales y de sucursales
Cada proyecto tiene un repositorio central que se considera el repositorio oficial, que es administrado por los mantenedores del proyecto. Los desarrolladores clonan este repositorio para crear copias locales idénticas del código base. Los cambios de código fuente en el repositorio central se sincronizan periódicamente con el repositorio local.

El desarrollador crea una nueva rama en su repositorio local y modifica el código fuente en esa rama. Una vez que se realiza el desarrollo, el cambio debe integrarse en el repositorio central.

#  Solicitudes de extracción

Las contribuciones a un repositorio de código fuente que utiliza un sistema de control de versiones distribuido se realizan comúnmente mediante una solicitud de extracción , también conocida como solicitud de combinación . [10] El colaborador solicita que el encargado del proyecto extraiga el cambio de código fuente, de ahí el nombre "solicitud de extracción". El mantenedor tiene que fusionar la solicitud de extracción si la contribución debe convertirse en parte de la base de origen. [11]

El desarrollador crea una solicitud de extracción para notificar a los mantenedores de un nuevo cambio; un hilo de comentarios está asociado con cada solicitud de extracción. Esto permite una discusión enfocada de los cambios de código . Las solicitudes de extracción enviadas son visibles para cualquier persona con acceso al repositorio. Los encargados de mantenimiento pueden aceptar o rechazar una solicitud de extracción. 

Una vez que se revisa y aprueba la solicitud de extracción, se fusiona con el repositorio. Dependiendo del flujo de trabajo establecido, es posible que sea necesario probar el código antes de incluirlo en la versión oficial. Por lo tanto, algunos proyectos contienen una rama especial para fusionar solicitudes de extracción no probadas. [11] [13] Otros proyectos ejecutan un conjunto de pruebas automatizado en cada solicitud de extracción, utilizando una herramienta de integración continua como Travis CI , y el revisor verifica que cualquier código nuevo tenga la cobertura de prueba adecuada.

