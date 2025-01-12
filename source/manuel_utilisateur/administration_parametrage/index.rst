#############################
Administration et paramétrage
#############################


Etablissements
==============

Type
----

Typologie d'un établissement représentant son activité.


Catégories
----------

Liste des catégories d'un établissement représentant sa capacité.


Natures
-------

Liste des natures d'un établissement (ERP Référentiel, ERP non référentiel, Bâtiment non ERP, ...).

Codes :
 

États
-----

Liste des états d'un établissement (Ouvert, Fermé, Non suivi, ...).

Codes :


Statut juridique
----------------

Liste des statuts juridiques d'un établissement (ville, public, privé, ...).

Codes :


Tutelle administrative
----------------------

Liste des tutelles administratives d'un établissement lorsque son statut juridique est 'public' ou du code 'PUB'.


Périodicité de Visite
---------------------

Paramétrage de la périodicité des visites obligatoires à réaliser sur les établissements de nature 'ERP référentiel'.


La périodicité des visites s'applique sur les établissements dont la nature est 'ERP Référentiel' (**etablissement_nature_periodique** : paramètre correpondant au code de la nature 'ERPR'), dans l'état 'Ouvert' (**etablissement_etat_periodique** : paramètre correpondant au code de l'état 'OUVE') et dont la ou les autorités compétentes sont paramétrées à 'CCS' et/ou 'SCDS' (**etablissement_autorite_competente_periodique** : paramètre correspondant aux codes des autorités compétentes 'CCS' et/ou 'SCDS').

Un dossier de coordination de type 'Visite Périodique de Sécurité' (**dossier_coordination_type_periodique** : paramètre correpondant au code du type de dossier de coordination 'VPS') est le dossier de coordination rattaché à un établissement pour la gestion de la périodicité des visites.


Adresses
========

Voies
-----

Liste des voies auxquelles sont rattachées les établissements.


Arrondissements
---------------

Liste des arrondissements auxquels sont rattachés les établissements.


Contacts
========

Types
-----

Typologie d'un contact.

Codes :

  - EXPL
  - INST


Civilités
---------

Liste des civilités d'un contact.


Contraintes
===========

Listing
-------

Liste des contraintes paramétrées et destinées à être appliquées aux établissements et dossiers de coordination.
Elles peuvent provenir d'un référentiel SIG (via une synchronisation) ou être ajoutées manuellement.

Les informations spécifiques et facultatives d'une contrainte paramétrée sont :

  - l'ordre d'affichage (permet de classer les contraintes appliquées à un établissement ou un dossier de coordination à l'intérieur des groupes et sous-groupes) ;
  - le texte surchargé (permet d'étendre le texte standard de la contrainte à respecter).

Synchronisation
---------------

L'option SIG doit être activée pour faire apparaître cette rubrique.
Effectuer une synchronisation revient à mettre à jour les contraintes paramétrées selon le référentiel SIG :

  - s'il manque des contraintes dans openARIA elles sont ajoutées ;
  - si des contraintes d'openARIA ne sont plus dans le référentiel elles sont archivées ;
  - si des contraintes d'openARIA sont dans le référentiel elles sont mises à jour.

.. image:: contrainte_synchronisation.png

Seules contraintes paramétrées provenant d'un référentiel sont impactées par la synchronisation : celles ajoutées manuellement ne sont pas concernées.
La synchronisation ne se fait que dans le sens SIG → openARIA : les contraintes présentes sur le référentiel ne sont pas modifiées.

Les informations d'une contrainte récupérée du SIG sont :

  - identifiant dans le référentiel ;
  - nature (POS/PLU/CC/RNU) ;
  - groupe ;
  - sous-groupe ;
  - libellé ;
  - texte.

.. note::

  Lorsque l'on récupère des contraintes pour un établissement ou un dossier de coordination, openARIA est susceptible de demander une synchronisation des contraintes
  dans le cas où les contraintes récupérées depuis le référentiel SIG sont absentes du paramétrage.


Métiers
=======

Services
--------

Liste des services.


Acteurs
-------

Liste des acteurs de l'application représentant les cadres, techniciens et secrétaires affectés à un service. Un acteur peut être rattaché à un utilisateur ou non.


Avis
----

Liste des avis possibles sur un dossier que ce soit en réunion, suite à une visite ou dans une analyse.


Instances
---------

Paramétrage des instances convoquées lors des réunions ou lors des visites ainsi que de leurs membres.


Autorités compétentes
---------------------

Liste des autorités compétentes d'un dossier d'instruction.


Dérogations SCDA
----------------

Liste des dérogations SCDA disponibles depuis les données techniques des établissements.


Réunions
========

Types
-----

Typologie et paramétrage de toutes les informations communes à chaque réunion et qui caractérisent un type de réunion.


Catégories
----------

Liste des catégories de dossiers traitées en réunion.


Autorités de police
===================

Types
-----

Typologie et paramétrage d'une décision d'autorité de police notamment les délais.


Motifs
------

Liste des motifs d'une décision d'autorité de police.


Analyses
========

Types
-----

Typologie et paramétrage des analyses notamment les modèles d'éditions associés.


Essais réalisés
---------------

Textes types disponibles à l'insertion depuis le formulaire de saisie des essais réalisés lors de l'analyse des dossiers d'instruction.


Documents présentés
-------------------

Textes types disponibles à l'insertion depuis le formulaire de saisie des documents présentés lors de l'analyse des dossiers d'instruction.


Réglementations applicables
---------------------------

Textes types disponibles à l'insertion depuis le formulaire de saisie des réglementation applicables lors de l'analyse des dossiers d'instruction.


Prescriptions
-------------

Paramétrage des prescriptions réglementaires et spécifiques utilisées dans les analyses des dossiers d'instruction.


Documents entrants
==================

Types
-----

Typologie d'un document entrant.


Documents générés
=================

Compléments
-----------

Textes types disponibles à l'insertion depuis le formulaire de saisie d'un document généré dans les champs compléments.


Qualités de signataire
----------------------

Liste des qualités d'un signataire.


Signataires
-----------

Paramétrage des signataires disponibles depuis un document généré ou un PV.


Visites
=======

Durées
------

Liste des durées de visite.


Motifs d'annulation
-------------------

Liste des motifs d'annulation d'une visite.


Dossiers
========

Types
-----

Typologie des types de dossiers de coordination (Visites, Plans, ...).


Types de DC
-----------

Typologie et paramétrage des dossiers de coordination (AT, PC, Visite périodque, ...).

.. _administration_geolocalisation:


Éditions
========

Types
-----

Typologie et paramétrage d'un modèle d'édition qui permet de filtrer les modèles d'édition disponibles en fonction du contexte des interfaces.


Catégories
----------

Paramétrage des catégories de types de modèles d'édition. Cette catégorisation permet de définir le contexte dans lequel les types de modèles d'édtion rattachés à cette catégorie vont être disponibles.


Modèles d'édition
-----------------

Paramétrage des modèles d'édition par la sélection de leur type et de la lettre type utilisée.


Lettres types
-------------

Composition des lettres types.


Logos
-----

Paramétrage des logos disponibles depuis l'écran de composition des lettres types.


Sous-états
----------

Paramétrage des tableaux (appelés sous-états) disponibles à l'insertion depuis l'écran de composition des lettres types.


Requêtes
--------

Paramétrage des configurations de champs de fusion disponibles depuis l'écran de composition des lettres types.


Général
=======

Collectivités
-------------

Paramétrage des collectivités.

.. _administration_parametre:

Paramètres
----------

Divers paramètres de l'application : champs de fusion généraux disponibles pour les éditions pdf, activation/désactivation de modules complémentaires, paramétrages fonctionnels, ...

Utilisation des options :

* **etablissement_code_prefixe** : Par défaut : ''. A la création d'un établissement, le code est composé de ce préfixe et d'un identifiant numérique. Par exemple : 'T12' ou 'F2432'.

* **etablissement_nature_erpr** : code de la nature d'établissement qui correspond à un ERP Référentiel (voir :ref:`etablissement_listing_referentiel`).

**etablissement_autorite_competente_periodique** : code des autorités compétentes qui correspondent aux autorités compétentes mandatées pour mener des visites périodiques. Par exemple : 'CCS' ou 'SCDS'. Si plusieurs autorités compétentes sont mandatées pour mener des visites périodiques, le paramètre sera renseigné de la façon suivante : 'CCS;SCDS'.

* **option_sig** : la valeur par défaut est *aucun*. Les valeurs possibles sont
  *sig_externe*, *sig_interne* ou *aucun*.

* **option_contrainte** : la valeur par défaut est *true*. Les valeurs possibles sont *true* et *false*.

* **option_unite_accessibilite** : la valeur par défaut est *true*. Les valeurs possibles sont *true* et *false*.

* **option_referentiel_patrimoine** : :ref:`module_interface_avec_le_referentiel_patrimoine`

* **swrod** : :ref:`module_swrod`

* **option_referentiel_ads** : :ref:`module_interface_avec_le_referentiel_ads`

* **dc_a_qualifier_redlimit** : c'est le nombre de jours depuis la date de la demande à partir duquel les enregistrements dans le listing des DC à qualifier et dans le widget des DC à qualifier apparaissent en rouge. Si le paramètre n'est pas positionné alors la valeur par défaut est de 15 jours. :ref:`dossiers_dc_a_qualifier`

* **template__proces_verbal_numero** : Par défaut : `[ANNEE]/[CHRONO]`. Les variables de remplacement disponibles sont : [ANNEE] ('2017' année du PV sur 4 caractères), [CHRONO] ('00123' séquence du procès verbal pour le service pour l'année du PV).

* **template__proces_verbal_numero_complet** : Par défaut : `[CODE_SERVICE]-[PROCES_VERBAL_NUMERO]`. Les variables de remplacement disponibles sont : [CODE_SERVICE] ('SI' ou 'ACC' le code du service émetteur en majuscule), [PROCES_VERBAL_NUMERO] (le numéro officiel du procès verbal selon le template ci-dessus).

* **template__arrete_numero** : Par défaut : `[ANNEE]_[CHRONO]_ERP`. Les variables de remplacement disponibles sont : [ANNEE] ('2017' année de l'arrêté sur 4 caractères), [CHRONO] ('00123' séquence de l'arrêté pour cette année).


Gestion des utilisateurs
========================

Profils
-------

Paramétrage des profils utilisateurs et de toutes les permissions qui y sont associées.


Utilisateurs
------------

Paramétrage des utilisateurs autorisés à se connecter à l'application.


Tableaux de bord
================

Widgets
-------

Paramétrage des blocs d'informations affichables sur le tableau de bord.


Composition
-----------

Composition des tableaux de bord par profil.


Options avancées
================

Géolocalisation
---------------

Si un SIG externe est paramétré, il est possible de géolocaliser l'ensemble des établissements
et des dossiers de coordination, en un seul clic.

.. image:: administration_geocoder-tous.png

Un message de validation fait apparaître le nombre d'éléments qui ont pu être géolocalisés
automatiquement par le SIG, ainsi que le nombre d'éléments qui n'ont pas pu être géolocalisés.
Pour les éléments qui ne sont pas géolocalisables automatiquement (dont les informations
sont inconnues du SIG), il est possible de dessiner manuellement l'élément sur le SIG.
Pour cela, il faut se rendre directement sur :ref:`l'établissement<etablissement_geolocaliser>` ou le :ref:`dossier de coordination<dossiers_dc_geolocaliser>`.

.. image:: administration_geocoder-tous-success.png


Import
------

Ce module permet l'intégration de données dans l'application depuis des fichiers CSV.

Import des établissements
#########################

Les établissements peuvent être ajoutés depuis un fichier CSV. Un fichier CSV modèle est disponible sur le formulaire d'import.

.. image:: administration-form-import-etablissement.png

.. note::

  Il est nécessaire de mettre à jour manuellement la séquence de l'établissement lors de l'utilisation de cet import CSV.

.. note::

  Même lorsqu’un Système d’Information Géographique est paramétré les établissements ne sont pas géolocalisés automatiquement lors de l'import CSV. Les établissements restent géolocalisable depuis l'interface de géolocalisation de tous les établissements et des dossiers de coordination (voir :ref:`administration_geolocalisation` Géocoder tous). 


Générateur
----------

Ce module permet la génération d'éléments à partir du modèle de données.



