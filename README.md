# SGVD

# Sistema de control de versiones distribuido
Un sistema de control de versiones distribuido (DVCS) es un sistema de control de versiones que funciona con un principio de hardware distribuido o, en algunos otros sistemas informáticos distribuidos, como una red virtual.

# Techopedia explica el Sistema de control de versiones distribuido (DVCS)
Con un sistema de control de versiones distribuido (DVCS), se rastrean diferentes revisiones de archivos en todo el sistema distribuido. Esto puede requerir estrategias específicas de consistencia para que los colaboradores u otros usuarios sepan qué está sucediendo con los archivos en un momento dado. Por ejemplo, un tipo popular de DVCS implica el uso de un repositorio como intermediario entre estaciones de trabajo y servidores. El repositorio contiene versiones revisadas de archivos, y el sistema de software verifica periódicamente con el repositorio para propósitos de consistencia.

La idea esencial de un DVCS es poder rastrear los cambios en archivos o documentos individuales. Las diferentes medidas de seguimiento funcionan de manera diferente para permitir una investigación transparente sobre cómo han cambiado los archivos específicos y cuándo han cambiado. Algunos expertos de TI hablan sobre un proceso **"push / pull"** en el que se intercambia información entre servidores y otros componentes para ayudar a mantener las versiones de archivos en el sistema moderno y consistente.

# Distribuido vs centralizado

 Los sistemas de control de versiones distribuidos (DVCS) utilizan un enfoque de igual a igual para el control de versiones, a diferencia del enfoque cliente-servidor de los sistemas centralizados. El control de revisión distribuido sincroniza los repositorios transfiriendo parches de igual a igual. No existe una única versión central del código base; en su lugar, cada usuario tiene una copia de trabajo y el historial de cambios completo.

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
