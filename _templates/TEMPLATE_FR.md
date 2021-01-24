> Mots clés : flash, mémoire  
Auteur : hector Nussbaumer, @Syycorax
## Lors de la compilation j'ai l'erreur suivante. Que faire?

```
region `FLASH' overflowed by 42802 bytes
```
Cette erreur survient lors de la compilation pour n0100. Malheureusement, toutes les langues ne rentrent plus dans la mémoire de la n0100. Il faut donc ajouter ce flag a la compilation
```
EPSILON_I18N=fr
```
"fr" est a remplacer avec la langue voulue.