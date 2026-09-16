# Docker Node.js ToDo-App

Eine einfache ToDo-Anwendung mit Node.js, die in einem Docker-Container ausgeführt wird.

## Installation

### 1. Repository klonen

Repository von GitHub klonen:

```bash
git clone https://github.com/joelkapoor720/docker-nodejs-joel.git
cd docker-nodejs-joel
```

### 2. Abhängigkeiten installieren

Node.js muss installiert sein.

Die benötigten Abhängigkeiten werden mit folgendem Befehl installiert:

```bash
npm install
```

### 3. Docker installieren

Installiere Docker Desktop und stelle sicher, dass Docker Desktop läuft.

Überprüfe die Docker-Installation mit:

```bash
docker --version
```

Zusätzlich kann Docker mit folgendem Befehl getestet werden:

```bash
docker run hello-world
```

### 4. Docker-Image erstellen

Im Projektordner wird das Docker-Image mit dem `Dockerfile` erstellt:

```bash
docker build -t docker-nodejs-joel .
```

### 5. Docker-Container starten

Starte anschließend einen Container mit:

```bash
docker run --name todo-app -p 3000:3000 docker-nodejs-joel
```

Die Anwendung läuft danach im Docker-Container.

### 6. Anwendung öffnen

Öffne im Browser:

```text
http://localhost:3000
```

Dort kann die ToDo-Anwendung verwendet werden.

### 7. Laufenden Container überprüfen

Mit folgendem Befehl kann überprüft werden, ob der Container läuft:

```bash
docker ps
```

Der Container sollte den Namen `todo-app` haben und den Port `3000` verwenden.

### 8. Container stoppen

Um den Container zu stoppen:

```bash
docker stop todo-app
```

Um den Container später wieder zu starten:

```bash
docker start todo-app
```
