# UD1 A1. Lenguajes de marcas

## 1- Indica que es un lenguaje de marcas
Un lenguaje de marcas es un conjunto de reglas y convenciones utilizadas para definir la estructura y organización de un contenido mediante "etiquetas" o "marcas". Estas marcas no suelen ser visibles para el usuario final, pero proporcionan instrucciones sobre cómo debe ser interpretado o presentado el contenido. Los lenguajes de marcas son fundamentales para la estructuración de datos y contenidos, especialmente en la web.
## 2- Características generales de los lenguajes de marcas
Uso de etiquetas: Los lenguajes de marcas utilizan etiquetas para delimitar y organizar el contenido. Estas etiquetas pueden ser de apertura y cierre (como en HTML) o estar presentes solo en la apertura.
Jerarquía y estructura: Las etiquetas pueden estar anidadas unas dentro de otras, lo que crea una estructura jerárquica que facilita la interpretación del contenido.
Legibilidad: Están diseñados para ser legibles por humanos y por máquinas, lo que facilita su creación, modificación y procesado.
Independencia del contenido: Permiten separar el contenido de su presentación o forma de ser procesado. Por ejemplo, en HTML el contenido está estructurado, pero su presentación puede definirse en CSS.
Portabilidad: Al ser esencialmente texto plano, pueden ser leídos y procesados por diversas aplicaciones y sistemas operativos.
Extensibilidad: Pueden ser extendidos mediante la creación de nuevas etiquetas o atributos, según las necesidades del usuario o aplicación.
## 3- Clasifica los lenguajes de marcas e identifica los más relevantes
Lenguajes de marcas de presentación:
Son utilizados principalmente para describir cómo debe ser presentado el contenido.
Ejemplos: HTML (HyperText Markup Language), XML.
Lenguajes de marcas de datos:
Se usan para describir datos estructurados.
Ejemplos: XML (eXtensible Markup Language), JSON (aunque técnicamente no es un lenguaje de marcas, cumple una función similar en la estructura de datos), YAML.
Lenguajes de marcas específicos para aplicaciones:
Diseñados para un propósito específico o en un contexto particular.
Ejemplos: iCalendar, vCard, KML (Keyhole Markup Language), RSS (Really Simple Syndication).
## 4- Indica los distintos ámbitos de aplicación de los lenguajes de marcas
Web: Lenguajes como HTML y XML son fundamentales para la creación y estructuración de sitios web.
Intercambio de datos: Lenguajes como XML, JSON o YAML permiten el intercambio de datos entre diferentes sistemas y aplicaciones.
Geolocalización: KML se usa para representar datos geoespaciales, compatible con aplicaciones como Google Earth.
Gestión de información personal: iCalendar y vCard se utilizan para gestionar y compartir información de calendarios y contactos.
Distribución de contenido: RSS facilita la distribución de noticias y actualizaciones de contenido en sitios web o blogs.
## 5- Inserta un trozo de código de cada uno de los lenguajes de marcas que se indican a continuación. Añadir a cada trozo de código un pequeño resumen sobre su estructura y la aplicación asociada que los procesa

### 1. HTML (HyperText Markup Language)

``````
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Página de ejemplo</title>
</head>
<body>
    <h1>Hola, Mundo</h1>
    <p>Bienvenido a mi página web.</p>
</body>
</html>
``````
Estructura:
HTML utiliza etiquetas como <-html->, <-head->, <-body->, etc., para organizar el contenido de una página web. Las etiquetas de apertura <-h1->, <-p->, etc., son acompañadas por etiquetas de cierre correspondientes, como <-/h1->, <-/p->. Es procesado por navegadores web (Chrome, Firefox, etc.) para mostrar páginas web.

### 2. iCalendar (Formato de calendario)
   
``````
BEGIN:VCALENDAR
VERSION:2.0
PRODID:-//Mi Organización//Mi Calendario 1.0//ES
BEGIN:VEVENT
UID:1234567890@miempresa.com
DTSTAMP:20231010T120000Z
DTSTART:20231011T090000Z
DTEND:20231011T100000Z
SUMMARY:Reunión con el equipo
END:VEVENT
END:VCALENDAR
``````

Estructura:
iCalendar utiliza bloques de etiquetas como BEGIN:VEVENT y END:VEVENT para representar eventos. Cada evento contiene propiedades como la fecha de inicio (DTSTART), final (DTEND), y un resumen (SUMMARY). Es procesado por aplicaciones de calendario como Google Calendar, Outlook, entre otros.

### 3. vCard (Formato de tarjeta de contacto)
``````
BEGIN:VCARD
VERSION:3.0
FN:Juan Pérez
ORG:Mi Empresa
TEL;TYPE=WORK,VOICE:+34 123 456 789
EMAIL:juan.perez@miempresa.com
END:VCARD
``````

Estructura:
vCard utiliza etiquetas como FN (nombre completo), ORG (organización), TEL (teléfono) y EMAIL para describir la información de contacto de una persona. Es procesado por aplicaciones de gestión de contactos como Microsoft Outlook, Apple Contacts, y aplicaciones móviles.

### 4. KML (Keyhole Markup Language)

`````
<?xml version="1.0" encoding="UTF-8"?>
<kml xmlns="http://www.opengis.net/kml/2.2">
  <Placemark>
    <name>Mi ubicación</name>
    <Point>
      <coordinates>-122.0822035425683,37.42228990140251,0</coordinates>
    </Point>
  </Placemark>
</kml>
``````

Estructura:
KML es un lenguaje basado en XML usado para representar información geográfica. En este ejemplo, se define una ubicación con las etiquetas <Placemark> y <coordinates>. Este código puede ser procesado por aplicaciones como Google Earth para visualizar ubicaciones en mapas.

### 5. RSS (Really Simple Syndication)

``````
<rss version="2.0">
  <channel>
    <title>Mi Blog</title>
    <link>https://www.miblog.com</link>
    <description>Actualizaciones del blog de tecnología</description>
    <item>
      <title>Última entrada del blog</title>
      <link>https://www.miblog.com/entrada-reciente</link>
      <description>Resumen de la última entrada del blog.</description>
    </item>
  </channel>
</rss>
``````

Estructura:
RSS utiliza etiquetas como <channel> para agrupar el contenido del feed y <item> para cada entrada o actualización. Cada entrada contiene un título, un enlace y una descripción. Es procesado por lectores de RSS como Feedly o aplicaciones similares para distribuir contenido en formato de suscripción.
