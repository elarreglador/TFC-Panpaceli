# TFC-Panpaceli

Panpaceli es un escaparate especializado en alimentos sin alergenos en el que diferentes vendedores muestran sus productos.

# Capturas de pantalla (Vendedor)

<table>
  <tr>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-29-00-708_com.example.panpaceli.jpg" alt="" width="200" title="Datos de vendedor"></td>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-29-09-819_com.example.panpaceli.jpg" alt="" width="200" title="Listado de pedidos de vendedor"></td>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-29-19-043_com.example.panpaceli.jpg" alt="" width="200" title="Listado de productos propios"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-29-24-270_com.example.panpaceli.jpg" alt="" width="200" title="Info."></td>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-29-30-548_com.example.panpaceli.jpg" alt="" width="200" title="Info."></td>
    <td><img src="" alt="" width="200" title=""></td>
  </tr>
</table>

# Capturas de pantalla (Cliente)

<table>
  <tr>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-47-30-770_com.example.panpaceli.jpg" alt="" width="200" title="Datos de cliente"></td>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-47-43-810_com.example.panpaceli.jpg" alt="" width="200" title="Listado de productos disponibles"></td>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-47-48-038_com.example.panpaceli.jpg" alt="" width="200" title="Listado de pedidos de cliente"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-47-54-987_com.example.panpaceli.jpg" alt="" width="200" title="Info."></td>
    <td><img src="https://github.com/elarreglador/TFC-Panpaceli/blob/main/Img/Fotos%20y%20capturas/Capturas%20propias/Screenshot_2025-05-19-17-48-00-891_com.example.panpaceli.jpg" alt="" width="200" title="Info."></td>
    <td><img src="" alt="" width="200" title=""></td>
  </tr>
</table>

# Registro de actividad (git log)

Se está utilizando una convención de mensajes de commit con emojis y prefijos que categorizan el tipo de cambio, lo que facilita la lectura.

El log muestra claramente diferentes etapas o focos en el desarrollo:

### Fase Inicial (Documentación y Preparativos):

Desde abril de 2025, se han generado commits relacionados con la documentación (README, anexo, memoria, normativas aplicables como RGPD, LSSI-CE, Reglamento UE 1169/2011, etc.), la configuración del entorno (instalación de Ubuntu, Docker, Node-RED, MariaDB, SSH), y la estructura inicial del proyecto (tablas de la BD, creación de archivos, paleta de colores, logo).

### Fase de Autenticación y API (Finales de abril - Principios de mayo):

A partir del 20 de abril de 2025, se intensifica el desarrollo de la aplicación con la implementación de:

Navegación (go_router, login <-> signup).

Creación de usuarios (newCliente).

Manejo de tokens de seguridad (generación, almacenamiento, renovación, verificación), incluyendo la implementación de HTTPS para la API.

Comunicación con Node-RED y Postman para los endpoints de la API (setValue, getValue, idEnTabla).

Manejo de datos de cliente y vendedor.

### Fase de Funcionalidades Principales (Mayo):

A partir de mediados de mayo, me centro en la lógica de negocio y las funcionalidades clave de la aplicación:

Gestión de Productos: Creación, edición, eliminación y activación/desactivación de productos por parte de los vendedores.

Pedidos: Implementación de la funcionalidad para que los clientes puedan encargar productos (nuevoEncargo), mostrar el estado de los pedidos, permitir a los vendedores ver sus pedidos y cambiar su estado (pedidoSetState).

Geolocalización y Distancia: Adición de funciones GPS (getCurrentLocation, distancePythagoras), visualización de la distancia a los vendedores y filtrado de productos por distancia.

Mejoras Estéticas: Numerosos commits de Mejora estética y Cambio menor indican un pulido constante de la interfaz de usuario, incluyendo temas (darkTheme), imágenes de fondo dinámicas y la apariencia de las listas.

Front y back en paralelo: el desarrollo frontend/móvil va de la mano con la implementación del backend (API REST).

