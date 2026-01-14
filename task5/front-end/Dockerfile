# On utilise Nginx comme base (plus léger et prêt à l'emploi)
FROM nginx:latest

# 1. On copie les fichiers du site web (le dossier cloné) vers le dossier standard des sites web dans le conteneur
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# 2. On copie notre fichier de configuration personnalisé pour remplacer celui par défaut de Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
