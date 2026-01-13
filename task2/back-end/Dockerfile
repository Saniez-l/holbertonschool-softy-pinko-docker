# On part toujours d'Ubuntu
FROM ubuntu:latest

# Mise à jour
RUN apt-get update
RUN apt-get upgrade -y

# Installation de Python et PIP (le gestionnaire de paquets python)
RUN apt-get install -y python3 python3-pip

# CORRECTION DU BUG "EXTERNALLY-MANAGED"
# Cette ligne est obligatoire sur les nouvelles versions d'Ubuntu pour autoriser pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Installation de Flask via pip3
RUN pip3 install flask

# On définit le dossier de travail dans le conteneur
WORKDIR /app

# On copie ton fichier api.py (de ton PC) vers le dossier /app (dans le conteneur)
COPY ./api.py /app/api.py

# La commande qui se lance au démarrage : on lance le script python
CMD ["python3", "api.py"]