### Git log
```
* 9941d4a [David Moreno | 2025-05-28]  (HEAD -> main, origin/main, origin/HEAD) 🔴🐞 Node-red export: Corregido bug de guardado nuevo producto
* 8be5952 [elarreglador | 2025-05-27]  🐞 Bug corregido: Fuerza recarga de searchScreen tras 1a actiavacion GPS
* 0e65894 [elarreglador | 2025-05-24]  🐞 Bug corregido: Filtro de productos por distancia
* 37347fe [David Moreno | 2025-05-22]  (tag: v0.5.10) ✨ Cambio menor: notificacion a vendedor para recarga tras editar producto
* fe797e6 [David Moreno | 2025-05-22]  🐞 Bug corregido: Muestra distancia al vendedor
* 0acf720 [David Moreno | 2025-05-21]  🐞 Bug corregido: Corregido funcionamiento switch GPS
* 2343a44 [David Moreno | 2025-05-21]  ✨ Cambio menor:	Eliminados warnings relativos al theme
* ec8f230 [David Moreno | 2025-05-21]  🔴 Node-red export: Solucionado bug en updateProducto
* f0537fc [David Moreno | 2025-05-21]  🐞 Bug corregido: productFormScreen guarda los alergenos
* e633bc2 [David Moreno | 2025-05-21]  Agregado agradecimiento y propuesta de mejora
* 979de84 [elarreglador | 2025-05-21]  🔥 Borrado: Eliminada pantalla no usada
* 47905e5 [David Moreno | 2025-05-20]  1a Revision del anexo
* 69b82dd [David Moreno | 2025-05-20]  Agregada diapositivas
* 9a3ab53 [David Moreno | 2025-05-20]  2a Revision finalizada
* d8ba6cd [David Moreno | 2025-05-20]  2a Revision finalizada
* add1411 [elarreglador | 2025-05-20]  2a Revision. Estado actual: 2.4.1 Ingresos
* a408849 [David Moreno | 2025-05-19]  📚 Documentación: Revision de la memoria
* 88f8e5a [elarreglador | 2025-05-19]  Revision de documentacion hasta 2.2.1.8 Tablas de alergenos
* cca3ac7 [elarreglador | 2025-05-18]  (tag: v0.5.9) 🎨 Mejora estética: Editados colores de texto
* afd7915 [elarreglador | 2025-05-18]  🐞 Bug corregido: partnerViewScreen muestra mail de vendedor
* d58f4a0 [elarreglador | 2025-05-18]  🐞 Bug corregido: clientViewScreen se muestra mail de cliente
* 958487d [elarreglador | 2025-05-18]  📚 Documentación: Corregido texto en info. screen
* 596edb2 [elarreglador | 2025-05-18]  📚 Documentación: Documentado git log
* 91d4018 [elarreglador | 2025-05-18]  (tag: v0.5.8) 💡 Nueva funcionalidad: Agregado dialogo logout a vendedor
* b564d3b [elarreglador | 2025-05-18]  ✨ Cambio menor: dialogo logout permite cancelar, salir y logout
* a0a023e [elarreglador | 2025-05-18]  💡 Nueva funcionalidad: Agregado dialogo logout
* 8971120 [elarreglador | 2025-05-18]  🎨 Mejora estética: Editados colores de texto en tarjetas orderListScreen
* f2970db [elarreglador | 2025-05-18]  🎨 Mejora estética: Editados colores dependientes del theme
* 0f5662e [elarreglador | 2025-05-18]  (tag: v0.5.7) 💡 Nueva funcionalidad: searchScreen tambien funciona sin activar GPS
* f459f92 [elarreglador | 2025-05-18]  (tag: v0.5.6) 💡 Nueva funcionalidad: Muestra fecha y hora en ordersListScreen
* dcb9b1e [elarreglador | 2025-05-18]  (tag: v0.5.5) 💡 Nueva funcionalidad: Muestra fecha y hora en myOrdersListScreen
* ebdf77e [elarreglador | 2025-05-18]  🎨 Mejora estética: Editado darkTheme para mejor estetica
* 3b61f44 [elarreglador | 2025-05-17]  (tag: v0.5.4) 🎨 Mejora estética: loading de perfil vendedor y cliente muestran imagen de fondo que cambia con el theme
* 8da75f2 [elarreglador | 2025-05-17]  🎨 Mejora estética: Editado darkTheme para mejor estetica
* 6b295ad [elarreglador | 2025-05-17]  🎨 Mejora estética: todos los listados de productos de la app muestran imagen de fondo que cambia con el theme
* b84cc95 [elarreglador | 2025-05-17]  🎨 Mejora estética: orderListScreen muestra imagen de fondo que cambia con el theme
* 26557f5 [elarreglador | 2025-05-17]  📐 Formato y limpieza del código: Comentarios y reubicacion de codigo
* e5039d9 [elarreglador | 2025-05-17]  (tag: v0.5.3) 💡 Nueva funcionalidad: Filtro de distancia
* ad2b6dd [elarreglador | 2025-05-17]  ⚙️ Nueva(s) función(es) GPS: getConfirmadoUsuario(), setConfirmadoUsuario(), getAccesoGPS(), setAccesoGPS(), getFakeLocation()
* a2e9475 [elarreglador | 2025-05-17]  📐 Formato y limpieza del código: Comentarios y reubicacion de codigo
* 014c19c [elarreglador | 2025-05-16]  (tag: v0.5.2) 💡 Nueva funcionalidad: SearchScreen muestra distancia hasta el vendedor
* 5498aa1 [elarreglador | 2025-05-16]  ✨ Cambio menor: Muestra distancia falsa en searchScreen
* 9884459 [elarreglador | 2025-05-16]  ⚙️ Nueva(s) función(es): GPS.distancePythagoras() calcula distancias a partir de posiciones GPS
* 94dffe8 [elarreglador | 2025-05-16]  ✨ Cambio menor: Boton guardar en topBar de editPartnerScreen
* 788f2a0 [elarreglador | 2025-05-16]  💡 Nueva funcionalidad: editPartnerScreen permite geolocalizacion
* b721ca6 [elarreglador | 2025-05-16]  ✨ Cambio menor: Obtenemos la posicion gps a costa de no precargar esa info. Pendiente de corregir
* 68096f2 [elarreglador | 2025-05-16]  ⚙️ Nueva(s) función(es): GPS.getCurrentLocation()
* a72dc61 [elarreglador | 2025-05-16]  ✨ Cambio menor: Boton de geolocalizacion en editPartnerScreen
* c9e2b37 [elarreglador | 2025-05-16]  🐞 Bug corregido: al mostrar el vendedor en el mapa se le ubica segun su direccion, provincia y ciudad en lugar de por el CP
* 420b262 [elarreglador | 2025-05-16]  📜 Nueva(s) clase(s): creado gps.dart con info sobre trigonometria basica
* b600299 [elarreglador | 2025-05-16]  (tag: v0.5.1) 💡 Nueva funcionalidad: Se muestran datos del vendedor al pulsar sobre su nombre en searchScreen
* fbf391c [elarreglador | 2025-05-16]  🟠 Postman export: Nuevo endpoint /panpaceli/listadoProductos devuelve tambien info del vendedor
* 1e10998 [elarreglador | 2025-05-16]  🔴 Node-red export: Nuevo endpoint /panpaceli/listadoProductos devuelve tambien info del vendedor
* 6eaa202 [elarreglador | 2025-05-16]  🔗 Nuevo(s) API REST endpoint(s): navegacion de nombre vendedor en searchScreen a partnerViewScreen
* c01f26b [elarreglador | 2025-05-15]  (tag: v0.5.0) 📐 Formato y limpieza del código: comentarios y ordenado de funciones
* 2420874 [elarreglador | 2025-05-15]  🐞 Bug corregido: searchScreen no queda con roturlo Cargando... en topBar
* cb456e5 [elarreglador | 2025-05-15]  💡 Nueva funcionalidad: myProductListScreen admite recarga de productos
* 46d3873 [elarreglador | 2025-05-15]  💡 Nueva funcionalidad: productFormScreen guarda cambios en productos
* 992bdec [elarreglador | 2025-05-15]  🟠 Postman export: endpoint /panpaceli/updateProducto funcional
* 2b7b976 [elarreglador | 2025-05-15]  🔴 Node red: endpoint /panpaceli/updateProducto funcional
* 2d6d287 [elarreglador | 2025-05-15]  📐 Formato y limpieza del código: Comentado y tabulado
* 98a8e29 [elarreglador | 2025-05-15]  💡 Nueva funcionalidad: productFormScreen carga productos para su edicion
* 55d0ad4 [elarreglador | 2025-05-15]  📅 Creado script para visualizar un calendario de commits
* 5eef8cb [elarreglador | 2025-05-15]  (⎇) Finalizado merge hotFix/estadoPedido
* 90778e5 [elarreglador | 2025-05-15]  (⎇) Previo a merge de hotFix/estadoPedido
* ed4d4e9 [elarreglador | 2025-05-15]  🔴 Node red: endpoint /panpaceli/pedidoSetState corregido y simplificado
* 64fe895 [elarreglador | 2025-05-15]  ✨ Cambio menor: Muestra nombre de cliente en searchScreen
* c0d1556 [elarreglador | 2025-05-15]  (⎇) Inicio hotFix/estadoPedido
* 5e1ea7f [elarreglador | 2025-05-15]  (⎇) Previo hotFix/estadoPedido
* ad477c8 [elarreglador | 2025-05-14]  Carga parcial de datos de producto en productFormScreen
* 920dc68 [elarreglador | 2025-05-14]  Navegacion de myProductsListScrenn a productFormScreen transporta el producto, pendiente importar producto a los campos de texto
* 24e15b8 [elarreglador | 2025-05-14]  🎨 Mejora estética: Nombre comercial en topBar de vendedor en myOrdersListScreen
* a27169a [elarreglador | 2025-05-14]  🎨 Mejora estética: myProductListScreen muestra descripcion de producto en un contenedor
* b388185 [elarreglador | 2025-05-14]  ✨ Cambio menor: Corregido texto de informacion
* f17f971 [elarreglador | 2025-05-14]  💡 Nueva funcionalidad: myProductListScreen permite eliminar productos desactivados
* 634ee01 [elarreglador | 2025-05-14]  🟠 Postman export: endpoint /panpaceli/delProducto funcional
* 208d83a [elarreglador | 2025-05-14]  🔴 Node red: endpoint /panpaceli/delProducto funcional
* 0ade3b9 [elarreglador | 2025-05-14]  💡 Nueva funcionalidad: se puede acceder al perfil del cliente desde cada pedido en myOrderListScreen
* 10cdcdb [elarreglador | 2025-05-14]  🎨 Mejora estética: clientViewScreen muestra un esqueleto de ejemplo con datos fake
* 8c1896c [elarreglador | 2025-05-14]  🟠 Postman export: endpoint /panpaceli/getExplicitValue funcional
* 366b333 [elarreglador | 2025-05-14]  🔴 Node red: endpoint /panpaceli/getExplicitValue funcional
* 1dacfc0 [elarreglador | 2025-05-14]  🔗 Navegación a pantallas:	Navega de nombre usuario en cada pedido de myOrderListScreen a clientViewScreen
* 11485a4 [elarreglador | 2025-05-14]  💡 Nueva funcionalidad: Vendedor puede activar y desactivar sus productos
* 5e9cbb8 [elarreglador | 2025-05-13]  🔴 Node red: endpoint /panpaceli/setProductoActivo funcional
* 88cce69 [elarreglador | 2025-05-13]  📱 pantalla/vista/pagina: Agregado a myProductsListScreen boton que activa y desactiva el producto
* b5a65ef [elarreglador | 2025-05-13]  🎨 Mejora estética: myOrderListScreen separa la primera tarjeta de la barra superior
* 58df0d8 [elarreglador | 2025-05-13]  ✨ Cambio menor: dialogo para confirmar cambio de estado en myOrdersListScreen
* b8755d4 [elarreglador | 2025-05-13]  🎨 Mejora estética: los datos quedan ordenados en la tarjeta
* f4174d1 [elarreglador | 2025-05-13]  💡 Nueva funcionalidad: myOrderListScreen muestra nombre y telefono del cliente, tambien permite llamar
* ca7153c [elarreglador | 2025-05-13]  myOrdersListScreen permite cambiar el estado de los pedidos
* 5166f69 [elarreglador | 2025-05-13]  🟠 Postman export: endpoint /panpaceli/pedidoSetState funcional
* 7037626 [elarreglador | 2025-05-13]  🔴 Node red: endpoint /panpaceli/pedidoSetState funcional
* c3fed30 [elarreglador | 2025-05-13]  ✨ Cambio menor:	myOrderListScreen muestra el nombre del cliente
* c02ba29 [elarreglador | 2025-05-13]  🎨 Mejora estética: Nuevo theme y mejora estetica en navbar de vendedor y cliente
* 035a019 [elarreglador | 2025-05-13]  💡 Nueva funcionalidad: filtro de myOrderListScreen muestra/oculta pedidos cancelados
* ecbd0da [elarreglador | 2025-05-13]  🎨 Mejora estética: myOrdersListScreen y ordersListScreen muestran pedidos cancelados en gris y codigo de colores para los estados
* 22e7f20 [elarreglador | 2025-05-12]  🔴 Node red: endpoint /panpaceli/misEncargosVendedor entrega info del cliente
* 22ba028 [elarreglador | 2025-05-12]  🚨 Corregidos warnings
* 1e01b8a [elarreglador | 2025-05-12]  🔥 Borrado: Eliminado boton de filtro de ultimos 10 dias
* b187321 [elarreglador | 2025-05-12]  ✨ Cambio menor: filtro para el vendedor segun estado de pedidos en myOrdersListScreen funciona mejor
* 09ce55d [elarreglador | 2025-05-12]  💡 Nueva funcionalidad: filtro para el vendedor segun estado de pedidos en myOrdersListScreen
* 1bfc5b6 [elarreglador | 2025-05-12]  📱 pantalla/vista/pagina: myOrderListScreen muestra los pedidos que tiene el vendedor
* 542198d [elarreglador | 2025-05-12]  🟠 Postman export: endpoint /panpaceli/misEncargosVendedor funcional
* 77d4cae [elarreglador | 2025-05-12]  🔴 Node red: endpoint /panpaceli/misEncargosVendedor funcional
* 8bce515 [elarreglador | 2025-05-12]  💡 Nueva funcionalidad: Boton logout en navbar de cliente y vendedor
* 94c1b62 [elarreglador | 2025-05-12]  📚 Documentación: Comentado codigo en navbar de cliente y vendedor
* 1203864 [elarreglador | 2025-05-12]  📱 pantalla/vista/pagina: myOrdersListScreen basica
* 6aa9d66 [elarreglador | 2025-05-12]  🐞 Bug corregido: no hay parpadeo al cargar datos del vendedor
* 72dd11f [elarreglador | 2025-05-12]  ✨ Cambio menor: Se muestra barra de carga en editClientScreen
* 8ffbba4 [elarreglador | 2025-05-12]  📚 Documentación: Agrego comentarios a editPartnerScreen
* 1d190ee [elarreglador | 2025-05-12]  💡 Nueva funcionalidad: al tirar hacia abajo recarga orderListScreen
* 52145dd [elarreglador | 2025-05-12]  💡 Nueva funcionalidad: Boton de recarga en orderListScreen
* 7831bf5 [elarreglador | 2025-05-12]  🐞 Bug corregido: Solucionado problema que impedia cancelar pedido por parte de cliente
* 0fe9eaf [elarreglador | 2025-05-12]   🎨 Mejora estética: Al leer el apartado legal o acerca se muestra barra de desplazamiento
* 6063793 [elarreglador | 2025-05-12]  📐 Formato y limpieza: Retirado codigo inutil y mejorada apariencia de la pantalla
* abf1e2e [elarreglador | 2025-05-12]  🟠 Postman export: endpoint /panpaceli/estadoPedidos
* 6cd59e2 [elarreglador | 2025-05-12]  🔴 Node red: endpoint /panpaceli/estadoPedido funcional
* 31e863b [elarreglador | 2025-05-12]  🅧  OrderScreen permite cancelar pedidos
* a18f940 [elarreglador | 2025-05-11]  🧿 orderListScreen muestra el estado del pedido
* ce10a6a [elarreglador | 2025-05-11]  📱 pantalla/vista/pagina: orderListScreen muestra pedios reales
* fd5e58f [elarreglador | 2025-05-11]  🔴 Node red: endpoint /panpaceli/misEncargosCliente agrega un objeto vendedor
* efad1f6 [elarreglador | 2025-05-11]  📱 pantalla/vista/pagina: order_list_screen simula tener pedidos
* 897057b [elarreglador | 2025-05-11]  🔴 Node red: endpoint /panpaceli/misEncargosCliente agrega un objeto producto
* 16db0e3 [elarreglador | 2025-05-11]  🟠 Postman export: endpoint /panpaceli/misEncargosCliente
* ae53685 [elarreglador | 2025-05-11]  🔴 Node red: endpoint /panpaceli/misEncargosCliente funcional
* ea6e58e [elarreglador | 2025-05-11]  (tag: v0.4.0) 💡 Nueva funcionalidad: El usuario ya puede encargar productos
* ee93c85 [elarreglador | 2025-05-11]  🟠 Postman export: endpoint /panpaceli/nuevoEncargo
* f22ec38 [elarreglador | 2025-05-11]  🔴 Node red: endpoint /panpaceli/nuevoEncargo funcional
* 1bc5272 [elarreglador | 2025-05-11]  Ventana de confirmacion de encargo
* b4acee9 [elarreglador | 2025-05-11]  📱 pantalla/vista/pagina: searchScreen muestra todos los productos
* 08c87a0 [elarreglador | 2025-05-11]  📐 Formato y limpieza del código: Macrocomenteario
* 58e3b29 [elarreglador | 2025-05-11]  🟠 Postman export: endpoint /panpaceli/listaProductos
* 7583529 [elarreglador | 2025-05-11]  🔴 Node red: endpoint /panpaceli/listaProductos funcional
* 9698c17 [elarreglador | 2025-05-10]  aviso en myProductsListScreen en caso de que el vendedor no tenga productos
* 2558c21 [elarreglador | 2025-05-10]  🐞 Bug corregido: Solucionado problema que impedia agregar datos de vendedor al crear usuario
* bb0801c [elarreglador | 2025-05-10]  🎨 Mejora estética: Agrego logo y espaciado en login y signup
* 9a58df8 [elarreglador | 2025-05-10]  🎨 Mejora estética: indicador de carga hasta que edit_partner_screen carga datos
* 15cd557 [elarreglador | 2025-05-10]  🔥 Borrado: Eliminado aboutScreen, tambien en go_router
* 2275d76 [elarreglador | 2025-05-10]  ⚖️  Pantalla Legal y Acerca funcionales
* 5ca7baf [elarreglador | 2025-05-10]  🔴🐞 Node-red export: endpoint /panpaceli/newProducto guarda los alergenos
* 2326b68 [elarreglador | 2025-05-10]  ✨ Cambio menor: obtiene listado de productos en myProductsListScreen
* 1046bbf [elarreglador | 2025-05-10]  ✨ Cambio menor: Simula ok listado de productos en myProductsListScreen
* 867e39e [elarreglador | 2025-05-10]  🔴🐞 Node-red export: endpoint /panpaceli/newProducto guarda los alergenos
* 8ba98af [elarreglador | 2025-05-10]  🔴 Node-red export: endpoint /panpaceli/misProductos devuelve info de alergenos
* 43c5d0e [elarreglador | 2025-05-10]  🟠 Postman export: endpoint /panpaceli/misProductos
* bec143c [elarreglador | 2025-05-10]  🔴 Node-red export: endpoint /panpaceli/misProductos
* b121848 [elarreglador | 2025-05-10]  (⎇) Finalizado merge feature/crearProductos
* 044ffd6 [elarreglador | 2025-05-10]  🐞 Bug corregido: guarda el nombre del producto y regresa a la lista de productos
* a31f198 [elarreglador | 2025-05-10]  💾 Almacenamiento:	ya se guardan nuevos productos en la BD
* 4ca0c8a [elarreglador | 2025-05-10]  🟠 Postman export: endpoint /panpaceli/newProducto
* 05f473c [elarreglador | 2025-05-10]  🔴 Node-red export: endpoint /panpaceli/newProducto
* d991a7d [elarreglador | 2025-05-09]  🟠 Postman export: Nuevo endpoint /panpaceli/newProducto
* c60c712 [elarreglador | 2025-05-09]  🔴 Node-red export: Nuevo endpoint /panpaceli/newProducto
* 43ebf86 [elarreglador | 2025-05-09]  🎨 diseño: finalizado product_form_screen a falta de logica
* a8fc394 [elarreglador | 2025-05-09]  🔗 Navegación a pantallas: MyProductsListScreen -> ProductFormScreen
* cffc0c4 [elarreglador | 2025-05-09]  (⎇) Inicio feature/crearProductos
* cb0ef44 [elarreglador | 2025-05-09]  (⎇) Previo feature/crearProductos
*   2efab50 [elarreglador | 2025-05-09]  Merge branch 'docs/newInfo'
|\  
| * b5c6282 [elarreglador | 2025-05-09]  (⎇) Previo a merge de docs/newInfo
| * 7ce8669 [David Moreno | 2025-05-08]  Agregada nueva informacion por parte de Asier
* | ef2f6df [elarreglador | 2025-05-09]  (⎇) Finalizado merge feature/splashScreen
* | 932572b [elarreglador | 2025-05-09]  🐞 Bug corregido: Navegacion de Splash screen para clientes
* | eddec92 [elarreglador | 2025-05-09]  📱 pantalla/vista/pagina: splash_screen funcional
* | c2d6086 [elarreglador | 2025-05-09]  🎨 Mejora estética: cambios en logo
* | e61a24f [elarreglador | 2025-05-09]  generado splashScreen minima y parte de la imagen que contendra
* | 698eb78 [elarreglador | 2025-05-09]  (⎇) Inicio feature/splashScreen
* | 9f1e713 [elarreglador | 2025-05-08]  ✨ Cambio menor: Reemplazado icono de editPartnerScreen en partnerNavBar
* | 72071c8 [elarreglador | 2025-05-08]  🔗 Navegación a pantallas: El vendedor puede navegar entre diferentes pantallas con un navBar
* | 140776e [elarreglador | 2025-05-07]  Navegacion de vendedor en curso
* | d8358b8 [elarreglador | 2025-05-06]  🔗 Navegación a pantallas: El cliente puede navegar entre diferentes pantallas con un navBar
|/  
* 2fc1a4a [elarreglador | 2025-05-06]  ✨ Cambio menor: Carga de datos en edit_partner_screen  y agregada mas resolucion a coordenadas en la BD (de 9,6 a 10,7)
* c19911f [elarreglador | 2025-05-05]  ✨ Cambio menor: Se recupera la info de cliente en edit_client_screen
* d3798ba [elarreglador | 2025-05-05]  ⚙️ Nueva(s) función(es): idEnTabla()
* 8c26f5c [elarreglador | 2025-05-05]  🟠 Postman export: /panpaceli/idEnTabla funcional
* 9b9d09f [elarreglador | 2025-05-05]  🔴 Node-red: endpoint /idEnTabla funcional
* 948cc52 [elarreglador | 2025-05-05]  🔴🐞 Node-red: endpoint newVendedor funcional y setValueInt entiende Strings vacios = 0
* 11e7306 [elarreglador | 2025-05-05]  💾 Almacenamiento: Guarda los datos de cliente y vendedor a traves de la API
* 9fcaa92 [elarreglador | 2025-05-05]  🐞 Bug corregido: Eliminado mail de pantalla edit_client_screen
* fc354aa [elarreglador | 2025-05-05]  🔴🐞 Node-red: corregido endpoint /setValueInt
* fdef37c [David Moreno | 2025-05-05]  Nodered: endpoint newVendedor
* f2a4737 [elarreglador | 2025-05-04]  ✨ Cambio menor: Actualiza datos de cliente
* ca12051 [elarreglador | 2025-05-04]  🔴 Node-red: Eliminado nodo /setValue en favor de /setValueString y /setValueInt
* 14dbd37 [elarreglador | 2025-05-04]  ⚙️ Nueva(s) función(es): reemplazado api_service.setValue() por .setValueString y .setValueInt
* 39b336b [elarreglador | 2025-05-04]  🔴 Node-red: Los token duran 7 dias
* 6da9191 [elarreglador | 2025-05-04]  🔴🐞 Node-red: Solucionado fallo en endpoint setValue
* 1d481b6 [elarreglador | 2025-05-04]  📐 Formato y limpieza del código: Eliminado auth_service.updateToken(), deshabilitado warning de print(), activado flutter_lints (buenas practicas)
* 58ea289 [elarreglador | 2025-05-03]  🔴 Node-red: Renombrados nodos debug importantes
* 9b44fb1 [elarreglador | 2025-05-03]  Memoria: corregido ssh para node-red
* ad1a69e [elarreglador | 2025-05-03]  🔥 Solucionado fallo de falta de memoria swap por corte electrico masivo
* 1b430af [elarreglador | 2025-05-03]  Anexo: memoria swap tras reinicio
* 25afcdd [elarreglador | 2025-05-03]  ⚙️ Nueva(s) función(es): api_service.newCliente
* 7bbd670 [elarreglador | 2025-05-03]  🟠 Postman export: /panpaceli/newCliente funcional
* 1c84496 [elarreglador | 2025-05-03]  🔴 Node-red: endpoint /panpaceli/newCliente funcional
* 5b50f9a [elarreglador | 2025-05-03]  ⚙️ función(es): retirado api_service.setVendedor() en favor de api_service.setData()
* 06330e4 [elarreglador | 2025-05-03]  ⚙️ Nueva(s) función(es): api_service.getValue() y api_service.getJson()
* c271d22 [elarreglador | 2025-05-03]  🐞 Bug corregido: Ya se pueden leer cajas de texto en tema oscuro
* 6900788 [elarreglador | 2025-04-30]  ⚙️ Nueva(s) función(es): api_service.getValue
* bc4e636 [elarreglador | 2025-04-28]  📷 Multimedia:Generado wallpaper
* d8670d5 [elarreglador | 2025-04-28]  ✨ Cambio menor: Modo loading
* 407f564 [elarreglador | 2025-04-28]  📱 pantalla/vista/pagina: Hay acceso a EditPartnerScreen
* 2954930 [elarreglador | 2025-04-28]  🎨 Aplicado theme (orange)
* b21eccc [elarreglador | 2025-04-28]  🎨 Aplicado theme
* b6bee72 [elarreglador | 2025-04-27]  📱 pantalla/vista/pagina: Hay acceso a EditClientScreen
* c92414f [elarreglador | 2025-04-26]  🛡️  Seguridad: securizado endpoint /panpaceli/setValue
* 29fff33 [elarreglador | 2025-04-26]  🔴 Node-red: endpoint /panpaceli/setValue funcional
* 0b9cd49 [elarreglador | 2025-04-26]  🛡️ Seguridad: Notificacion consulta maliciosa en endpoint /panpaceli/consulta
* b2cda73 [elarreglador | 2025-04-26]  🛡️  Aplicado filtro de consultas al endpoint /panpaceli/consulta
* 380c1bb [elarreglador | 2025-04-26]  🔴 Node-red: endpoint /panpaceli/consulta funcional
* 34060fc [elarreglador | 2025-04-26]  🛒 Se registra en BD si el usuario es vendedor o cliente
* e6260c5 [elarreglador | 2025-04-25]  🔴 Node-red: endpoint /panpaceli/setVendedor funcional
* e33877e [elarreglador | 2025-04-25]  🐞 Bug corregido: se contrasta en la renovacion del token que exista el usuario en la BD
* 2282109 [elarreglador | 2025-04-24]  ⛏ En curso: endpoint de setVendedor
* a01b49e [elarreglador | 2025-04-24]  📚 Documentación: Info visual del token en la memoria
* cd7f9a5 [elarreglador | 2025-04-24]  🐞 Bug corregido: el token ya no se autoreferencia
* 058d0b8 [elarreglador | 2025-04-24]  🔴 Node-red funcion verificar token
* 0ac2ee0 [elarreglador | 2025-04-24]  ⚠️  Evitamos warning: subimos ndkVersion a 27.0.12077973 en directorio android
* 18418cd [elarreglador | 2025-04-24]  📐 Formato y limpieza del código: Comentados varios prints de debug
* 65b1c77 [elarreglador | 2025-04-24]  🔑 Al abrir la app se renueva el token, 🔴 Node-red export , 🟠 Postman export
* a9244dd [elarreglador | 2025-04-23]  🔴 Node-red /panpaceli/updateToken, mejora estetica
* 2e2b04c [elarreglador | 2025-04-23]  🔴 Node-red /panpaceli/updateToken , 🟠 Postman: verifica updateToken
* ec23381 [elarreglador | 2025-04-23]  Anexo: agregado software de mirroring
* 2baea3a [elarreglador | 2025-04-23]  (tag: v0.3.0) Memoria: Ampliacion de los puntos 3 y 4
* 75cc58c [elarreglador | 2025-04-23]  🐞 Bug corregido: no se muestra momentaneamente la pantalla de login si hay un token valido
* 91995d8 [elarreglador | 2025-04-23]  🐞 Bug corregido: Ya se reconoce el token almacenado en el terminal al abrir la App
* 871eee4 [elarreglador | 2025-04-22]  🐞 Bug corregido: Node-red time_sec se reconoce
* a6fe10f [elarreglador | 2025-04-22]  🔴 Node-red, duracion de token (time_sec) como variable de entorno
* 39225a5 [elarreglador | 2025-04-22]  🔑 login y singUp finalizados, token disponible
* 589de78 [elarreglador | 2025-04-22]  🔑 Al abrir la app busca el token guardado
* 5b33931 [elarreglador | 2025-04-22]  📜 Nueva(s) clase(s): AuthHelper singleton para el token
* ef7e8c9 [elarreglador | 2025-04-22]  🔑 Al hacer login recibimos el token
* 6527959 [elarreglador | 2025-04-22]  🔴 Node-red envia token si mail+hash=ok, 🟠 Postman verifica funcionamiento de node-red
* a07c3c6 [elarreglador | 2025-04-22]  ⚙️ Generado archivo config.dart con ruta del server
* 078a150 [elarreglador | 2025-04-22]  🔒 La APP acepta SIEMPRE certificados autofirmados, node-red solo por https
* cc28ff2 [elarreglador | 2025-04-22]  🔒 La API funciona ahora bajo cifrado https
* 1a7cee4 [elarreglador | 2025-04-21]  📨 Verificar mail valido en signup antes de enviar
* e4acbfe [elarreglador | 2025-04-21]  🗝️ la App recibe el salt desde la API
* 0833e23 [elarreglador | 2025-04-21]  📤 Agrego exportaciones de node-red y postman
* 7c425e4 [elarreglador | 2025-04-21]  📚 Anexo: cambios en BD
* f1030dc [elarreglador | 2025-04-21]  ✨ Cambio menor: Sube el hash en lugar del passwd
* f213ac4 [elarreglador | 2025-04-20]  🎲 Se genera un salt aleatorio en el registro
* 3662cbb [elarreglador | 2025-04-20]  👤 Se pueden crear nuevos usuarios
* 92ff9ca [elarreglador | 2025-04-20]  🎀 Retirada cinta roja de debug en esquina sup. izq.
* 41950ae [elarreglador | 2025-04-20]  ✨ .gitignore:	ya no sube elementos no necesarios a github
* 508f069 [elarreglador | 2025-04-20]  😄 Ya tenemos icono en la app
* e23c036 [elarreglador | 2025-04-20]  ⤵️  Actualizacion de dependencias
* 8faaa22 [elarreglador | 2025-04-20]  🧭 go_router instalado y navegacion bidireccional login <-> singin
* e4b93a2 [elarreglador | 2025-04-20]  📂 Estructura de archivos: ajustado a convencion, directorios en minuscula
* 85204de [elarreglador | 2025-04-20]  📱 pantalla/vista/pagina: Pantalla de inicio -> loginScreen
* ea1049a [elarreglador | 2025-04-20]  🎉 Primera pantalla funcional
* e02b5d2 [elarreglador | 2025-04-20]  📂 Creacion de structura de archivos
* bd4889a [elarreglador | 2025-04-19]  🚀 Primera compilacion funcional
* e31cb49 [elarreglador | 2025-04-19]  🎉 Primer commit de la app!
* 12a1e05 [elarreglador | 2025-04-19]  Nuevo archivo: backup BD panpaceli
* 24a8652 [elarreglador | 2025-04-19]  Anexo: BD panpaceli creada y con backup
* e07d47d [elarreglador | 2025-04-19]  Anexo: node-red + MariaDB comunicados
* 60789ea [elarreglador | 2025-04-19]  Anexo: MariaDB y creacion memoria virtual
* 920a47c [elarreglador | 2025-04-18]  Anexo: Personalizacion de terminal remoto en servidor
* 314cc92 [elarreglador | 2025-04-18]  Anexo: instalacion node-red
* 271f8f5 [elarreglador | 2025-04-17]  Descripcion de instalacion de ubuntu, docker, y node-red
* 52a8682 [elarreglador | 2025-04-17]  📜 Nuevo documento: Anexo
* 1357c04 [David Moreno | 2025-04-15]  📚 Documentación: Ampliacion del readme
* 5bc3bec [elarreglador | 2025-04-15]  2.3.1 Fases
* bc84fa0 [elarreglador | 2025-04-15]  📑 Recursos: Creado archivo de claves y agregado a .gitignore
* 6636c6a [David Moreno | 2025-04-14]  Revision ortografica
* f1dc073 [David Moreno | 2025-04-14]  Agregado visual de las tablas de la BD
* 83ef2c1 [David Moreno | 2025-04-14]  Codigo sql para creacion BD
* 04bc560 [elarreglador | 2025-04-14]  Inicio revision tablas y creacion codigo sql de creacion
* 58e32ed [elarreglador | 2025-04-13]  2.2 Estructura de proyecto, 2.2.1 Base de datos, revision ortografica
* ca9614e [elarreglador | 2025-04-13]  Primer borrador de BD e inclusion en la memoria
* 29eea54 [elarreglador | 2025-04-13]  Avance en la BD, mejora de aspecto en 2.2.2 Arbol de pantallas, creado texto legal
* 40501f6 [elarreglador | 2025-04-12]  Otro avance en BD y agregado Node-Red a soft destacado
* ea0e46c [elarreglador | 2025-04-11]  Avance en la BD
* 10e97c3 [elarreglador | 2025-04-09]  Inicio plantilla alergenos
* e2f2d3c [elarreglador | 2025-04-08]  2.2.4 Flujo de trabajo de la app: avanzo en la descripcion y maquetacion parcial de la BD
* 1682fab [elarreglador | 2025-04-07]  Inicio 2.2.4 Flujo de trabajo de la app
* becb7e7 [elarreglador | 2025-04-07]  Agregada valoracion de vendedores y clientes
* 26585a4 [elarreglador | 2025-04-06]  Dedicatoria
* aaa7e3e [elarreglador | 2025-04-05]  Finalizado agradecimientos
* c116853 [elarreglador | 2025-04-05]  Finalizado apartado 2.3 Planificación de la ejecución
* 78fb95e [elarreglador | 2025-04-05]  Finalizado apartado 2.1 Recopilación de información
* fe2b870 [elarreglador | 2025-04-05]  (tag: v0.2.0) Finalizado apartado 2.5 Normativa aplicable
* 3b2ee46 [elarreglador | 2025-04-05]  Reglamento (UE) 2019/1150 sobre equidad y transparencia en plataformas digitales.
* b69be4c [elarreglador | 2025-04-05]  (tag: v0.1.0) Finalizada documentacion Ley 34/2002
* eda86ab [elarreglador | 2025-04-01]  Edicion parcial de la ley 34/2002 (LSSI-CE)
* b40260c [elarreglador | 2025-03-29]  Ley Orgánica 3/2018 que adapta el RGPD a la normativa española
* 8d523ca [elarreglador | 2025-03-29]  reorganizacion de documentacion legal
* 114c98e [elarreglador | 2025-03-29]  Reglamento General de Protección de Datos (RGPD)
* a1f58a9 [elarreglador | 2025-03-28]  Retirada Normativa > Ley 17/2011 por no aplicar a este proyecto
* 6f23948 [elarreglador | 2025-03-28]  Normmativa > Reglamento (UE) 828/2014
* 7a6a29c [elarreglador | 2025-03-28]  Ampliada identificacion de producto
* 4fe0fac [elarreglador | 2025-03-27]  Finalizada revision de Reglamento (UE) 1169/2011
* 5ff34d6 [David Moreno | 2025-03-26]  Descargado reglamento UE 1169/2011
* 345e0c5 [David Moreno | 2025-03-26]  borrado test.txt
* 2f7f04e [David Moreno | 2025-03-26]  Verificando conexion desde nuevo equipo
* afe9a45 [elarreglador | 2025-03-24]  Arbol de pantallas
* 7b886f2 [elarreglador | 2025-03-22]  Actualizada documentacion PFC
* 7391654 [elarreglador | 2025-03-14]  Agrego readme.md para github
* 067676b [elarreglador | 2025-03-14]  Ya tengo tutor del TFC 😊
* 3956ae5 [elarreglador | 2025-03-14]  finalizada descripcion tabla vendedores
* fb60873 [elarreglador | 2025-03-12]  descripcion de la tabla vendedores creada y pendiente de finalizar
* b4bef6c [elarreglador | 2025-03-12]  Tabla usuarios creada
* 7e8436b [elarreglador | 2025-03-10]  Normativa aplicable tanto a nivel nacional como europeo
* 955da4c [elarreglador | 2025-03-07]  Agregados algunos gastos a la tabla en 2.4.2 Gastos
* 517de3c [elarreglador | 2025-03-07]  Finalizada descripcion de cada pantalla
* d69da14 [elarreglador | 2025-03-06]  Arbol de pantallas y descripcion de pantallas
* 99ca3a2 [elarreglador | 2025-03-06]  Inicio arbol de pantallas
* 2301c59 [elarreglador | 2025-03-05]  Agrego gastos e ingresos de forma parcial y la descripcion del proyecto
* 3cdab86 [elarreglador | 2025-03-03]  📐 Formato del documento: Fases segun instrucciones.
* 40e9b2b [elarreglador | 2025-03-03]  📐 Formato del documento: Ajustes segun instrucciones (parcial)
* 9510d6d [elarreglador | 2025-03-03]  🏗️ Arquitectura: Cambio de directorios y agregado recurso de tipografia
* 31cb15f [elarreglador | 2025-03-03]  🔤 Cambio de nombre: Estandarizado del nombre de la memoria
* f442c7d [elarreglador | 2025-02-28]  🎨 Creada paleta de colores
* d4fbce1 [elarreglador | 2025-02-28]  📷 Multimedia: Agregadas imagenes logotipo y cabecera de la memoria
* c5eeaac [elarreglador | 2025-02-28]  📜 Creado archivo de la memoria
* 30e6166 [elarreglador | 2025-02-28]  🔥 Eliminando Entregado del control de versiones
* 4751df4 [elarreglador | 2025-02-28]  📚 Documentacion: Agregados preparativos
* 2e28fb0 [elarreglador | 2025-02-28]  🎉 Primer commit!
```

# Versiones publicadas

 v0.5.10 🔖 - solucion bug activac. GPS y guardado alergenos

 v0.5.9 🔖 - Corregidos bugs y agregada documentacion

 v0.5.8 🔖 - Dialogo de logout y mejoras esteticas

 v0.5.7 🔖 - Permite busquedas de producto sin activar GPS

 v0.5.6 🔖 - Muestra fecha y hora del pedido al cliente

 v0.5.5 🔖 - Muestra fecha y hora del pedido al vendedor

 v0.5.4 🔖 - Mejora estetica: darkTheme e imagen de fondo

 v0.5.3 🔖 - Disponible filtro de distancia a vendedor

 v0.5.2 🔖 - Acceso a GPS y calculo de distancia trigonometrica client…

 v0.5.1 🔖 - Cliente tiene acceso a ficha de vendedor

Panpaceli: [Descarga de versiones disponibles](https://github.com/elarreglador/TFC-Panpaceli/tree/main/Historial%20APK).

