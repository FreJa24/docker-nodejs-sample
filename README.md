# ToDo-Applikation

Eine einfache ToDo-Applikation, die mit Node.js entwickelt wurde.

## Voraussetzungen

Um dieses Projekt lokal auszuführen, benötigst du:

- [Node.js](https://nodejs.org) (inkl. npm)
- [Git](https://git-scm.com/)

## Repository klonen

Klone das Repository mit folgendem Befehl:

\`\`\`bash
git clone https://github.com/FreJa24/docker-nodejs-sample
cd docker-nodejs-sample
\`\`\`

## Pakete installieren

Installiere die benötigten Node.js-Abhängigkeiten:

\`\`\`bash
npm install
\`\`\`

## Anwendung lokal starten

Starte die Anwendung im Entwicklungsmodus mit:

\`\`\`bash
npm run dev
\`\`\`

Die Anwendung ist anschliessend erreichbar unter:

**[http://localhost:3000](http://localhost:3000)**

## Docker-Image erstellen

Baue das Docker-Image mit folgendem Befehl:

\`\`\`bash
docker build -t todo-app .
\`\`\`

## Anwendung mit Docker starten

Starte einen Container aus dem Image:

\`\`\`bash
docker run --name todo-container -p 3000:3000 todo-app
\`\`\`

Die Anwendung ist danach erreichbar unter [http://localhost:3000](http://localhost:3000).

## Anwendung stoppen

\`\`\`bash
docker stop todo-container
docker rm todo-container
\`\`\`