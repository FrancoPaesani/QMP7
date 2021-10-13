# QMP7

  Recursos -> prendas, eventos y sugerencias.

* __Como usuarie de QueMePongo quiero ver todas las prendas que tengo en mi guardarropas desde el navegador para poder administrarlas.__

    * Ruta: 
      ~~~ 
      http://qmpongo/prendas?usuario=idUsuario
      ~~~
    * Método: GET
    * Códigos de respuesta posibles: 200 OK, 404 usuario invalido.
    * Body de respuesta posible: 
    
      ~~~ 
      [
        {prenda1}, {prenda2}, ... {prendaN}
      ]
      ~~~
 
* __Como usuario de QueMePongo, quiero crear una prenda desde el navegador.__
    * Ruta: 
      ~~~ 
      http://qmpongo/prendas?usuario=idUsuario
      ~~~
    * Método: POST
    * Body de envío posible:
       ~~~ 
        {prenda}
      ~~~
    * Códigos de respuesta posibles: 200/201, 400/401.
    * Body de respuesta posible: 
    
      ~~~ 
      {prenda}
      ~~~

* __Como usuarie de QueMePongo quiero ver una prenda en particular que tengo en mi guardarropas para poder editarla.__
    * Ruta: 
      ~~~ 
      http://qmpongo/prendas?usuario=idUsuario&prenda=idPrenda
      ~~~
    * Método: GET
    * Códigos de respuesta posibles: 200, 400/401/404.
    * Body de respuesta posible: 
    
      ~~~ 
      {prenda}
      ~~~

* __Como usuarie de QueMePongo, quiero poder eliminar una prenda de mi guardarropas.__
    * Ruta: 
      ~~~ 
      http://qmpongo/prendas?usuario=idUsuario&prenda=idPrenda
      ~~~
    * Método: DELETE
    * Códigos de respuesta posibles: 200/201, 400/401/404.
    * Body de respuesta posible: 
    
      ~~~ 
      {prendaEliminada}
      ~~~

* __Como usuarie de QueMePongo, quiero poder ver mis eventos para administrarlos.__
    * Ruta: 
      ~~~ 
      http://qmpongo/eventos?usuario=idUsuario
      ~~~
    * Método: GET
    * Códigos de respuesta posibles: 200, 400/401/404.
    * Body de respuesta posible: 
    
      ~~~ 
      [ {evento1}, {evento2}, ..., {eventoN} ]
      ~~~
* __Como usuarie de QueMePongo, quiero poder abrir las sugerencias de prendas para un evento 
en mi navegador.__
   * Ruta: 
      ~~~ 
      http://qmpongo/sugerencias?evento=idEvento
      ~~~
    * Método: GET
    * Códigos de respuesta posibles: 200, 400/401/404.
    * Body de respuesta posible: 
    
      ~~~ 
      [ {sugerencia1}, {sugerencia2}, ..., {sugerenciaN} ]
      ~~~
