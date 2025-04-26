Py Convert est un petit programme en Python qui automatise la conversion de fichiers .py en fichiers exécutables .exe sans avoir à saisir manuellement les commandes dans le terminal. Il simplifie le processus de création d'exécutables, rendant vos scripts Python prêts à être partagés et utilisés facilement sur n'importe quel système Windows.

Prérequis
Avant d'utiliser Py convert, assurez-vous d'avoir les éléments suivants :

Python installé sur votre machine.
Un éditeur de code (comme Visual Studio Code, PyCharm, etc.).
Pyinstaller 
Ouvrir le projet dans un éditeur de code :

Clonez ce dépôt ou téléchargez-le en tant que fichier ZIP et extrayez-le.
Ouvrez le dossier du projet dans votre éditeur de code préféré.
Configurer le chemin :

Avant d'exécuter le programme, vous devez spécifier le chemin vers votre script Python que vous souhaitez convertir,
 dans l'éditeur de code.
Recherchez la variable PYTHON_SCRIPT_PATH et définissez-la sur le chemin absolu de votre fichier
# Chemin vers le dossier où se trouve pyinstaller
PYINSTALLER_DIR = r"C:\Users\VotreNom\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.12_qbz5n2kfra8p0\LocalCache\local-packages\Python312\Scripts"
DIST_DIR = os.path.join(PYINSTALLER_DIR, "dist")

Installer les dépendances : https://github.com/Enjukar/Installateur-de-d-pendances/tree/main

Ouvrez un terminal dans votre éditeur de code.
Exécutez la commande suivante pour installer les dépendances nécessaires :
Copier
pip install -r requirements.txt
Utilisation
Exécuter le programme :

Dans le terminal, exécutez le script principal avec la commande suivante :
Copier
python main.py
Le programme générera un fichier exécutable .exe dans le même répertoire que votre script Python.
Partager votre exécutable :

Vous pouvez maintenant partager le fichier .exe généré avec d'autres utilisateurs Windows. Ils pourront exécuter votre programme sans avoir besoin d'installer Python.
Remarques
Assurez-vous que le chemin spécifié dans config.py est correct et pointe vers un fichier .py valide.
Ce programme est conçu pour fonctionner sur les systèmes Windows.
