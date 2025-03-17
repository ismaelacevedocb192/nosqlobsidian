#### Crear una Nueva Base de Datos

1. [[Conectar a Compass]].
2. **Haz clic en el botón "Create Database"** que aparece en la parte superior de la interfaz.
3. **Ingresa los detalles de la base de datos**:
    - En el campo "Database Name", escribe un nombre para tu base de datos (ejemplo: `miTiendaOnline`).
    - En el campo "Collection Name", escribe el nombre de tu primera colección (ejemplo: `productos`).
4. **Haz clic en "Create Database"** para confirmar. MongoDB creará tanto la base de datos como la primera colección.

#### Crear una Nueva Colección en tu Base de Datos

1. **Selecciona tu base de datos** recién creada en el panel izquierdo (ejemplo: `miTiendaOnline`).
2. **Haz clic en el botón "Create Collection"** que aparece en la parte superior.
3. **Ingresa el nombre de tu nueva colección** en el campo correspondiente (ejemplo: `clientes`).
4. **Haz clic en "Create Collection"** para confirmar.

#### Insertar Datos en una Colección

1. **Selecciona la colección** donde deseas insertar datos (ejemplo: `productos`).
2. **Haz clic en el botón "Add Data"** y selecciona "Insert Document".
3. **Ingresa los datos en formato JSON** en el editor que aparece. MongoDB Compass proporciona un editor visual que te permite añadir datos de forma estructurada.
4. **Haz clic en "Insert"** para guardar el documento en la colección.

#### Ejemplo Práctico: Creación de una Tienda Online

**Paso 1: Crear la Base de Datos y Colecciones**

1. Crear base de datos `tiendaOnline` con colección inicial `productos`.
2. Añadir colecciones adicionales: `clientes` y `pedidos`.

**Paso 2: Añadir Productos a la Colección "productos"**Selecciona la colección `productos` y añade documentos como el siguiente:


```json
{
  "nombre": "Laptop Ultradelgada",
  "marca": "TechPro",
  "precio": 1299.99,
  "stock": 15,
  "categorias": ["electrónica", "computadoras"],
  "especificaciones": {
    "procesador": "Intel Core i7",
    "ram": "16GB",
    "almacenamiento": "512GB SSD",
    "pantalla": "15.6 pulgadas"
  },
  "disponible": true
}
```

Añade otro producto:


```json
{
  "nombre": "Smartphone Galaxy X10",
  "marca": "Samsung",
  "precio": 899.99,
  "stock": 25,
  "categorias": ["electrónica", "móviles"],
  "especificaciones": {
    "procesador": "Snapdragon 8 Gen 2",
    "ram": "12GB",
    "almacenamiento": "256GB",
    "pantalla": "6.7 pulgadas AMOLED"
  },
  "disponible": true
}
```

**Paso 3: Añadir Clientes a la Colección "clientes"**Selecciona la colección `clientes` y añade:


```json
{
  "nombre": "Ana García",
  "email": "ana.garcia@ejemplo.com",
  "telefono": "555-123-4567",
  "direccion": {
    "calle": "Av. Principal 123",
    "ciudad": "Madrid",
    "codigoPostal": "28001",
    "pais": "España"
  },
  "fechaRegistro": "2023-05-15",
  "ultimaCompra": "2023-09-20"
}
```

**Paso 4: Añadir Pedidos a la Colección "pedidos"**Selecciona la colección `pedidos` y añade:


```json
{
  "numeroPedido": "ORD-2023-001",
  "clienteId": "ObjectId('paste-client-id-here')",
  "productos": [
    {
      "productoId": "ObjectId('paste-product-id-here')",
      "nombre": "Laptop Ultradelgada",
      "cantidad": 1,
      "precioUnitario": 1299.99
    }
  ],
  "total": 1299.99,
  "estado": "completado",
  "fechaPedido": "2023-09-20",
  "metodoPago": "tarjeta"
}
```

#### Consultar los Datos

Una vez que hayas insertado tus documentos, puedes explorarlos:

1. **Selecciona tu colección** en el panel izquierdo.
2. **Los documentos aparecerán** en el panel principal.
3. **Utiliza la barra de filtros** en la parte superior para buscar documentos específicos. Por ejemplo, para encontrar productos con precio menor a 1000:
    ```javascript
    {precio: {$lt: 1000}}
    ```

Con estos ejemplos, ya tienes una base de datos funcional para una tienda online con colecciones para productos, clientes y pedidos, todos conectados mediante referencias.