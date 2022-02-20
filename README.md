# asaitec

Notas:

- He tenido problemas con la recepción del mail con la prueba, de ahí los 10 min de tardanza.
- Como especificaba el documento, he hecho la prueba en Java, creando un proyecto Spring Boot con Maven.
- He intentado subir el jar pero github se quejaba y lo he subido todo en un comprimido. Con hacer un clean install se generará en el directorio target el jar en cuestión.
- He "improvisado" adrede un poco y en vez de outputs por pantalla o ficheros he hecho una API con la que mostrar los datos en un JSON de salida que me parecia más elegante que descargar un .csv.
- He creado 2 entidades (offerbean y productbean) en el que un producto puede tener varias ofertas vinculadas en BD. La tabla de ofertas la he planteado con un codigo y descripción con la que poder switchear para hacer unas operaciones u otras. Hay un campo llamado divisor por el que obtendría las ofertas con una división de la cantidad de productos (o precios) por el divisor y así aplicarlo todo a la oferta final, pero no me ha dado tiempo de acabar el algoritmo (switch en el codigo con una línea de comentario), aunque el planteamiento final del algoritmo lo podemos comentar en la siguiente entrevista (en caso de que la haya).
- Me habría gustado añadir una tercera entidad "invoice" o "receipt" donde registrar las ventas por BD pero no me ha dado para más y tampoco aparecía como requisito.
- He creado 3 endpoints, uno para obtener todos los productos con sus precios, uno para añadir una oferta a un producto y otro para guardar en bd una invoice y obtener el resultado en un json, aunque como he comentado antes este último no me ha dado tiempo a terminarlo.
- Hay 2 librerias que suelo usar y he añadido, lombok y mapstrut, con la que me ahorro hacer los getters/setters y para mapear objetos y ahorrarme los seteos a mano (en este caso entre beans/dtos).
- No he añadido seguridad a la API, no aparecía como requisito y no me ha dado tiempo a añadirla.
- Cualquier cosa, comentamos.
