# 1. On définit l'image de base (OS)
FROM ubuntu:latest

# 2. On exécute les commandes de mise à jour
# On met à jour la liste des paquets
RUN apt-get update

# On installe les nouvelles versions des paquets installés
# Le flag "-y" est CRUCIAL pour dire "Oui" automatiquement aux invites
RUN apt-get upgrade -y

# 3. La commande qui se lance au démarrage du conteneur
CMD ["echo", "Hello, World!"]