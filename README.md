```error: could not find expected file curl/curl.h, or curl/curl.h for curl -- you may have to install curl in your system and/or pass curl_dir or curl_incdir to the luarocks command. example: luarocks install lua-curl curl_dir=/usr/local```

Este error se debe a un error de ubicacion de curl

para arregalarlo ubicar la carpeta curl en /usr/include/

Clonamos repositorio.

```git clone https://github.com/george0884/lua-curl-error```


Descomprimimos.

```cd lua-curl-error && tar -xzvf curl.tar.gz```


Copiamos la carpeta.

```sudo cp curl -r /usr/include/```


Monocomando recomendado, no deja residuos.

```git clone https://github.com/george0884/lua-curl-error && cd lua-curl-error && tar -xzvf curl.tar.gz && sudo cp curl -r /usr/include/ && cd .. && sudo rm -Rf lua-curl-error```

Done!.
