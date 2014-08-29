Este subdirectorio NO ES PARTE de la aplicación FLOD, pero sirve para guardar los datos usados durante el demo presentado en la media party 2014


Para cargar los datos y dejarlos disponibles en un SPARQL endpoint

* Descomprimir escuelas.ttl.gz

* Bajar Apache Fuseki desde https://repository.apache.org/content/repositories/snapshots/org/apache/jena/jena-fuseki/1.1.1-SNAPSHOT/

* Descomprimir Fuseki en algun directorio `$FUSEKI`

* Entrar a `$FUSEKI`

* `mkdir escuela`

* `./fuseki-server --loc escuelas --update /escuelas`
	* Esto va a dejar corriendo la base de datos

* En otro terminal, desde $FUSEKI, ejecutar `./s-put http://localhost:3030/escuelas/data default $PATH_TO_THIS_REPO/data/escuelas.ttl`
	* Esto carga los datos de ejemplo


