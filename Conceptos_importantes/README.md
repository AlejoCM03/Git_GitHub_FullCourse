[Web oficial git](https://git-scm.com/)

Git es un sistema de control de versiones **distribuido, gratuito y de codigo abierto,** diseñado para manejar distintos tipos de proyectos, desde los mas pequeños, hasta los mas grandes, con velocidad y eficiencia.

### Ramas y fusiones

Git fomenta y permite tener multiples ramas locales que pueden ser completamente independientes unas de otras.
* Cambio de contexto sin fricción: Crea una rama para probar una idea, hacer algunos commits, volver a la rama original, aplicar un parche, regresar a donde estas experimentando y fusionar cambios.
* Lineas de codigo basado en Roles: Tener una rama que siempre contiene solo lo que va a producción, otra en la que hagas pruebas,y varias mas pequeñas para el trabajo diario.
* Flujo de trabajo basado en funcionalidades: Crear nuevas ramas para cada funcionalidad en la que se trabaje. Luego eliminar cada rama cuando esa funcionalidad se fusione en la linea principal.
* Experimentacion descartable: Crear una rama para experimentar, darte cuenta que no va a funcionar y simplemente eliminarla, abandonando el trabajo sin que nadie mas lo vea.

### Pequeño y rapido

Casi todas las acciones se realizan localmente, lo cual otorga una gran ventaja en velocidad sobre los sistemas centralizados que constantemente se comunican con un servidor.
Git fue construido para trabajar en el Kernel de Linux, lo que significa que desde el primer dia ha tenido que manejar eficientemente repositorios grandes. Git esta escrito en C, lo que reduce la sobrecarga de los tiempos de ejecucion asociados con los lenguajes de nivel mas alto.

### Distribuido

Es decir, que no todo depende de un unico sitio, se tiene una copia de codigo.
+ Multiples copias de seguridad: Significa que, incluso si estas utilizando un flujo de trabajo centralizado, cada usuario esencialmente tiene una copia de seguridad completa en el servidor principal. 
+ Cualquier flujo de trabajo: Se pueden implementar infinitos flujos de trabajo con relativa facilidad.
+ Flujo de trabajo estilo subversion: Git no permitara hacer _push_ si alguien mas ha hecho _push_ desde la ultima vez que hiciste _fetch_
+ Flujo de trabajo de gestor de integraciones: 
    _Gestor de integraciones:_ una persona que realiza commits en el repositorio _bendecido_. Varios desarrolladores luego clonan ese repositorio, hacen _push_ a sus propios repositorios independientes y solicitan al integrador que incorpore sus cambios.
+ Flujo de trabajo del dictador y tenientes: Algunas personas(_tenientes_) estan a cargo de un subsitema especifico del proyecto y se encargan de fusionar todos los cambios de ese subsistema. Otro integrador (_dictador_) obtiene cambios solo de sus _tenientes_ y luego hace _push_ al repositorio _bendecido_.

### Aseguramiento de datos

Es imposible cambiar cualquier archivo, fecha, mensaje de commit o cualquier otro dato en un repositorio sin cambiar los ID's de lo que esta despues de ello. Con tu ID identificado, puedes estar seguro que nada en tu historial fue modificado.

### Gratis y de codigo abierto


