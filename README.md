# **Internet Explorer** y **ES6** no son amigos :(

## Justificación
La intención del presente documento es mostrar desde un punto de vista pragmático y las desventajas de dar soporte a Internet Explorer 11 (para futuras referencias ie11)  la fecha.
Se añadirán links a fuentes de confianza donde se presentan mucho más a detalle los puntos que aquí menciono.

## ¿Qué es ECMAScript (ES)?
> Para muchos la palabra ECMA no resulta tan conocida. Se trata de un acrónimo de “European Computer Manufacturers Association (ECMA)”, una organización internacional basada en membresías de estándares para la comunicación y la información.
En el año de 1997 se crea un comité (TC39) en la ECMA para estandarizar JavaScript. A partir de entonces, los estándares de JavaScript se rigen como ECMAScript. No solo JavaScript se basa en el lenguaje ECMAScript, existen otros como JScript y ActionScript 3 que también lo hacen. Haciendo una analogía, diremos que ECMAScript es el lenguaje y JavaScript, JScript y ActionScript 3 son dialectos de este lenguaje, siendo JavaScript su dialecto más conocido y utilizado.

Fuente: [DevCode](https://devcode.la/blog/que-es-y-por-que-aprender-ecmascript/)

En resumen ECMA es el organismo que define las especificaciones de Javascript (js) a través los estándares y versiones de ECMAScript (es)

## ECMAScript Compatibilidad (pasado, presente y futuro)
Año | Versión | Soporte
--- | --- | ---
*2009* | [ECMAScript 5](https://en.wikipedia.org/wiki/ECMAScript#5th_Edition) | Totalmente soportado. Excepto por el modo “strict” en IE9
*2015* | [ECMAScript 6](https://en.wikipedia.org/wiki/ECMAScript#6th_Edition_-_ECMAScript_2015) | Parcialmente soportado en todos los navegadores modernos
*2016* | [ECMAScript 7](https://en.wikipedia.org/wiki/ECMAScript#7th_Edition_-_ECMAScript_2016) | Poco soportado en todos los navegadores

Un extracto pequeño de la página: [W3Schools](https://www.w3schools.com/js/js_versions.asp)

Gran parte del código js que se escribe actualmente entra dentro de las especificaciones de es5 sin embargo, la versión 6 cuanta con características que mejoran el lenguaje de manera significativa, algunas de las cuales se describen brevemente en el siguiente post: [ES6 vs ES5](https://medium.com/front-end-hacking/es6-vs-es5-9254f8390332)

Ahora, como se puede observar en la tabla anterior, la versión 6 fue publicada hace ya 2 años y aunque la columna de soporte dice: “Parcialmente soportado en todos los navegadores modernos” el porcentaje de soporte entre ie y otros navegadores es brutal.

[Aquí](https://kangax.github.io/compat-table/es6) se encuentra una tabla que muestra las diferentes características del lenguaje que son soportadas en los distintos navegadores. Si nos fijamos en la fila principal de la misma podremos encontrar el soporte en porcentaje con el que las distintas versiones de cada navegador cuentan. En donde podemos observar que figuran (las últimas versiones):

-	Microsoft Edge 15 -> 93%
-	Mozilla Firefox 55 -> 97%
-	Google Chrome 60 -> 97%
-	Opera 47 -> 97%
-	Safari 10 -> 99%
-	Mobile IOS 11 -> 99%
-	Internet Explorer 11%

Como se puede observar el soporte no es completo, pero queda claramente demostrado que la diferencia en compatibilidad es abismal.

## Internet Explorer (en la actualidad)
La más reciente versión del navegador es la 11. La cual fue lanzada hace más de 3 años (el 17 de Octubre de 2013) Fuente: 
[Wikipedia](https://en.wikipedia.org/wiki/Internet_Explorer_11)

Y se especula que no habrá una nueva versión del navegador en el futuro.

Otro punto bastante importante a considerar es el ranking de uso de los navegadores. El cual se puede consultar en la siguiente dirección: [W3Counter](https://www.w3counter.com/globalstats.php) 

Como se puede apreciar en la lista, la cantidad a la fecha de personas que utilizan ie11 es de menos del 4% de la población mundial.

## La apuesta de Microsoft
En el siguiente foro: [teamtreehouse](https://teamtreehouse.com/community/ie11-largely-doesnt-support-es6-shouldnt-this-be-mentioned-somewhere), se muestra una respuesta por parte de un moderador que traducida dice: “Microsoft dejó de dar soporte a Internet Explorer el 12 de Enero de 2016” y muestra un link al anuncio en la página oficial de Microsoft: [End of IE Support](https://www.microsoft.com/en-us/windowsforbusiness/end-of-ie-support)

A partir de la [versión 10](https://es.wikipedia.org/wiki/Windows_10) del sistema operativo Windows, Microsoft ha decidido hacer a [Edge](https://en.wikipedia.org/wiki/Microsoft_Edge) su navegador por defecto y limpiar la mala fama que Internet Explorer le dejo los últimos años.
El siguiente es un post oficial publicado por el equipo interno del navegador Edge de Microsoft en el que se destaca el soporte a las nuevas versiones del estándar ECMAScript: [JavaScript moves forward in Microsoft Edge with ECMAScript 6 and beyond](https://blogs.windows.com/msedgedev/2015/05/12/javascript-moves-forward-in-microsoft-edge-with-ecmascript-6-and-beyond)

## Conclusiones
Dar soporte al navegador Internet Explorer implicaría no solo perder las características que el estándar de ECMA nos provee actualmente, sino también sacrificar las futuras.
En base a las estadísticas mostradas anteriormente considero que es importante hacerle saber a cualquier cliente la realidad de la tecnología actual y que las modificaciones que requeriría una retrocompatibilidad implican no solo tiempo, sino también sacrifican el avance en el uso de soluciones más innovadoras y eficientes en sus sistemas.
