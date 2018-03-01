![SellerAzon](https://sellerazon.com/img/logo.svg)




Diario de actividad
===================
Trata de sustituir las notas

Prioridades
-----------
* SellerAzon
* Wizear
* Documentation

2018-03-01
----------
* [Documentation]() Empiezo diario.md (este diario de actividad) y voy moviendo datos de notas aqui.
* Apache [Kafka](https://kafka.apache.org/) parece que sirve para logs y mensajes que escalan
  * [Kafka papers and presentations](https://cwiki.apache.org/confluence/display/KAFKA/Kafka+papers+and+presentations)
  * [Como lo usa linkedin](https://www.slideshare.net/GuozhangWang/apache-kafka-at-linkedin-43307044)
* Habilito el Plugin de [Atom para Docker](https://github.com/alanzanattadev/atom-docker) y me despierta la curiosidad sobre Atom al ver el [gráfico](https://raw.githubusercontent.com/alanzanattadev/atom-docker/master/screenshot-compose-panel.png) de un Docker basado en Apache Kafka
* Instalo Atom pluging [Ascii-Tree](https://atom.io/packages/ascii-tree) para hacer trees en la documentacion de gulp.js. [Representing a directory file structure in markdown](https://stackoverflow.com/questions/19699059/representing-directory-file-structure-in-markdown-syntax). Al final lo desinstalo porque creo que no funciona (Ctrl+Alt+t)
* Actualizo nethserver.secuware.com y hago un nethserver.md en documentation
* Documentation gulp.md (ejemplo de compilacion de proyecto)
* Pug+markdown-it
  * no consigo [filtrar markdown](https://pugjs.org/language/filters.html#custom-filters) usando jstransformer-markdown-it porque me da error static [analizar posible solucion](https://stackoverflow.com/questions/41987584/pug-js-variable-passing)
  * Docker gulp modificado para jstransformer-markdown-it
  * usar directamente [Pug](https://github.com/pugjs/pug)
    ```javascript
      #!/usr/bin/env node
      'use strict';
      var pug = require('pug');
      var html = pug.renderFile('src/web/index.pug',{
        pretty: true,
        filters: {
          // 'my-own-filter': function (text, options) {
          //   if (options.addStart) text = 'Start\n' + text;
          //   if (options.addEnd)   text = text + '\nEnd';
          //   return text;
          // }
      }// , merge(options, locals));
      });
      console.log(html);
    ```

2018-02-28
----------
* [documentation]() Mejorando documentation
* [gulp]() Mejorado docker gulp para intentar convertir .md a .html

2018-02-27
----------
* [wizear]() Wizear grafo de seguidores

2018-02-26
----------
* [wizear]() Prime es el CSS de GitHub para convertir .md a .html
* [markdown]() Markdown para hacer documentación. Se renderiza en Atom (aunque se puede convertir a HTML)

2018-02-25
----------
* [wizear]() Funcionando un docker usando ecs-cli para manejar un docker parecido al que había en dockercloud. Accede a RDS, S3 desde node (onevoice-toree). No funciona todavia como sustituto de Altavoz-scd

2018-02-22
----------
* [dniweb]() Aprendo lo necesario para utilizar Docker en Amazon (ECS)
* [Dockercloud]() No conseguir acceder a RDS (VPC) borre la maquina y no puedo instalar el Role. Ahora no tengo dockercloud
* [Onevoice]() Migracion de eb a docker de altavoz.sociedadcivil.com  Se queda a medias
* [Onevoice]() Migracion de altavoz-scd.js y altavoz-scd.css de CodeKit a gulp. Creado proyecto docker dniweb/onevoice-three
* [npm-casi2]() Cambiado dependencia script.js por script-js.js
* [Onevoice]() Posible corrección de Twitter ID grandes en altavoz.sociedadcivil.com el error puede que este en el log de logins en casi2 / mysql.js
* [npm-casi2]() Eliminación de la dependencia de getimage.php en usertokens.js para moverlo a js
* [npm-casi2]() Instalado npm-check-updates (ncu) para actualizar package.json
* [sellerAzon]() Analizar [Redux](https://redux.js.org) para almacenar el estado de aplicaciones
* [sellerAzon]() Estudio de voronoi en d3js para mejorar UX en la selección de graficos

Versiones de este documento
---------------------------
| Fecha  | Revision |
|---|---|
| 2018-03-01 | Primera version |


<a href="https://pugjs.org"><img src="https://sellerazon.com/img/logo.svg" height="120" <a href="https://pugjs.org"><img src="https://sellerazon.com/img/logo.svg" height="50" align="right"></a>

<a href="https://pugjs.org"><img src="https://cdn.rawgit.com/pugjs/pug-logo/eec436cee8fd9d1726d7839cbe99d1f694692c0c/SVG/pug-final-logo-_-colour-128.svg" height="200" align="right"></a>
