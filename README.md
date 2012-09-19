# radio

__radio__, un script python para escuchar la radio con mplayer

# Instalación

[Descargar](https://github.com/quijot/radio/zipball/master) y descomprimir.

## Requisitos previos

[python](http://www.python.org/), [mplayer](http://www.mplayer2.org/). Por lo tanto, __radio es multiplataforma__.

Para instalar ambos en GNU/Linux (reemplazar apt-get con el [gestor de paquetes de tu distribución](https://es.wikipedia.org/wiki/Categor%C3%ADa:Gestores_de_paquetes_Linux)):

    # en Debian, Ubuntu y Mint (con sudo)
    $ apt-get install python mplayer2

En Windows: descargar, guardar, siguiente, siguiente, etc...

Si tenés una Mac sos alto gato. Y si tenés otra cosa, no necesitás de esto.

## Archivos

> Ejecute el comando _tree_ ubicado dentro del directorio donde está __radio__

    $ tree -a
        .
        ├── LICENSE
        ├── lists
        │   ├── .default.list
        │   └── ar.list
        ├── radio
        └── README.md

# Uso

## Escuchar la radio

    $ ./radio <radio_id>

donde \<radio\_id\> debe estar en alguna lista (archivos __.list__ en el
 directorio [__lists__][.l]). Para _apagar la radio_, presione _Ctrl+C_.

Si ejecuta

    $ ./radio

se __imprime la ayuda__ y todas las listas de radios en el directorio [_lists_][.l].

## Listas de radios

Se administran en archivos con extensión _.list_.

Dentro del directorio donde está __radio__, debería encontrarse un directorio
 llamado [_lists_][.l] y allí dentro, un archivo oculto llamado [_.default.list_][.d].

### Agregar radios

Para agregar información de radios puede editar [_.default.list_][.d] o agregar
 archivos _.list_ con el mismo formato interno de [_.default.list_][.d], por ejemplo,
 se adjunta también [_ar.list_][ar] con radios de Argentina.

Dentro de [_.default.list_][.d] está indicado cómo agregar la información:

    Para agregar una radio agregue una línea:
        radio_id: radio_name|radio_url
    
    Por ejemplo:
        ahijuna: Radio Ahijuna FM 94.7|mms://200.110.208.108/ahijunafm

# Licencia

__radio__ se encuentra bajo los términos de la Beer-ware License (Revision 42).
Para mayor información leer
[LICENSE](https://raw.github.com/quijot/radio/master/LICENSE).

[.l]: https://github.com/quijot/radio/tree/master/lists "Directorio de listas de radios."
[.d]: https://raw.github.com/quijot/radio/master/lists/.default.list "Lista de radios por defecto."
[ar]: https://raw.github.com/quijot/radio/master/lists/ar.list "Lista de radios de Argentina."
