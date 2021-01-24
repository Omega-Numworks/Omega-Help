> Mots clés : Toolchain, Not found  
Auteur : Nom de l'auteur, @Syycorax

## Lors de la compilation j'ai l'erreur suivante. Que faire?

```/bin/sh: arm-none-eabi-g++: command not found```

Il semblerait que la Toolchain ARM ne soit pas installée, pour le verifier, on peut executer 

``which arm-none-eabi-g++``

Si cette commande renvoie

``arm-none-eabi-gcc not found``

La toolchain n'est pas installée ou pas/mal indiquée dans le PATH

1. Verifier que la [toolchain](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads)est bien installée:

2. Ajouter la toolchain dans le PATH: executer

``export PATH=$PATH:~/.local/bin/:/chemin-de-la-toolchain/bin
``

En cas de problème, vous pouvez nous contacter dans le salon #help-fr du [discord](https://discord.gg/JpmjSH3)