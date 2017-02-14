.. _gestion_des_logs:

#############################
Gestion des fichiers journaux
#############################

Les fichiers journaux permettent d'avoir un historique des événements du fonctionnement d'openARIA. Plusieurs fichiers
de logs sont présents dans l'application, chacun ayant un usage différent. 

Fichier journal des erreurs de l'application
############################################

Le fichier **var/log/error.log** contient les erreurs importantes liées à l'utilisation d'openARIA, telles que les erreurs de base de données, les erreurs lors de l'enregistrement d'un fichier sur le disque, les erreurs lors d'une synchronisation des contraintes avec un SIG, etc.

Fichier journal des web services
################################

Le fichier **var/log/services.log** contient une trace de toutes les requêtes entrantes et sortantes des web services openARIA. Pour chaque requête est détaillé le nom de la fonction utilisée, les paramètres en entrée et le retour de la requête.

Fichier journal des plugins
###########################

Les connecteurs externes à openARIA gèrent eux-même leur propre fichier de log.
