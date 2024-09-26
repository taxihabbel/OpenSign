FROM node:18

# Erstelle Arbeitsverzeichnis
WORKDIR /app

# Kopiere package.json und installiere Abhängigkeiten
COPY package*.json ./
RUN npm install --only=production

# Kopiere den Rest des Projekts
COPY . .

# Setze die Umgebungsvariablen
ENV NODE_ENV=production

# Exponiere den Port
EXPOSE 8080

# Startbefehl
CMD ["npm", "start"]
