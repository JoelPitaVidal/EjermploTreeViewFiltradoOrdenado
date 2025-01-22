# Ejemplo con Treeview de filtrado y ordenado

Este proyecto es un ejemplo de cómo utilizar un `Gtk.TreeView` con filtrado y ordenado en una aplicación de GTK+ en Python. La aplicación muestra una lista de usuarios obtenida de una base de datos SQLite.

## Descripción del código

El código principal se encuentra en el archivo `EjermploTreeViewFiltradoOrdenado.py`. A continuación se describe el funcionamiento del código:

1. **Configuración de la ventana principal**:
   - Se establece el título de la ventana y su tamaño.
   - Se desactiva la opción de redimensionar la ventana.

2. **Creación de la caja vertical**:
   - Se crea una caja vertical (`Gtk.Box`) para organizar los widgets dentro de la ventana.

3. **Conexión a la base de datos**:
   - Se establece una conexión a la base de datos `usuarios.db`.

4. **Modelo de datos**:
   - Se crea un modelo de datos (`Gtk.ListStore`) para almacenar la información de los usuarios.
   - Se realiza una consulta a la base de datos para obtener los datos de los usuarios y se añaden al modelo.

5. **Creación del TreeView**:
   - Se crea un `Gtk.TreeView` y se configura para utilizar el modelo de datos creado anteriormente.
   - Se configuran las columnas del `TreeView` para mostrar la información de los usuarios (DNI, Nombre, Edad, Género, Fallecido).

6. **Columnas adicionales**:
   - Se añade una columna de progreso para mostrar la edad de los usuarios.
   - Se añade una columna con un combo box para seleccionar el género de los usuarios.
   - Se añade una columna con un toggle button para indicar si el usuario está fallecido.

7. **Añadir el TreeView a la caja vertical**:
   - Se añade el `TreeView` a la caja vertical.

8. **Mostrar la ventana**:
   - Se añade la caja vertical a la ventana principal y se muestran todos los widgets.

## Requisitos

- Python 3
- GTK+ 3
- SQLite

## Ejecución

Para ejecutar la aplicación, simplemente ejecuta el archivo `EjermploTreeViewFiltradoOrdenado.py` con Python:

```bash
python EjermploTreeViewFiltradoOrdenado.py
