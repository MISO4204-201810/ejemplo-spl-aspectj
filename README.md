# Ejemplo de SPL usando AspectJ y Maven

Proyecto Maven que incluye dos módulos (subproyectos) donde uno combina un aspecto con las clases y otro no.

## Contenido

El repositorio contiene un Maven con dos subproyectos. Esto significa que se tiene un archivo `pom.xml` en el directorio raíz que define los sub-modulos, y otros archivos `pom.xml` en cada subdirectorio para cada uno de los módulos.

| Archivo | Proyecto   |
| :------ | :--------- |
| `pom.xml` | ejemplo-spl-aspectj, proyecto raíz |
| `producto-proyecto-base/pom.xml`  | proyecto base que no tiene aspectos |
| `producto-con-aspectos/pom.xml`   | proyecto con aspectos que se combinan con el proyecto base |


## Ejecución

Como son varios proyectos, se recomienda compilar e instalar los archivos binarios de los proyectos en el Maven local (en el computador donde se desarrolla).

```bash
mvn install
```

La aplicación solo incluye una prueba para cada uno de los dos proyectos. Es posible ejecutar las pruebas desde la línea de comandos usando Maven.

```bash
mvn test
```

Si usa Eclipse, es posible importar el código como un `Proyecto Maven` y ejecutar las pruebas haciendo 

  - click-derecho sobre el proyecto y seleccionando `Run As > Maven test`.
  - o haciendo clic-derecho sobre la prueba y seleccionado `Run As > JUnit test`.
