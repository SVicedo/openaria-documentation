
.. _tests_ci:

#############################
Tests et Intégration Continue
#############################


openARIA possède des tests unitaires et fonctionnels joués intégralement à chaque modification du code source afin d'assurer sa stabilité et sa pérennité. 
Tous les tests sont présents dans le répertoire tests/. Deux frameworks de test sont utilisés : RobotFramework et PHPUnit. http://docs.openmairie.org/?project=framework&path=tests_ci/



Écrire un TestSuite RobotFramework
##################################


Créer le fichier exemple.robot dans le répertoire tests/.


Copier/Coller le code suivant dans le fichier créé :

.. code::

    *** Settings ***
    Resource  resources/resources.robot
    Suite Setup  For Suite Setup
    Suite Teardown  For Suite Teardown
    Documentation  La programmations des visites...


    *** Test Cases ***
    Exemple de testcase

        Depuis la page d'accueil  admin  admin
        Log  Je suis authentité en tant qu'utilisateur 'admin'



Exécuter la commande :

.. code:: bash

    ./om-tests -c runone -t exemple.robot


Ressources
##########


Les ressources sont des librairies de mots-clés RobotFramework. 


Voici la documentation des librairies spécifiques à openARIA :

Librairie de l'application openARIA `App <https://scm.adullact.net/anonscm/svn/openaria/trunk/tests/doc/app.html>`_.

.. raw:: html

   <iframe src="https://scm.adullact.net/anonscm/svn/openaria/trunk/tests/doc/app.html" width="100%" height="500px"></iframe>


Librairie du framework openMairie `Core <https://scm.adullact.net/anonscm/svn/openaria/trunk/tests/doc/core.html>`_.

.. raw:: html

   <iframe src="https://scm.adullact.net/anonscm/svn/openaria/trunk/tests/doc/core.html" width="100%" height="500px"></iframe>


Voici les documentations des librairies génériques utilisées par openARIA :

- Base - BuiltIn : http://robotframework.org/robotframework/latest/libraries/BuiltIn.html
- Base - String : http://robotframework.org/robotframework/latest/libraries/String.html
- Base - Collections : http://robotframework.org/robotframework/latest/libraries/Collections.html
- Base - OperatingSystem : http://robotframework.org/robotframework/latest/libraries/OperatingSystem.html
- Selenium2 : http://rtomac.github.io/robotframework-selenium2library/doc/Selenium2Library.html
- Requests : http://bulkan.github.io/robotframework-requests/
- Selenium2Screenshots : https://robotframework-selenium2screenshots.readthedocs.org/en/latest/_downloads/keywords.html
  


