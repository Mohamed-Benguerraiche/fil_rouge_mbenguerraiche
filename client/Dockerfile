# Utilisez l'image Node.js en tant qu'image de base
FROM node

# Définissez le répertoire de travail dans le conteneur
WORKDIR /usr/src/app

# Copiez le fichier package.json et package-lock.json dans le conteneur
COPY client/package*.json ./

# Installez les dépendances
RUN npm install

# Copiez tous les fichiers du projet dans le conteneur
COPY client/ .

# Exposez le port correspondant au service
EXPOSE 3000

# Commande de démarrage du service
CMD ["npm", "start"]
