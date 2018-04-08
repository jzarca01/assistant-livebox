# EN COURS DE DEVELOPEMENT !

# assistant-livebox

Ce plugin de [`assistant-plugins`](https://aymkdn.github.io/assistant-plugins/) permet de contrôler la Livebox d'Orange.

> Consulter [le changelog](https://github.com/Aymkdn/assistant-livebox/blob/master/changelog.md) pour connaitre les dernières mises à jour.

**ATTENTION** : vous n'avez besoin **QUE** du plugin `assistant-livebox` pour piloter la Livebox (pas besoin de `assistant-ifttt` ou `assistant-wait`, ou autre....).  

Merci à [@ABOAT](https://github.com/ABOATDev) pour avoir testé le plugin, puisque je ne possède pas de Livebox !

## Installation

Si vous n'avez pas installé [`assistant-plugins`](https://aymkdn.github.io/assistant-plugins/), alors il faut le faire, et sélectionner **livebox** comme plugin.

Si vous avez déjà installé [`assistant-plugins`](https://aymkdn.github.io/assistant-plugins/), et que vous souhaitez ajouter ce plugin, alors :
  - Pour Windows, télécharger [`install_livebox.bat`](https://github-proxy.kodono.info/?q=https://raw.githubusercontent.com/Aymkdn/assistant-livebox/master/install_livebox.bat&download=install_livebox.bat) dans le répertoire `assistant-plugins`, puis l'exécuter en double-cliquant dessus.  
  - Pour Linux/MacOS, ouvrir une console dans le répertoire `assistant-plugins` et taper :  
  `npm install assistant-livebox@latest --save --loglevel error && npm run-script postinstall`

## Configuration

Éditer le fichier `configuration.json` du répertoire `assistant-plugins`.

Dans la section concernant le plugin `livebox`, on trouve plusieurs paramètres.

### Paramètre `ip_box`

Il s'agit de l'adresse IP de votre décodeur Livebox. Si vous n'avez pas bidouillé votre réseau, vous devriez pouvoir laisser l'IP par défaut.


## Utilisation

J'ai créé des applets IFTTT qui sont déjà disponibles. Vous pouvez donc les utiliser.

Voici les phrases clés à dire — s'assurer d'avoir installé les applets associées :
  - `allume la livebox` ([https://ifttt.com/applets/zXEgyuJZ-allume-la-livebox](https://ifttt.com/applets/zXEgyuJZ-allume-la-livebox)) : allume **seulement** la livebox
  - `allume la télé` ([https://ifttt.com/applets/bkVTxw7F-allume-la-tele-via-la-livebox/](https://ifttt.com/applets/bkVTxw7F-allume-la-tele-via-la-livebox/)) : allume la livebox **ET** va mettre une chaine télé (via livebox TV, ou via Mon Bouquet, ou via Les Chaines CANAL selon la configuration)
  - `allume la télé et zappe sur ...` ([https://ifttt.com/applets/Bj6nH7Xw-allume-la-tele-via-la-livebox-et-zappe-sur-une-chaine](https://ifttt.com/applets/Bj6nH7Xw-allume-la-tele-via-la-livebox-et-zappe-sur-une-chaine)) : allume la livebox (si elle n'est pas allumée) puis va mettre la chaine de télé demandée   
    Exemples :  
    *OK Google, allume la télé et zappe sur M6*  
    *OK Google, allume la télé et zappe sur la 6*  
  - `éteins la livebox` ([https://ifttt.com/applets/TaE7QPgp-eteins-la-livebox](https://ifttt.com/applets/TaE7QPgp-eteins-la-livebox)) : pour éteindre la livebox
  - `zappe sur ...` ([https://ifttt.com/applets/d6B7Yrk5-zappe-sur-une-chaine-de-la-livebox](https://ifttt.com/applets/d6B7Yrk5-zappe-sur-une-chaine-de-la-livebox)) : zappe sur la chaine demandée, et fonctionne aussi avec le numéro de la chaine  
   Exemples :  
    *OK Google, zappe sur TMC*  
    *OK Google, zappe sur la 10*  
  - `coupe le son de la livebox` ([https://ifttt.com/applets/kx4Ku7vj-coupe-le-son-de-la-livebox](https://ifttt.com/applets/kx4Ku7vj-coupe-le-son-de-la-livebox))
  - `remets le son de la livebox` ([https://ifttt.com/applets/S4wcuJn7-remets-le-son-de-la-livebox](https://ifttt.com/applets/S4wcuJn7-remets-le-son-de-la-livebox))
  - `baisse le son de la livebox` ([https://ifttt.com/applets/WWf3zG58-baisse-le-son-de-la-livebox](https://ifttt.com/applets/WWf3zG58-baisse-le-son-de-la-livebox)) : va baisser le son de 15 barres
  - `baisse le son de la livebox de X` ([https://ifttt.com/applets/cbeL79cW-baisse-le-son-de-x-barres-sur-la-livebox](https://ifttt.com/applets/cbeL79cW-baisse-le-son-de-x-barres-sur-la-livebox)) : va baisser le son de X barres  
   Exemple : *OK Google, baisse le son de la livebox de 50*
  - `monte le son de la livebox` ([https://ifttt.com/applets/uCcg6RdE-augmente-le-son-de-la-livebox](https://ifttt.com/applets/uCcg6RdE-augmente-le-son-de-la-livebox)) : va augmenter le son de 15 barres
  - `monte le son de la livebox de X` ([https://ifttt.com/applets/UuDGXdmL-augmente-le-son-de-x-barres-sur-la-livebox](https://ifttt.com/applets/UuDGXdmL-augmente-le-son-de-x-barres-sur-la-livebox)) : va augmenter le son de X barres  
    Exemple : *OK Google, augmente le son de la livebox de 25*
  - `mets la livebox sur pause` ([https://ifttt.com/applets/N7um4qJU-mets-sur-pause-la-livebox](https://ifttt.com/applets/N7um4qJU-mets-sur-pause-la-livebox)) : met le programme en cours sur pause
  - `remets la livebox en lecture` ([https://ifttt.com/applets/mHAXMym9-remets-la-livebox-en-lecture](https://ifttt.com/applets/mHAXMym9-remets-la-livebox-en-lecture)) : remet en lecture le programme en cours
  - `reviens au direct` ([https://ifttt.com/applets/zfSALsrD-remets-le-direct-sur-la-livebox](https://ifttt.com/applets/zfSALsrD-remets-le-direct-sur-la-livebox)) : lorsque la livebox TV a été mise sur pause et qu'on souhaite revenir au direct
  - `va dans Mes Enregistrements` ([https://ifttt.com/applets/KxHGy7vw-va-dans-mes-enregistrements-sur-la-livebox](https://ifttt.com/applets/KxHGy7vw-va-dans-mes-enregistrements-sur-la-livebox)) : pour aller dans le menu "Mes Enregistrements" de la livebox
  - `va dans Mes Vidéos` ([https://ifttt.com/applets/ZkWauBKi-va-dans-mes-videos-sur-la-livebox](https://ifttt.com/applets/ZkWauBKi-va-dans-mes-videos-sur-la-livebox)) : pour aller dans le menu "Mes Vidéos" de la livebox
  - `va dans le dossier ...` ([https://ifttt.com/applets/bbdEPtcx-va-dans-un-dossier-stocke-sur-la-livebox](https://ifttt.com/applets/bbdEPtcx-va-dans-un-dossier-stocke-sur-la-livebox)) : parcourt tous les dossiers définis dans `search_path` (voir la section Configuration ci-dessus) afin de trouver le dossier souhaité  
    Exemples :  
    *OK Google, va dans le dossier Star Trek*  
    *OK Google, va dans le dossier The Walking Dead* (il vous faudra prendre votre plus bel accent anglais !)

## Personnalisation

Il est également possible de créer ses propres applets et commandes pour piloter la livebox.

Il faut pour cela procéder ainsi :

  1) Créer une nouvelle *applet* dans IFTTT : [https://ifttt.com/create](https://ifttt.com/create)  
  2) Cliquer sur **this** puis choisir **Google Assistant**  
  3) Choisir la carte **Say a simple phrase** (ou autre, selon votre cas)  
  4) Dans *« What do you want to say? »* mettre la phrase qui va déclencher l'action  
  5) Remplir les autres champs de la carte  
  6) Maintenant, cliquer sur **that** puis choisir **Pushbullet**  
  7) Choisir la carte **Push a Note**  
  8) Dans le champs *« Title »*, mettre `Assistant`  
  9) Dans le champs *« Message »*, mettre `livebox_` suivi par la commande souhaitée (si plusieurs commandes, les séparer par une virgule) (voir plus bas)  
  10) Enregistrer puis cliquer sur **Finish**  
  11) Dites : « OK Google » suivi de votre phrase spéciale du point 4)  
  12) Google Home va s'exécuter

### Commandes

Dans l'étape 9) précédente, vous devez y indiquer une commande. Voici donc les commandes disponibles :

  - `red` : envoie la commande `red` (touche rouge de la télécommande)
  - `yellow` : envoie la commande `yellow` (touche jaune de la télécommande)
  - `blue` : envoie la commande `blue` (touche bleue de la télécommande)
  - `green` : envoie la commande `green` (touche verte de la télécommande)
  - `up` : envoie la commande `up` (flèche haut)
  - `down` : envoie la commande `down` (flèche bas)
  - `left` : envoie la commande `left` (flèche gauche)
  - `right` : envoie la commande `right` (flèche droite)
  - `OK` : envoie la commande `OK`
  - `mute` : envoie la commande `mute` (sourdine)
  - `play` : envoie la commande `play`
  - `fwd` : envoie la commande `fwd` (avance rapide)
  - `bwd` : envoie la commande `bwd` (retour rapide)
  - `waitXXXX` : enclenche un timer de XXXX millisecondes
  - `on` : envoie la séquence `power` suivi d'un timer de 7 secondes (`wait7000`)
  - `off` : envoie la commande `power`
  - `tv` : envoie la séquence `home`, `wait2000`, `right`, `left`, `red`, `ok`, `wait4000`
  - `unmute` : envoie `mute`
  - `home` : envoie la séquence `home`, `wait2000`, `red`
  - `back` : envoie la commande `red`
  - `pause` : envoie la commande `play`
  - `videos` : envoie la séquence `home`, `wait2000`, `right`, `left`, `red`, `right`, `ok`
  - `direct` : envoie la séquence `green`, `ok`
  - `enregistrements` : envoie la séquence `home`, `wait2000`, `right`, `left`, `red`, `up`, `ok`
  - `soundDown` : envoie la commande `vol_dec`
  - `soundUp` : envoie la commande `vol_inc`
  - `programUp` : envoie la commande `prgm_inc`
  - `programDown` : envoie la commande `prgm_dec`
  - `folder XYZ` : permet de chercher le répertoire XYZ dans `search_path` (qui est défini dans la configuration), puis de s'y rendre
  - `zappe sur ABC` : permet de zapper sur la chaine ABC (exemple : `livebox_zappe sur la 1` ou `livebox_zappe sur TF1`)

### Exemple

Par exemple, supposons que vous avez un enregistrement journalier (disons l'émission [Quotidien de Yann Barthès qui passe sur TMC](https://www.tf1.fr/tmc/quotidien-avec-yann-barthes)), et que vous souhaitez lancer le dernier Quotidien enregistré.

Pour cela vous souhaitez donner la commande : *OK Google, lance le programme Quotidien*

Il faut donc créer une applet IFTTT (comme décrit plus haut) et pour la commande envoyée à Pushbullet vous mettrez : `livebox_enregistrements,wait7000,ok,ok` qui peut se traduire par `livebox, va dans Mes Enregistrements, puis patiente 7 secondes, et ensuite appuie sur OK, puis OK encore une fois`
