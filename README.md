

## Instrucciones

### Iteración 1

Primero, tendrás que importar la base de datos que utilizaremos en esta práctica. Vamos a utilizar la base de datos de Crunchbase. Crunchbase es el principal destino para descubrir las tendencias de la industria, inversiones y noticias sobre cientos de miles de empresas a nivel mundial, desde nuevas empresas hasta las empresas más top a nivel de riquezas. Crunchbase es reconocida como la principal fuente información sobre empresas por millones de usuarios.

La base de datos contiene más de 18k de documentos, y cada uno de ello contiene una gran cantidad de información de cada compañía. Un ejemplo del documento es el siguiente:

![image](https://user-images.githubusercontent.com/23629340/36494916-d6db1770-1733-11e8-903e-5119b3c1b688.png)

1. Deberás descargar el zip de la base de datos en la ruta del repositorio.
2. Descomprime el archivo.
3. Navega hasta la carpeta del repositorio en la terminal e introduce el siguiente comando para importar la base de datos:

```bash
$ mongoimport --db companies --collection companies --file companies.json
```
_Nota: en caso de errores o de que el comando no responda, añade [--jsonArray] al final del comando anterior. 

4. Comprueba en Mongo Compass si se ha importado correctamente. 

![image](https://user-images.githubusercontent.com/23629340/36534191-1f1bc5ec-17c6-11e8-9463-4945679b98c0.png)

### Iteración 2.

Ahora estás listo para empezar a trabajar. Deberás realizar las siguiente búsquedas:

1. Todas las compañías cuyo nombre coincida con 'Babelgum'. Devuelve solo el campo `name`.
2. Todas las compañías que tengan más de 5000 empleados. Limita la búsqueda a 20 compañías y devuelve la información ordenada descendentemente por el **número de empleados** (`number_of_employees`)
3. Todas las compañías que hayan sido fundada entre el año 2000 y 2005, ambos incluídos. Devuelve sólo el campo `name` y el `founded_year`
4. Todas las compañías cuyo importe de valoración sea mayor que 100.000.000 y que haya sido fundada antes de 2010. Devuelve solo los campos `name` y `ipo`
5. Ordena todas las compañías por el campo `ipo` en orden descendente. 
6. Todas las compañías que no incluyan el campo `partners`.
7. Todas las compaías que tengan al menos 100 empleados pero menos de 1000. Devuelve sólo el campo `name` y `number_of_employees`
8. Todas las compañías que tengan menos de 1000 empleados y que hayan sido fundadas antes de 2005. Ordénalas por el número de empleados ascendentemente y limita la busqueda a 10 compañías. 
9. Recuperas las 10 compañías con más empleados ordenados por `number_of_employees` descendentemente.
10. Todas las compañías fundadas en el segundo semestre del año.  Limita la búsqueda a 1000 empresas. 
11. Todas las compañías fundadas antes del 2000 que tengan un valor de adquisición mayor que 10.000.000.
12. Todas las compañías adquiridas (acquired) después de 2010 ordenadas por la cuenta de adquisición (amount_acquisition) y devuelve sólo su `nombre` y el campo `acquisition`.
13. Ordena las empresas por orden de fundación y devuelve sólo el nombre y el año de fundación. 
14. Todas las compañías que sean de la categoría web y tengan más de 4000 empleados. Ordenalos por número de empleados en orden ascendente. 


Happy Coding!