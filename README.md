# Usar codigo de Objective-c en swift

Primero se debe crear el archivo Cabecera (Bridging-Header.h) donde se incluiran las librerias y clases de objective-c 

# Localizar el BridgingHeader en xcode

Ir al proyecto > Build Settings

En el buscador buscar: Objective-c Bridging Header 

Le pasamos como value: Nombre del proyecto/Bridging-Header.h (Osea el nombre de la cabecera)

// Esto es todo si las clases estan en la carpeta raiz.

# Si las clases estan como Pods

Ahi mismo buscamos: User Header Search Paths

Y como parametro le pasamos: Pods/**

# En el target de pruebas tambien se debe agregar para evitar errores con la cabecera

<blockquote class="imgur-embed-pub" lang="en" data-id="a/SRUnkjk"><a href="//imgur.com/SRUnkjk"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Listo !!
