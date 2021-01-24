> Mots clés : Toolchain, Not found  
Auteur : Hector Nussbaumer, @Syycorax

## Lors de la compilation j'ai l'erreur suivante. Que faire?

```
/bin/sh: arm-none-eabi-g++: command not found
```

Il semblerait que la Toolchain ARM ne soit pas installée. Pour le vérifier, on peut exécuter la commande suivante :

```bash
which arm-none-eabi-g++
```

Si cette commande renvoie

```
arm-none-eabi-gcc not found
```

La toolchain n'est pas installée ou pas/mal indiquée dans le PATH. Voici comment corriger l'erreur :

1. Verifier que la [toolchain](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads) est bien installée ;

2. Ajouter la toolchain dans le PATH avec la commande suivante :

```bash
export PATH=$PATH:~/.local/bin/:/chemin-de-la-toolchain/bin
