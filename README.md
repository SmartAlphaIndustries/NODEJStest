# NODEJStest


## Errores ocurridos durante la instalación
Tras haber instalado NodeJS y NestJs, FEDORA incumple algunos requerimientos como la instalación del yarn, es necesario hacerlo a través de ``` dnf install yarnpkg```

Después realizar lo siguiente
```bash
$ mkdir ~/.npm-global

$ npm config set prefix '~/.npm-global'

$ export PATH=~/.npm-global/bin:$PATH


```

En mi caso, utilizó zsh, por lo tanto antes de  realizar 
```bash
$  source ~/.bash_profile
```
Nota en otros SO's es:
```bash
$  source ~/.profile
```

tuve que realizar 
```bash
$ exec bash
```

Finalmente para volver a zsh
```bash
$ yaexec zsh
```



