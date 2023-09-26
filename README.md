# README.md para Weather App

## Descripción

Este es un código para una aplicación de clima que utiliza la biblioteca `tkinter` para la interfaz gráfica de usuario, `geopy` para obtener la ubicación geográfica, `timezonefinder` para obtener la zona horaria, y la API de OpenWeatherMap para obtener los datos del clima.

## Requisitos

Para ejecutar este código, necesitarás las siguientes bibliotecas de Python:

- tkinter
- geopy
- timezonefinder
- datetime
- requests
- pytz

Además, necesitarás una clave API de OpenWeatherMap, que puedes obtener [aquí](https://home.openweathermap.org/users/sign_in).

## Cómo usar

1. Clona este repositorio en tu máquina local.
2. Instala las bibliotecas requeridas mencionadas anteriormente usando pip.
3. Abre el archivo en tu editor de código preferido.
4. Reemplaza 'youruseragent' y 'yourapikey' con tu User Agent y tu clave API de OpenWeatherMap respectivamente.
5. Ejecuta el script.

Una vez que el programa esté en ejecución, verás una interfaz gráfica de usuario donde puedes ingresar el nombre de una ciudad. Al presionar el botón de búsqueda, la aplicación mostrará la hora actual en esa ciudad junto con varios detalles del clima como la temperatura, la velocidad del viento, la humedad, la descripción del clima y la presión atmosférica.

## Funciones

El código consta de varias funciones y bloques de código:

- `getWeather()`: Esta función se activa cuando se presiona el botón de búsqueda. Obtiene los datos geográficos de la ciudad ingresada usando `geopy`, determina la zona horaria con `timezonefinder`, y luego hace una solicitud a la API de OpenWeatherMap para obtener los datos del clima. Los datos se muestran en la interfaz gráfica de usuario.

- Bloque `root = Tk()`: Este bloque configura la ventana principal de la aplicación.

- Bloque `textfield = tk.Entry(...)`: Este bloque crea un campo de entrada donde puedes escribir el nombre de una ciudad.

- Bloque `myimage_icon = Button(...)`: Este bloque crea el botón de búsqueda que activa la función `getWeather()` cuando se presiona.

- Bloques `Label(...)`: Estos bloques crean varias etiquetas que se utilizan para mostrar los datos del clima en la interfaz gráfica de usuario.

Por favor, ten en cuenta que este código requiere ciertos archivos de imagen (por ejemplo, 'Copy of search.png', 'Copy of search_icon.png', 'Copy of logo.png', 'Copy of box.png') para mostrar correctamente todos los elementos gráficos. Asegúrate de tener estos archivos en el mismo directorio que tu script.

## Contribuciones

Las contribuciones a este proyecto son bienvenidas. Si encuentras un error o tienes una sugerencia para mejorar el código, por favor abre un issue o un pull request.
