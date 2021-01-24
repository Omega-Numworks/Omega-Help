> Mots clés : Submodules, Recursive  
Auteur : Nom de l'auteur, @Syycorax

## Lors de la compilation j'ai l'erreur suivante. Que faire?

```
apps/Makefile:12: apps/atom/Makefile: No such file or directory
make: *** No rule to make target 'apps/atom/Makefile'.  Stop.
```
Lors de l'éxécution de la commande `git clone` il ne faut pas oublier le `--recursive`. Pour remédier à cette erreur il faut exécuter la commande suivante: `git submodule update --init`"