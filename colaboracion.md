# Preguntas de investigación

## Juan Pasamar

1. ¿Que es un repositorio remoto y en qué se diferencia de uno local?

En esencia, son lo mismo: un sistema donde controlas las versiones de tu software, pero se diferencian en un punto clave:

- El repositorio remoto es un repositorio centralizado en la nube, donde todos los que tengan el repositorio local en su máquina convergen.
- El repositorio local es un control de versiones a nivel de máquina.

2. ¿Qué es un "fork" en GitHub y cómo se usa en proyectos colaborativos?

Los repositorios públicos en GitHub tienen la opción de crearles un "fork". Esto sirve para que la comunidad pueda añadir su propio código al software inicial, y crear una `pull request`con los cambios a los dueños del repositorio original.

De esta manera, los cambios no afectan al repositorio original.

En proyectos colaborativos, la comunidad crea forks del repositorio para crear sus propias funcionalidades.

3. ¿Qué es un "pull request" (PR) y cuál es su propósito? Describe el flujo de trabajo típico.

Un "pull request" es una solicitud para que los cambios de una rama o fork se implanten a otra rama. Lo podemos considerar una "solicitud de merge".

En el flujo de trabajo típico, cada funcionalidad que deseemos agregar al software tiene su propia rama en la que trabajar de manera independiente para evitar errores. Una vez acabamos dicha funcionalidad, creamos una PR en GitHub a la rama de producción, que el encargado deberá revisar para implementar.

4. ¿Qué son los "issues" y los "proyectos" en GitHub? ¿Para qué sirven?

Los issues en GitHub son herramientas que permiten a los desarrolladores rastrear errores, sugerir mejoras o discutir nuevas ideas dentro de un repositorio. Funcionan como una especie de lista de tareas dentro del proyecto.

Los proyectos en GitHub son tableros organizativos que ayudan a planificar y gestionar el desarrollo de un software, similar a herramientas como Trello o Jira.

5. Explica la importancia de las ramas en un entorno de trabajo colaborativo. ¿Cómo se suelen organizar
   las ramas en proyectos grandes (ejemplo: main, dev, feature)?

Las ramas en un entorno colaborativo son muy importantes, ya que evitan conflictos debido a que el trabajo de unos no influye en el de otros. Facilitan la revisión del código gracias a las pull requests. Permiten experimentar sin riesgos ya que los cambios no afectan al código fuente principal, y mejoran el flujo de trabajo.

- main (o master) – La rama principal y estable. Contiene la versión de producción del proyecto. Solo se fusionan cambios que han sido probados y aprobados.
- dev (desarrollo) – Es la rama donde se integran los cambios antes de pasarlos a main. Aquí se prueban nuevas funcionalidades antes de ser consideradas estables.
- feature/nombre-feature – Ramas específicas para desarrollar nuevas características. Cada nueva funcionalidad tiene su propia rama basada en dev y se elimina después de fusionarse.
- hotfix/nombre-hotfix – Ramas creadas para corregir errores urgentes en producción. Estas se derivan de main y, una vez corregido el error, se fusionan tanto en main como en dev.
- release/nombre-release – Se usa para preparar una nueva versión estable. Permite hacer pruebas finales antes de enviarla a producción.
