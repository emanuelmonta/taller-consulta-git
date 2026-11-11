*1*
**Git** es un sistema de control de versiones distribuido, gratuito y de código abierto, diseñado por Linus Torvalds en 2005 para gestionar el código fuente del núcleo Linux. Su función principal es **registrar todos los cambios realizados en un proyecto a lo largo del tiempo**, permitiendo a los desarrolladores volver a versiones anteriores, comparar estados y trabajar en equipo de manera eficiente.

### ¿Qué problema resuelve en el desarrollo de software?

Antes de sistemas como Git, el desarrollo colaborativo era un proceso caótico y propenso a errores. Git soluciona problemas fundamentales como:

1. **El fin del caos de archivos duplicados:**
* **El problema antiguo:** Guardar copias como `proyecto_final.zip`, `proyecto_final_v2.zip`, `proyecto_final_revisado_por_juan.zip` dificultaba saber cuál era la versión correcta.
* **La solución de Git:** Mantiene un único directorio de proyecto conectado a una base de datos interna (el repositorio) que almacena el historial completo de forma limpia y organizada.


2. **La colaboración sin pisar el trabajo de otros:**
* **El problema antiguo:** Si dos personas editaban el mismo archivo al mismo tiempo, uno sobrescribía el trabajo del otro y se perdía información.
* **La solución de Git:** Gracias a las **ramas** (*branches*), los desarrolladores pueden trabajar en funciones o correcciones de forma aislada y segura (`feature/login`, `bugfix/header`), para luego fusionarlas (*merge*) de manera controlada. Git ayuda a detectar automáticamente conflictos si dos personas modifican exactamente la misma línea de código.


3. **La red de seguridad (historial y reversión):**
* **El problema antiguo:** Un cambio experimental rompía todo el sistema y obligaba a reescribir código desde cero o intentar recordar qué se modificó.
* **La solución de Git:** Cada cambio (*commit*) es un punto de restauración. Si algo falla, se puede **viajar en el tiempo** para inspeccionar versiones anteriores, revertir errores específicos de forma instantánea o auditar quién escribió cada línea de código y por qué.


4. **El trabajo desconectado y distribuido:**
* Al ser *distribuido*, cada desarrollador tiene una copia local completa del repositorio con todo su historial. Esto permite trabajar sin conexión a internet y sincronizar los cambios con servidores remotos (como GitHub, GitLab o Bitbucket) cuando sea necesario.

*2.*
### Diferencias clave entre Git y GitHub.

* A menudo se confunden o se usan como si fueran sinónimos, pero Git y GitHub no son lo mismo. La diferencia fundamental radica en que uno es la herramienta tecnológica y el otro es el servicio de alojamiento (hosting) en la nube. *

* Naturaleza y función: *

* Git es un software de control de versiones local e independiente. Se instala en tu computadora y se ejecuta desde la terminal para rastrear los cambios en tu código fuente y gestionar ramas de trabajo de forma offline. *

* GitHub es una plataforma web y un servicio en la nube (propiedad de Microsoft) diseñado para alojar repositorios Git, facilitando la colaboración en equipo, la revisión de código (pull requests), la gestión de tareas (issues) y la automatización (GitHub Actions). *

* Dependencia: *

* Puedes usar Git perfectamente en tu ordenador sin necesidad de tener internet ni una cuenta en GitHub. *

* GitHub depende completamente de Git para funcionar; de hecho, utiliza Git como motor principal para gestionar las versiones del código que los usuarios suben a sus servidores. *

* Infraestructura: *

* Git opera de manera distribuida; cada desarrollador tiene una copia completa del historial en su máquina local. *

* GitHub actúa como un servidor centralizado remoto donde los equipos sincronizan sus repositorios locales para centralizar el trabajo compartido. *