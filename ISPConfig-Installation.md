**Tout le travail ici se fera sur le server 1, un server ubuntu**

- Mettons à jour le système:

`sudo apt-get update && sudo apt-get upgrade`

Dans la suite du travail, nous aurons besoin d'un nom de domaine, nous allons faisons donc une reservation de nom de domaine sur
https://www.freenom.com/fr/index.html

Nous avons reservé le domaine: `cyber-spector.icu`

Pour ISPConfig, nous allons creer un sous domaine `ispconfig.cyber-spector.icu`

- Configurer le nom du server:

`nano /etc/hostname`

    ispconfig.cyber-spector.icu

- Configurer le ficher /etc/hosts

`sudo nano /etc/hosts`

    127.0.0.1 ispconfig.cyber-spector.icu
    127.0.0.1 localhost

- Redémarrez la machine

    `systemctl reboot`

**Étape 2** - Exécuter le programme d'installation pour ISPConfig

