
# Bitcoin Alps Website

Diese README-Datei erklärt, wie Hugo, das Blowfish-Theme und das Hugo Modules Feature zur Verwaltung von Themes und anderen Abhängigkeiten für die Bitcoin Alps-Website installiert und verwendet werden. Sie zeigt auch, wie einen lokalen Entwicklungsserver gestartet und eine produktionsreife Version der Website für das Deployment generieren werden kann.

## Lokale Installation

1. Installiere Hugo:

    ```bash
    # macOS
    brew install hugo

    # Windows
    choco install hugo -confirm

    # Linux
    sudo apt install hugo
    ```

2. Klone das Github-Repository:

    ```bash
    git clone https://github.com/bitcoin-alps/bitcoin-alps.ch.git
    ```

## Entwicklung

1. Starte einen lokalen Entwicklungsserver:

    ```bash
    hugo server
    ```

2. Öffne deinen Browser und gehe zu [http://localhost:1313], um deine Website anzusehen.

3. Sobald du Änderungen an deinen Inhalten und Vorlagen vornimmst, wird die Website automatisch neu aufgebaut und die Änderungen werden im Browser widergespiegelt.

## Kontinuierliches Deployment mit Cloudflare Pages

Wir verwenden Cloudflare Pages als vereinfachte Möglichkeit, die Bereitstellung der Hugo-Website jedes Mal zu automatisieren, wenn Änderungen an unserem Repository vorgenommen werden. Dies bedeutet, dass Cloudflare Pages die Site automatisch aus der Quelle erstellt und die aktualisierte Version im Web bereitstellt, wenn ein Commit in den Master-Zweig dieses Repositorys eingebunden wird.

## Beitrag zu unserer Website

Wir leben den Open-Source-Geist, ganz wie das Ethos hinter Bitcoin, im Glauben, dass Zusammenarbeit und Transparenz zu besseren und innovativeren Ergebnissen führen. Alle ist willkommen, zu unserer Website beizutragen, und dies ist unkompliziert möglich – durch das Einreichen eines Pull Requests.

### Was ist ein Pull Request?

Ein Pull Request ist eine Möglichkeit, Änderungen an einem Repository vorzuschlagen, das auf Plattformen wie GitHub gehostet wird. Es ermöglicht dir, den vorhandenen Code zu nehmen, auf deinem eigenen Branch zu ändern und dann die Repository-Betreuer (uns) zu bitten, deine Änderungen in den Hauptcode einzufügen. 

### Wie man beiträgt

1. **Fork das Repository:** Zuerst erstelle einen Fork des Repositorys unserer Website. Diese Aktion kopiert das Repository auf deinen GitHub-Account und ermöglicht es dir, unabhängig Änderungen vorzunehmen.
2. **Mache deine Änderungen:** Klone das Repository von deinem Account auf deinen lokalen Rechner und nimm die gewünschten Änderungen vor. Ob es darum geht, einen Tippfehler zu korrigieren, Inhalte hinzuzufügen oder das Design zu verbessern, deine Beiträge sind wertvoll.
3. **Commit und Push:** Nachdem du deine Änderungen vorgenommen hast, committe sie zu deinem Branch und pushe die Änderungen zurück zu deinem GitHub-Repository.
4. **Erstelle einen Pull Request:** Navigiere zum ursprünglichen Repository, von dem du geforkt hast. Du solltest eine Option sehen, um einen "Pull Request" basierend auf den Änderungen, die du zu deinem Repository gepusht hast, zu erstellen. Fülle die Details aus, erkläre, was du geändert hast und warum, und reiche die Anfrage ein.

Wir werden deinen Beitrag überprüfen, möglicherweise um Anpassungen bitten, und wenn alles gut aussieht, deine Änderungen in den Hauptzweig mergen. Dein Beitrag wird dann Teil der Website sein, sichtbar und zugänglich für alle.

## Hugo-Template aktualisieren

Das "Blowfish"-Theme wird regelmäßig mit neuen Funktionen und Fixes aktualisiert. Das Theme kann mit folgendem befehl auf die neueste Version aktualisiert werden:

```bash
hugo mod get -u
```