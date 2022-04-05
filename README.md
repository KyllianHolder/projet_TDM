# projet_TDM

Lancer le projet : 

Installation
Exécutez les commandes suivantes sur vos machines virtuelles

pip

Pour installer pip, vous devez exécuter les commandes suivantes sur votre terminal :

Note : Veuillez noter que toutes les lignes commençant par "$" doivent être exécutées sur le terminal.

$ sudo apt update

$ sudo apt install python3-dev

$ sudo apt install python3-pip

Installation de virtualenv

$ sudo apt install virtualenv

Installation dans virtualenv

$ virtualenv --system-site-packages -p python3 env

$ source env/bin/activate

Installation de Jupyter

$ python3 -m pip install --upgrade --force-reinstall  --no-cache jupyter

Installation de scikit-learn

$ python3 -m pip install scikit-learn

Installation de numpy

$ python3 -m pip install numpy

Installation de pandas

$ python3 -m pip install pandas

Installation de matplotlib

$ python3 -m pip install matplotlib

Installation Git for Python 

$ pip install gitpython

$ jupyter notebook


1.  Collection de données 
    Systeme de recommandation : spotify, youtube, ...
    Mais d'images ! 
    On utilise Kaggle, on automise la collection :
    Faire une fonction git clone pour choper les images?


2. 

Différence entre algo classificiation et kamins :
kamins n'a pas la notion de aime ou aime pas
algo supervisé et non supervisé, j'ai des données masi j'ai peu d'infos, mais je veux quamdeme trouver des objets similaires 
