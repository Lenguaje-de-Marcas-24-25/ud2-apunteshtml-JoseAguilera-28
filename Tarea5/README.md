# Preguntas sobre XML

## 1. Indica las características propias del lenguaje XML

- **Lenguaje de marcado**: XML (eXtensible Markup Language) es un lenguaje utilizado para almacenar y transportar datos de forma estructurada.
- **Personalizable**: Permite definir etiquetas propias, lo que lo hace flexible para representar diferentes tipos de datos.
- **Auto-descriptivo**: Los datos están acompañados por sus etiquetas, lo que facilita la comprensión de la estructura del contenido.
- **Independiente de la plataforma**: Los documentos XML pueden ser procesados en cualquier sistema operativo y lenguaje de programación.
- **Rigidez sintáctica**: La sintaxis es estricta, por lo que un documento XML debe estar bien formado para ser interpretado correctamente.
- **Facilita la interoperabilidad**: Es ampliamente utilizado para el intercambio de información entre diferentes sistemas y aplicaciones.

## 2. Identifica la estructura de un documento XML y sus reglas sintácticas

Un documento XML tiene una estructura general que sigue las siguientes reglas:

```
xml
<?xml version="1.0" encoding="UTF-8"?>
<raiz>
    <elemento>
        <subelemento>Aquí van los datos</subelemento>
    </elemento>
</raiz>

```

## 3. En XML, ¿qué es un nodo raíz?

El nodo raíz es el elemento principal que contiene todos los demás elementos de un documento XML. Es el primer elemento del documento y sirve como contenedor para todos los demás. Solo puede haber un nodo raíz en un documento XML.

## 4. Indica qué es un elemento vacío. Ejemplos

Un elemento vacío en XML es un elemento que no tiene contenido ni elementos hijos. Se puede representar de dos maneras:

```
-<elemento></elemento>
o
-<elemento/>

Ejemplos:

-<imagen/>

-<br/>
```
## 5. ¿Qué sentido tiene crear documentos XML bien formados?

Crear un documento XML bien formado es esencial para garantizar que el documento sea procesado correctamente por un parser XML. Un documento bien formado cumple con todas las reglas sintácticas del lenguaje, lo que asegura la interoperabilidad entre diferentes aplicaciones y sistemas que utilicen XML. Si el documento no está bien formado, es probable que no sea aceptado o que cause errores en las aplicaciones.

## 6. ¿Qué es un espacio de nombres? Ventajas de uso

Un espacio de nombres en XML es una forma de evitar conflictos de nombres cuando se combinan documentos de diferentes fuentes que podrían tener etiquetas con los mismos nombres. Se define mediante un prefijo asociado a una URL única.

Ventajas:

1. Evita conflictos de nombres: Ayuda a distinguir entre elementos que tienen el mismo nombre pero pertenecen a contextos diferentes.

2. Facilita la combinación de documentos XML: Permite integrar datos de distintos esquemas XML sin colisiones de nombres.
   
3. Mejora la claridad: Especifica el origen o contexto de los elementos y atributos.

## 7. Entidades en XML. Crea un XML con las entidades vistas en clase

Las entidades en XML son representaciones de caracteres especiales que no pueden ser utilizados directamente en el contenido del documento.

[Enlace a entidades en XML](Entidades.xml)

## 8. Comentarios en XML. Muestra uno de los ejercicios anteriores con el enunciado dentro de un comentario

```
Los comentarios en XML se escriben con la sintaxis <!-- comentario -->. No son procesados por los parsers XML y sirven para añadir anotaciones al documento.


<?xml version="1.0" encoding="UTF-8"?>
<!-- Ejemplo de un documento XML de pedidos. --

     Este documento contiene información sobre varios pedidos. -->
     
<pedidos>
    <pedido cod="1">
        <fecha>24-10-2024</fecha>
        <pu>45.5</pu>
        <cantidad>2</cantidad>
        <descripcion>Botella de Vino</descripcion>
        <tipo>C</tipo>
    </pedido>
    <pedido cod="2">
        <fecha>24-10-2024</fecha>
        <pu>25</pu>
        <cantidad>1</cantidad>
        <descripcion>Menu Ejecutivo</descripcion>
        <tipo>A</tipo>
    </pedido>
</pedidos>
```