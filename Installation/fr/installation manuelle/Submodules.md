> Mots clés : Submodules, Recursive  
Auteur : Hector Nussbaumer, @Syycorax

## Lors de la compilation, j'ai l'erreur suivante. Que faire?

```
apps/Makefile:12: apps/atom/Makefile: No such file or directory
make: *** No rule to make target 'apps/atom/Makefile'.  Stop.
```
Lors de l'exécution de la commande `git clone`, il ne faut pas oublier le `--recursive`.
Si vous avez déjà clone, vous pouvez remédier à cette erreur en exécutant la commande suivante : 
```bash
git submodule update --init
```