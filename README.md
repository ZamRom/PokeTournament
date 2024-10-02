# PokeTournament
Project to System modeling

## Contactos

Ariel Rodolfo Zarmudio Romero- zamromxd@gmail.com

## Licencia

PokeSearch es distribuido bajo la licencia [GNU](https://es.wikipedia.org/wiki/GNU_General_Public_License).

## Descripción

PokeTournament esta planteado para ser un modelo de como sucedería un torneo de Pokémon al simular combates entre los equipos que el usuario brinde como valores iniciales para hacer simulaciones con equipos reales o "preestablecidos" (como los que ya tienen NPC de los juegos) para distintos propositos.

## Justificación

Se encontró que es complicado para jugadores que no han tenido un acercamiento a los juegos estilo RPG o TBS tienen ciertas dificultades en entender el sistema de combate o sus relaciones entre 'stats' con respecto a los ataques y pokemon por lo que se desarrolla este modelo planeando que para estos usuarios sea mas sencillo tener este acercamiento hacia los pokemon y sus relaciones para que no tengan problemas para iniciar a jugar la saga principal de Pokémon

## Características

- **Torneo dinamico:** El torneo con los mismos equipos deberían resultar distintos tan solo con ordenar de manera distinta los pokemon iniciales de cada equipo.
- **Comportamiento semirealista (con respecto a los juegos):** El modelo debería actuar de manera estrategica con respecto a solo la informacion que tiene, es decir, actuara de manera estrategica solo hacía los pokemon que ha visto y solo con movimientos que realmente si podrían aprender.

## Hipotesis

Dado 2^n equipos de Pokémon dados por el usuario, simular combates dobles usando de manera estrategica sus movimientos para vencer al equipo enemigo de manera procedural hasta obtener un vencedor del torneo. Se planea extender este apartado de manera posterior \*

## Arquitectura

**Adquisición:** Para la adquisicion de informacion se utilizará la base de datos creada por el equipo del proyecto de [PokeSearch](https://github.com/ZamRom/PokeSearch) aunque podría ser modificada en un uso posterior si se ve que no cumplé los valores requeridos para el proyecto.  
**Almacenamiento:** Se utilizará MariaDB como MDBS para realizar las consultas SQL requeridas.
**Procesamiento:** Una vez que el usuario creé e inserte los equipos de pokemon para el torneo se planea que sea organizado de manera aleatoria para brindar dinamismo y utilizando las formulas de creacion de estadisticas y de daño se simule el combate de la mejor manera. Dentro del combate podría usarse el algoritmo creado para el proyecto de PokeSearch para escoger el mejor pokemon del equipo para el combate actual.

## Tecnologías Utilizadas

- [Python](https://docs.python.org/release/3.11.9/) (v3.11.9)
- [mysql](https://dev.mysql.com/doc/connector-python/en/)
- [MariaDB](https://mariadb.com/kb/en/documentation/)