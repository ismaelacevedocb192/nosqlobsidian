#### Requisitos Previos

1. [[Crear Cuenta en MongoDB]] con un clúster creado.
2. **Tener instalado MongoDB Compass** en tu ordenador. Si aún no lo tienes, descárgalo desde el sitio oficial de MongoDB.

#### Obtener la Cadena de Conexión desde Atlas

1. **Inicia sesión en tu cuenta de MongoDB Atlas**.
2. **Accede a tu clúster** haciendo clic en el botón "Connect" del clúster que deseas conectar.
3. **Selecciona "Connect with MongoDB Compass"** en las opciones de conexión que se muestran.
4. **En la siguiente pantalla, selecciona "I have MongoDB Compass"** ya que lo tenemos instalado y vamos a usarlo .
5. **Selecciona la versión de Compass** que estás utilizando. Si tienes una versión reciente, selecciona "1.12 or later".
6. **Copia la cadena de conexión** que te proporciona Atlas. Esta cadena contiene toda la información necesaria para conectarte a tu base de datos (host, puerto, etc.).

#### Conectar desde MongoDB Compass

1. **Abre MongoDB Compass** en tu ordenador.
2. **En la pantalla de inicio de Compass, pega la cadena de conexión** que copiaste de MongoDB Atlas en el campo correspondiente.
3. **Reemplaza `<password>` en la cadena de conexión** con la contraseña del usuario de la base de datos que configuraste en Atlas .
4. **Haz clic en el botón "Connect"** para establecer la conexión con tu clúster de MongoDB Atlas .
5. **Espera a que se establezca la conexión**. Si todo está configurado correctamente, verás las bases de datos disponibles en tu clúster.

#### Solución de Problemas Comunes

- Si no puedes conectarte, **verifica que la dirección IP desde la que te conectas esté permitida** en la configuración de Network Access de Atlas.
- **Asegúrate de que las credenciales (usuario y contraseña) sean correctas** y que el usuario tenga los permisos necesarios para acceder a la base de datos Si sigues teniendo problemas, es posible que sea un problema temporal de red o que necesites revisar tu conexión a internet vez conectado, podrás explorar e interactuar con tus datos utilizando la interfaz gráfica de MongoDB Compass, que te permite consultar, modificar y eliminar datos, todo desde una sola interfaz.