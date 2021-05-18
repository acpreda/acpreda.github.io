# acpreda.github.io

## Generación del sitio

Con Docker se obtiene un contenedor de Jekyll y se ejecuta así desde el directorio
raiz del proyecto:
```
cd Projects/acpreda/acpreda.github.io
docker run \
  --name jekyll \
  --volume="$PWD:/srv/jekyll" \
  -p 4000:4000 \
  -it \
  jekyll/jekyll:4 \
  /bin/bash
```
