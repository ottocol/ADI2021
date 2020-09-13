# Software necesario para ADI 20/21
 
Todo el software es multiplataforma y funciona en Windows, Linux y OSX.

## Node

### Linux/MacOS

> Además de lo explicado aquí,  puedes ir a la [página oficial de descargas](https://nodejs.org/es/download/) de Node, pero esa instalación sí requiere permisos de `root`

Lo más sencillo es usar `n`, un gestor de versiones de Node que nos permite tener varias versiones coexistiendo en nuestra máquina y no necesita permisos de superusuario para instalarlas. Así podemos instalarlo en un par de minutos en cualquier máquina.

Para instalar la última versión LTS de Node con `n`, simplemente tecleamos en una terminal:

```bash
curl -L https://git.io/n-install | bash
```
La instalación se hace en el directorio `$HOME/n`, para no requerir permisos de superusuario (la instalación ya habrá actualizado las  variables de entorno para apuntar a este directorio). Para ver más información sobre la herramienta (cómo instalar varias versiones de Node en la misma máquina, fijar por defecto cuál usar, etc), puedes ver su [repo de Github](https://github.com/tj/n).

### Windows

Puedes [descargar un instalador](https://nodejs.org/es/download/) desde la web de NodeJS.

### Comprobar que node está instalado correctamente

Ahora para comprobar que node está instalado, teclea en una terminal:

```bash
node --version
```

debería aparecer la versión instalada de Node. Si no funciona abre otra terminal y ejecuta de nuevo el comando, ya que es posible que las variables de entorno del instalador todavía no hayan tenido efecto en la terminal actual.

## Herramientas adicionales que necesitarás

- [Postman](https://www.getpostman.com/) o [HTTPie](https://httpie.org/) para hacer peticiones de prueba al API REST
- Algunos paquetes adicionales de node. Teniendo instalado ya node, en una terminal, sea windows, linux o Mac, escribe

```bash
npm install -g nodemon # para todas las prácticas
npm install -g @vue/cli # para la práctica 3
```
- Un navegador web cualquiera (recomendables Chrome o Firefox)
- Un editor de código para Javascript/HTML/CSS. Usa el que prefieras, aunque en los laboratorios está el [Visual Studio Code](https://code.visualstudio.com/)