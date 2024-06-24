
## Schritte

### 1. Virtuelle Umgebung erstellen

1. Öffne ein Terminal.
2. Navigiere zum Projektverzeichnis.
3. Führe den folgenden Befehl aus:

    ```
    python3 -m venv venv
    ```

### 2. Aktivieren der virtuellen Umgebung

Nachdem Sie die virtuelle Umgebung erstellt haben, muss sie aktiviert werden:

- **Mac/Linux**:

    ```
    source venv/bin/activate
    ```

- **Windows**:

    ```
    .\venv\Scripts\activate
    ```

### 3. Installieren der Abhängigkeiten

Installiere alle erforderlichen Pakete, die in der `requirements.txt`-Datei gelistet sind:

```
pip install -r requirements.txt
```

### 4. Starten des Frontends

Um die `index.html` unter `localhost:8006` verfügbar zu machen, führe den folgenden Befehl aus:

```
python3 -m http.server 8006
```

### 5. Starten des Backends

Um ein minimales Backend mit FastAPI zu starten, verwende folgenden Befehl.

```
uvicorn minimal_server:app --reload --port 8006
```
