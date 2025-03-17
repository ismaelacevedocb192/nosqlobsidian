#### Paso 1: Crear la Base de Datos y Colección

1. Abre MongoDB Compass y conéctate a tu clúster.
2. Haz clic en "Create Database".
3. Nombra la base de datos como `futbolMexicano`.
4. Nombra la colección inicial como `jugadoresLigaMX`.
5. Haz clic en "Create Database".

#### Paso 2: Diseñar la Estructura de Documentos

Cada documento de jugador tendrá la siguiente estructura básica:

```json
{
  "nombre": "Nombre del Jugador",
  "apellidos": "Apellidos del Jugador",
  "equipo": "Nombre del Equipo",
  "numero": 10,
  "posicion": "Posición del Jugador",
  "nacionalidad": "País de origen",
  "edad": 25,
  "estatura": 180,
  "peso": 75
}
```

#### Paso 3: Insertar Datos de Ejemplo

Selecciona la colección `jugadoresLigaMX` y usa "Add Data" → "Insert Document" para añadir jugadores. Aquí tienes varios ejemplos que puedes insertar:


```json
{
  "nombre": "Guillermo",
  "apellidos": "Ochoa",
  "equipo": "Club América",
  "numero": 13,
  "posicion": "Portero",
  "nacionalidad": "México",
  "edad": 38,
  "estatura": 185,
  "peso": 78
}
```


```json
{
  "nombre": "André-Pierre",
  "apellidos": "Gignac",
  "equipo": "Tigres UANL",
  "numero": 10,
  "posicion": "Delantero",
  "nacionalidad": "Francia",
  "edad": 38,
  "estatura": 187,
  "peso": 82
}
```


```json
{
  "nombre": "Henry",
  "apellidos": "Martín",
  "equipo": "Club América",
  "numero": 21,
  "posicion": "Delantero",
  "nacionalidad": "México",
  "edad": 31,
  "estatura": 177,
  "peso": 73
}
```

```json
{
  "nombre": "Víctor",
  "apellidos": "Guzmán",
  "equipo": "Chivas de Guadalajara",
  "numero": 7,
  "posicion": "Mediocampista",
  "nacionalidad": "México",
  "edad": 28,
  "estatura": 176,
  "peso": 72
}
```


```json
{
  "nombre": "Germán",
  "apellidos": "Berterame",
  "equipo": "Monterrey",
  "numero": 9,
  "posicion": "Delantero",
  "nacionalidad": "Argentina",
  "edad": 25,
  "estatura": 183,
  "peso": 78
}
```


```json
{
  "nombre": "César",
  "apellidos": "Huerta",
  "equipo": "Pumas UNAM",
  "numero": 24,
  "posicion": "Extremo",
  "nacionalidad": "México",
  "edad": 23,
  "estatura": 173,
  "peso": 68
}
```


```json
{
  "nombre": "Carlos",
  "apellidos": "Acevedo",
  "equipo": "Santos Laguna",
  "numero": 1,
  "posicion": "Portero",
  "nacionalidad": "México",
  "edad": 27,
  "estatura": 185,
  "peso": 79
}
```


```json
{
  "nombre": "Julián",
  "apellidos": "Quiñones",
  "equipo": "Club América",
  "numero": 33,
  "posicion": "Delantero",
  "nacionalidad": "Colombia/México",
  "edad": 27,
  "estatura": 184,
  "peso": 76
}
```

#### Paso 4: Consultar los Datos

Una vez insertados los datos, puedes realizar consultas como:

1. **Buscar jugadores por equipo**:
    
    javascript
    
    ```javascript
    {equipo: "Club América"}
    ```
    
2. **Buscar jugadores por posición**:
    
    javascript
    
    ```javascript
    {posicion: "Delantero"}
    ```
    
3. **Buscar jugadores con un número específico**:
    
    javascript
    
    ```javascript
    {numero: 10}
    ```
    
4. **Buscar jugadores por nacionalidad**:
    
    javascript
    
    ```javascript
    {nacionalidad: "México"}
    ```
    

#### Paso 5: Expandir tu Set de Datos

Puedes continuar añadiendo más jugadores siguiendo la misma estructura. Para un conjunto de datos más completo, puedes incluir todos los equipos de la Liga MX y sus respectivos jugadores.Este es un set de datos básico que puedes expandir con más campos según tus necesidades, como:

- Fecha de nacimiento
- Fecha de incorporación al equipo
- Estadísticas de juego (goles, asistencias, etc.)
- Historial de equipos anteriores
- Valor de mercado

Recuerda que MongoDB es flexible, así que puedes modificar la estructura de los documentos según necesites.