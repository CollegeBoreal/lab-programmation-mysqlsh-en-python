{{ chefs }} :tada: :tada: :tada: 

C'est ce que l'on appelle un parcours sans faute.

- [ ] Rajouter manuellement un document

Pour terminer, on va rajouter un document manuellement pour expérimenter l'API

Dans la fonction `former_des_chefs`, juste aprés la création de la collection `chefs_de_gouvernement` ajoute le code ci-dessous en respectant l'indentation

```
  # Ajout manuel
  maColl.add({"HeadOfState": "Marc Ravalomanana","GovernmentForm": "Republic"}).execute()
```

- [ ] Sauvegarder la collection des chefs dans la base de données

Ajoute un commentaire `#` devant la ligne `#db.drop_collection(nomColl)` dans la fonction `former_des_chefs`

```
  # Détruit la collection
  #db.drop_collection(nomColl)
```

- [ ] Exécute ton programme. Et vérifie la collection avec [MySQLWorkBench](https://www.mysql.com/products/workbench/)

- [ ] Sauveguarde ta base de données (dump)

:warning: Remplace `--MON-REPERTOIRE--` par le répertoire ou tu as cloné ton référentiel (par exemple Developer)

:computer: Sous PowerShell

```
PS > docker container exec some-mysqlds `
        mysqldump --user root --password=password world_x `
        > $ENV:UserProfile\--MON-REPERTOIRE--\lab-programmation-mysqlsh-en-python\b000000000.sql
```

:apple: Sous Bash

```
$ docker container exec some-mysqlds \
         mysqldump --user root --password=password world_x \
         > ~/--MON-REPERTOIRE--/lab-programmation-mysqlsh-en-python/b000000000.sql
```


**Soumet ton code** vers GitHub pour continuer:
```
git add b000000000.py b000000000.sql
git commit -m "Tutoriel complété"
git push
```
