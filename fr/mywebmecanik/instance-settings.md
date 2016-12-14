# Paramétrage d'une instance

## Introduction ##

Le paramétrage du nom de domaine d'envoi des emails est une étape importante. Sans ce paramétrage, aucun email ne partira de la plateforme.
Vous retrouvez toutes ces informations dans les détails techniques de l'instance.

[image](assets/instance-details.png)

## Fichier TXT : Autorisation d'utilisation du nom de domaine ##

Il vous sera demandé pour chaque compte, de déposer un fichier `.txt` à la racine du nom de domaine (via accès FTP). Ce fichier à un nom unique qui montrera au routeur email que vous avez la maitrise sur le nom de domaine, et nous autorisera ainsi à l'utiliser.

1. Créer le fichier (vide) avec le nom indiqué (ex : `jlbzgoh89Y4IOUEOI.txt`)
2. Le déposer à la racine du nom de domaine. (par exemple, l'URL suivant doit exister et afficher une page blanche : `http://mondomaine.comjlbzgoh89Y4IOUEOI.txt`)
3. Retournez sur les détails de l'instance sur myWebmecanik et cliquez sur le bouton **valider**.

## Redirection SPF : Amélioration de la délivrabilité ##

1. Sur le paramétrage des DNS du nom de domaine, créez une entrée SPF comme donnée dans le détail de l'instance. **Note** : Il est possible que vous ayez déjà une entrée SPF, hors il n'est pas possible d'avoir plusieurs entrée sur un même nom de domaine. Consultez la [documentation Google pour les entrées multi SPF](https://support.google.com/a/answer/4568483?hl=fr).
2. Retournez sur les détails de l'instance sur myWebmecanik et cliquez sur le bouton **valider**.

## Redirection DKIM : Amélioration de la délivrabilité ##

1. Sur le paramétrage des DNS du nom de domaine, créez une entrée DKIM comme donnée dans le détail de l'instance.
2. Retournez sur les détails de l'instance sur myWebmecanik et cliquez sur le bouton **valider**.
