# SGVD

# Sistema de control de versiones distribuido
Un sistema de control de versiones distribuido (DVCS) es un sistema de control de versiones que funciona con un principio de hardware distribuido o, en algunos otros sistemas informáticos distribuidos, como una red virtual.

# Sistema de control de versiones distribuido (DVCS)
Los Sistemas de Control de Versiones permiten gestionar los cambios realizados en el código fuente de programas o documentos. En los años 90 la mayoría de VCS era sistemas centralizados, en el que un servidor central guarda toda la información y los clientes se conectan al servidor. En el mundo del software libre, el sistema más popular fue CVS (Concurrent Versions System), sustituido a partir del 2004 por Subversion.

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
