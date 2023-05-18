# WORKSHOP 5 - API

Para este Workshop el enunciado no va a ser guiado como en otras ocasiones, debes tener en cuenta que en el mundo profesional cuando debes desarrollar una API, nadie te va a indicar:

- Qué entidades debes crear
- Qué validaciones deben tener los campos
- Qué endpoints debes hacer
- Qué librerías usar
- …
- etc

Así que teniendo en cuenta esto, vamos a darte la información que te daría un cliente o un jefe de proyecto 😛

Debes hacer un API para una aplicación de venta de productos de segunda mano, la aplicación tendrá las siguientes funcionalidades.

**REGISTRO**

![Untitled](/assets/Untitled.png)

Un usuario debe poder registrarse indicando nombre y apellidos, email y contraseña

**LOGIN**

![Untitled](/assets/Untitled%201.png)

Por supuesto, si hay un registro habrá un login… un usuario podrá hacer login con su usuario y contraseña

**BÚSQUEDA**

![Untitled](/assets/Untitled%202.png)

Independientemente de si el usuario está logado o no, podrá buscar productos

**DETALLE**

![Untitled](/assets/Untitled%203.png)

Independientemente de si el usuario está logado o no, podrá ver detalles de productos

**INICIAR / CONTINUAR UNA CONVERSACIÓN**

Si el usuario está logado, podrá iniciar o continuar una conversación con el dueño para ver si llegan a un acuerdo:

![Untitled](/assets/Untitled%204.png)

**SUBIR UN PRODUCTO**

Si el usuario está logado podrá subir productos

![Untitled](/assets/Untitled%205.png)

**MARCAR PRODUCTO COMO VENDIDO**

Un usuario que esté logado, deberá poder indicar que ha vendido un producto, para ello deberá indicar a quien se lo ha vendido.

![Untitled](/assets/Untitled%206.png)

Ahora que ya sabes la operativa de nuestra aplicación, debes ocuparte de hacer el API lo mejor posible, ten en cuenta que debes controlar tooooodas las situaciones posibles.

Por ejemplo:

- Un usuario que no esté logado no debe poder subir productos, iniciar conversaciones… etc
- Si el usuario logado es Fran (por poner un ejemplo) no puede marcar que ha vendido un producto de Edu, o que está iniciando una conversación entre Gon y Pedro… etc
- Si el usuario logado es Gon, no puede indicar que Edu vende un producto…
- No se puede realizar una venta de un producto que ya está vendido
- No se deben poder subir productos a los que les falten datos o que tengan el precio negativo… etc
- …
- Y cualquier lógica que se te ocurra que debas controlar en la aplicación

**EXTRAS**

- Añade funcionalidad para que un usuario pueda marcar / desmarcar un producto como favorito
- Añade un usuario admin que pueda hacer todas las operaciones
- Añade categorías a los productos para que un producto se pueda etiquetar dentro de una categoría (coches, muebles, ropa… etc)
- Añade filtros a las busquedas: precio, categoria…
- Añade ubicación a tus productos, puedes hacerlo por latitud / longitud, o por codigo postal
