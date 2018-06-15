# <a name="contribute-to-microsoft-graph-documentation"></a>Mitwirkung an der Microsoft Graph-Dokumentation

Vielen Dank für Ihr Interesse an der Microsoft Graph-Dokumentation!

- [Möglichkeiten zur Mitwirkung](#ways-to-contribute)
- [Bevor wir Ihre Pull-Anfrage annehmen können](#before-we-can-accept-your-pull-request)
- [Verwenden von GitHub, Git und diesem Repository](#use-github-git-and-this-repository)
- [Verwenden von Markdown zum Formatieren Ihres Themas](#how-to-use-markdown-to-format-your-topic)
- [Weitere Ressourcen](#more-resources)

## <a name="ways-to-contribute"></a>Möglichkeiten zur Mitwirkung

Sie können folgendermaßen an der [Microsoft Graph-Dokumentation](http://developer.microsoft.com/graph/docs) mitwirken:

- Wirken Sie an Artikeln über das [öffentliche Microsoft Graph-Entwicklerdokumentationsrepository](https://github.com/microsoftgraph/microsoft-graph-docs) mit
- Melden Sie Dokumentationsfehler über [GitHub-Probleme](https://github.com/microsoftgraph/microsoft-graph-docs/issues)
- Fügen Sie Dokumentationsanfragen zu [UserVoice der Office Developer-Plattform](http://officespdev.uservoice.com) hinzu

## <a name="before-we-can-accept-your-pull-request"></a>Bevor wir Ihre Pull-Anfrage annehmen können

### <a name="minor-corrections"></a>Kleinere Korrekturen

Kleinere Korrekturen oder Erläuterungen, die Sie für die Dokumentation und die Codebeispiele in diesem Repository einsenden, erfordern kein Lizenzvertrag für Mitwirkende (Contribution License Agreement, CLA). Beiträge werden in Form von Pull-Anfragen angenommen. Wir versuchen, Pull-Anfragen innerhalb von 10 Werktagen zu überprüfen.

### <a name="larger-submissions"></a>Größere Einsendungen

Wenn Sie neue oder erhebliche Änderungen an Dokumentation und Codebeispielen übermitteln möchten, müssen Sie einen Lizenzvertrag für Mitwirkende (Contribution License Agreement, CLA) unterzeichnen, bevor wir Ihre Pull-Anforderung annehmen können, wenn Sie in einer dieser Gruppen sind:

- Mitglieder der Microsoft Open Technologies-Gruppe
- Mitwirkende, die nicht für Microsoft arbeiten

Als Mitglied der Community **müssen Sie den Lizenzvertrag für Mitwirkende (CLA) unterzeichnen, bevor Sie umfangreiche Beiträge zu diesem Projekt leisten können**, aber Sie müssen die Dokumentation nur einmal ausfüllen und einsenden. Lesen Sie bitte aufmerksam das Dokument. Möglicherweise muss auch Ihr Arbeitgeber das Dokument unterzeichnen.

Durch das Unterzeichnen des Lizenzvertrags für Mitwirkende (CLA) erhalten Sie keine Zugriffsrechte auf das Hauptrepository, aber es bedeutet, dass die Microsoft-Teams in der Lage sind, Ihre Beiträge zu prüfen und überdenken. Falls das geschieht, werden Sie entsprechend genannt.

Sie können den Lizenzvertrag für Mitwirkende (CLA) [hier](https://cla.microsoft.com) herunterladen oder digital signieren. Sobald wir Ihren CLA erhalten und verarbeitet haben, versuchen wir, Ihre Pull-Anforderungen innerhalb von 10 Werktagen zu überprüfen.

## <a name="use-github-git-and-this-repository"></a>Verwenden von GitHub, Git und diesem Repository

**Hinweis:** Die meisten der Informationen in diesem Abschnitt finden Sie in [GitHub-Hilfeartikeln][].  Wenn Sie mit Git und GitHub vertraut sind, fahren Sie mit dem Abschnitt zum **Einsenden und Bearbeiten von Inhalten** mit speziellen Informationen zum Code-/Inhaltsfluss dieses Repositorys fort.

### <a name="setting-up-your-fork-of-the-repository"></a>Einrichten Ihrer Verzweigung des Repositorys

1. Richten Sie ein GitHub-Konto ein, damit Sie an diesem Projekt mitwirken können. Wechseln Sie dazu, falls noch nicht geschehen, zur [GitHub-Startseite][].
2. Richten Sie Ihren Computer mit Git ein. Folgen Sie den Anweisungen im [Lernprogramm zum Einrichten von Git][Set Up Git].
3. Erstellen Sie Ihre eigene Verzweigung dieses Repositorys. Klicken Sie dazu oben auf der Seite auf die Schaltfläche **Verzweigung**.
4. Kopieren Sie die Verzweigung auf Ihren lokalen Computer. Öffnen Sie hierzu Git Bash. Geben Sie an der Eingabeaufforderung Folgendes ein:

```cmd
git clone https://github.com/{your user name}/microsoft-graph-docs.git
```

Erstellen Sie danach einen Verweis auf das Stammrepository durch Eingabe der folgenden Befehle:

```cmd
cd microsoft-graph-docs
git remote add upstream https://github.com/microsoftgraph/microsoft-graph-docs.git
git fetch upstream
```

Ausgezeichnet. Sie haben nun Ihr Repository eingerichtet. Sie müssen diese Schritte nicht erneut ausführen.

### <a name="contribute-and-edit-content"></a>Einsenden und Bearbeiten von Inhalten

Um die Mitwirkung für Sie so einfach wie möglich zu machen, führen Sie dieses Verfahren aus.

1. Erstellen Sie eine neue Verzweigung.
1. Fügen Sie neue Inhalte hinzu, oder bearbeiten Sie vorhandene Inhalte.
1. Senden Sie eine Pull-Anforderung an das Hauptrepository.
1. Löschen Sie die Verzweigung.

Begrenzen Sie jede Verzweigung  auf ein einzelnes Konzept bzw. einen einzelnen Artikel, um den Workflow zu optimieren und das Risiko von Zusammenführungskonflikten zu verringern. Die folgenden Arten von Beiträgen eignen sich für eine neue Verzweigung:

- Ein neuer Artikel (und die zugehörigen Bilder)
- Bearbeitung von Rechtschreibung und Grammatik für einen Artikel
- Vornehmen einer einzelnen Formatierungsänderung für eine große Gruppe von Artikeln (z. B. Übernehmen einer neuen Copyright-Fußzeile).

#### <a name="create-a-new-branch"></a>Erstellen einer neuen Verzweigung.

1. Öffnen Sie GitBash.
1. Geben Sie `git pull upstream master:<new branch name>` an der Eingabeaufforderung ein. Dadurch wird eine neue Verzweigung lokal erstellt, die aus der neuesten *Microsoft Graph*-Hauptverzweigung kopiert wird. **Hinweis:** Interne Mitwirkende ersetzen `master` im Befehl mit der Verzweigung für das anvisierte Veröffentlichungsdatum.
1. Geben Sie `git push origin <new branch name>` an der Eingabeaufforderung ein. Dadurch wird GitHub auf die neue Verzweigung hingewiesen. Die neue Verzweigung sollte nun in Ihrer Verzweigung des Repository auf GitHub angezeigt werden.
1. Geben Sie `git checkout <new branch name>` ein, um zur neuen Verzweigung zu wechseln.

#### <a name="add-new-content-or-edit-existing-content"></a>Hinzufügen neuer Inhalte oder Bearbeiten vorhandener Inhalte

Zum Bearbeiten von Dateien öffnen Sie sie in einem Editor Ihrer Wahl und ändern sie. Um eine neue Datei zu erstellen, verwenden Sie den Editor Ihrer Wahl, und speichern Sie die neue Datei im entsprechenden Speicherort in Ihrer lokalen Kopie des Repositorys. Speichern Sie während der Bearbeitung häufig.

Die Dateien auf Ihrem lokalen Computer sind eine Arbeitskopie der neuen Verzweigung, die Sie in Ihrem lokalen Repository erstellt haben. Änderungen in diesem Ordner wirken sich erst auf das lokale Repository aus, wenn Sie eine Änderung übernehmen. Um eine Änderung am lokalen Repository zu übernehmen, geben Sie die folgenden Befehle in GitBash ein:

```cmd
git add .
git commit -v -a -m "<Describe the changes made in this commit>"
```

Der `add`-Befehl fügt Ihre Änderungen einem Stagingbereich als Vorbereitung für die Aufnahme im Repository hinzu. Der Punkt nach dem `add`-Befehl gibt an, dass Sie alle Dateien, die Sie hinzugefügt oder geändert haben, übernehmen möchten und dass Unterordner rekursiv überprüft werden sollen. (Wenn Sie nicht alle Änderungen übernehmen möchten, können Sie bestimmte Dateien hinzufügen. Sie können den Vorgang auch rückgängig machen. Falls Sie Hilfe benötigen, geben Sie `git add -help` oder `git status` ein.)

Der Befehl `commit` wendet die bereitgestellten Änderungen auf das Repository an. Die Option `-m` bedeutet, dass Sie den Commit-Kommentar in der Befehlszeile angeben. Wenn Sie kein bestimmtes Datum für die Veröffentlichung anvisieren, können Sie "Veröffentlichung so bald wie möglich" eingeben.  Die Optionen -v und -a können weggelassen werden. Die Option -v ist für die ausführliche Ausgabe des Befehls, und -a entspricht in ihrer Funktion den bereits verwendeten Befehl zum Hinzufügen.)

Sie können während der Arbeit mehrfach übernehmen oder warten und erst nach Abschluss der Arbeit übernehmen.

#### <a name="submit-a-pull-request-to-the-main-repository"></a>Einsenden einer Pull-Anforderung an das Hauptrepository

Wenn Sie Ihre Arbeit abgeschlossen haben und bereit sind, sie mit dem zentralen Repository zusammenzuführen, gehen Sie folgendermaßen vor.

1. Geben in GitBash an der Eingabeaufforderung `git push origin <new branch name>` ein. Im lokalen Repository bezieht sich `origin` auf Ihr GitHub-Repository, aus dem Sie das lokale Repository geklont haben. Mit diesem Befehl wird der aktuelle Status Ihrer neuen Verzweigung, einschließlich aller im vorherigen Schritt vorgenommenen Commits, in Ihre GitHub-Verzweigung übertragen.
2. Navigieren Sie auf der GitHub-Website in Ihrer Verzweigung zur neuen Verzweigung.
3. Klicken Sie oben auf der Seite auf die Schaltfläche **Pull anfordern**.
4. Stellen Sie sicher, dass die untere Verzweigung `microsoftgraph/microsoft-graph-docs@master` und die obere Verzweigung `<your username>/microsoft-graph-docs@<branch name>` lautet.
5. Klicken Sie auf die Schaltfläche **Commitbereich aktualisieren**.
6. Geben Sie Ihrer Pull-Anforderung einen Titel, und beschreiben Sie alle Änderungen, die Sie vornehmen. Wenn Ihr Beitrag ein Problem mit einem UserVoice-Element oder GitHub-Element behebt, verweisen Sie auf dieses Problem in der Beschreibung.
7. Senden Sie die Pull-Anforderung.

Eine der Websiteadministratoren wird nun Ihre Pull-Anforderung verarbeiten. Ihre Pull-Anforderung wird auf der Oberfläche der Website microsoftgraph/microsoft-graph-docs unter Probleme angezeigt. Wenn die Pull-Anforderung angenommen wird, wird das Problem gelöst.

#### <a name="create-a-new-branch-after-merge"></a>Erstellen einer neuen Verzweigung nach dem Zusammenführen

Nachdem eine Verzweigung erfolgreich zusammengeführt wurde (d. h. Ihre Pull-Anforderung wurde angenommen), arbeiten Sie nicht in der lokalen Verzweigung weiter, die erfolgreich zusammengeführt wurde. Dies kann zu Zusammenführungskonflikten führen, wenn Sie eine weitere Pull-Anforderung einsenden. Wenn Sie eine weitere Aktualisierung vornehmen möchten, erstellen Sie stattdessen eine neue lokale Verzweigung aus der erfolgreich zusammengeführten übergeordneten Verzweigung.

Nehmen Sie z. B. an, dass Ihre lokale Verzweigung X erfolgreich mit der Hauptverzweigung microsoftgraph/microsoft-graph-docs zusammengeführt wurde und dass Sie die zusammengeführten Inhalte weiter aktualisieren möchten. Erstellen Sie eine neue lokale Verzweigung X2 aus der Hauptverzweigung microsoftgraph/microsoft-graph-docs. Öffnen Sie dazu GitBash, und führen Sie die folgenden Befehle aus:

```cmd
cd microsoft-graph-docs
git pull upstream master:X2
git push origin X2
```

Sie haben nun lokale Kopien (in einer neuen lokalen Verzweigung) der Arbeit, die Sie in Verzweigung X übermittelt haben. Die X2-Verzweigung enthält auch alle Arbeiten, die andere Autoren zusammengeführt haben. Wenn Ihre Arbeit also von der anderer Personen abhängt (z. B. freigegebene Bilder), ist sie in der neuen Verzweigung verfügbar. Sie können feststellen, ob sich Ihre vorherige Arbeit (und die anderer Personen) in der Verzweigung befindet, indem Sie die neue Verzweigung überprüfen ...

```cmd
git checkout X2
```

... und den Inhalt verifizieren. Der `checkout`-Befehl aktualisiert die Dateien auf dem Datenträger auf den aktuellen Status der X2-Verzweigung.
Sobald Sie die neue Verzweigung überprüft haben, können Sie Aktualisierungen am Inhalt vornehmen und wie gewohnt übernehmen.
Um aber zu vermeiden, dass Sie versehentlich in der zusammengeführten Verzweigung (X) arbeiten, empfiehlt es sich, sie zu löschen (Informationen finden Sie im folgenden Abschnitt **Löschen einer Verzweigung**).

#### <a name="delete-a-branch"></a>Löschen einer Verzweigung

Nachdem Ihre Änderungen erfolgreich mit dem zentralen Repository zusammengeführt wurden, können Sie die verwendete Verzweigung löschen, da Sie sie nicht mehr benötigen. Jede zusätzliche Arbeit erfordert eine neue Verzweigung.

Zum Löschen der Verzweigung gehen Sie folgendermaßen vor:

1. Geben in GitBash an der Eingabeaufforderung `git checkout master` ein.  Dadurch wird sichergestellt, dass Sie sich nicht in der zu löschenden Verzweigung befinden (das ist nicht zulässig).
2. Geben Sie dann `git branch -d <branch name>` in der Befehlszeile ein.  Dadurch wird die Verzweigung auf dem lokalen Computer nur dann gelöscht, wenn sie erfolgreich mit dem übergeordneten Repository zusammengeführt wurde. (Sie können dieses Verhalten mit dem `–D`-Flag außer Kraft setzen, allerdings sollten Sie sich in diesem Falle wirklich sicher sein.)
3. Geben Sie schließlich `git push origin :<branch name>` an der Befehlszeile ein (ein Leerzeichen vor dem Doppelpunkt, kein Leerzeichen dahinter).  Dadurch wird die Verzweigung in Ihrer Github-Verzweigung gelöscht.

Herzlichen Glückwunsch, Sie haben erfolgreich am Projekt mitgewirkt.

## <a name="how-to-use-markdown-to-format-your-topic"></a>Verwenden von Markdown zum Formatieren Ihres Themas

### <a name="standard-markdown"></a>Standard-Markdown

Alle Artikel in diesem Repository verwenden Markdown.  Während Sie eine vollständige Einführung (und eine Auflistung der gesamten Syntax) auf der [Markdown-Homepage] [] finden, behandeln wir hier die zentralen Grundlagen.

Wenn Sie nach einem guten Editor suchen, versuchen Sie [Visual Studio Code][vscode].

### <a name="markdown-basics"></a>Markdown- Grundlagen

Dies ist eine Liste der am häufigsten verwendeten Markdown-Syntax:

- **Zeilenumbrüche und Absätze:** In Markdown gibt es kein HTML-`<br />`-Element. Stattdessen wird ein neuer Absatz durch eine leere Zeile zwischen zwei Textblöcke gekennzeichnet.
- **Kursiv:** Das HTML-Element `<i>some text</i>` wird als `*some text*` geschrieben
- **Fett:** Das HTML-Element `<strong>some text</strong>` wird als `**some text**` geschrieben
- **Überschriften:** HTML-Überschriften werden von einigen `#`-Zeichen am Anfang der Zeile gekennzeichnet.  Die Anzahl der `#`Zeichen entspricht der hierarchischen Ebene der Überschrift (z. B. `#` = h1, `##` = h2 und `###` = h3).
- **Nummerierte Listen:** Um eine nummerierte (sortierte) Liste zu erstellen, beginnen Sie die Zeile mit `1. `. Wenn Sie mehrere Elemente in einem einzelnen Listenelement verwenden möchten, formatieren Sie die Liste wie folgt:

    1. Beachten Sie das Leerzeichen nach dem „.“

       Beachten Sie auch, dass zwischen den beiden Absätzen im Listenelement ein Zeilenumbruch ist, und dass der Einzug hier dem Einzug der Zeile oben entspricht.

- **Aufzählungen:** Aufzählungen (nicht sortiert) sind fast identisch mit sortierten Listen, abgesehen davon, dass `1. ` durch `- `, `* ` oder `+ ` ersetzt wird.  Mehrere Elementlisten funktionieren genauso wie sortierte Listen.
- **Links:** Die grundlegende Syntax für einen Link ist `[visible link text](link url)`.
  Links können auch Verweise enthalten, was im Abschnitt **Link- und Bildverweise** weiter unten erläutert wird.
- **Bilder:** Die grundlegende Syntax für ein Bild ist `![alt text for the image](image url)`.
  Bilder können auch Verweise enthalten, was im Abschnitt **Link- und Bildverweise** weiter unten erläutert wird.
- **Inline-HTML:** Mit Markdown können Sie HTML inline einschließen, dies sollte jedoch vermieden werden.

### <a name="link-and-image-references"></a>Link- und Bildverweise

In Markdown gibt es eine nützliche Funktion, mit der ein Benutzer einen Verweis anstelle einer URL für Bilder und Links einfügen kann. So sieht die Syntax für diese Funktion aus:

```markdown
The image below is from [Google][googleweb]

![Google's logo][logo]

[googleweb]: http://www.google.com
[logo]: https://www.google.com/images/srpr/logo3w.png
```

Mithilfe von Verweisen, die am Ende Ihrer Datei gruppiert werden, können Sie Link- und Bild-URLs ganz einfach finden, bearbeiten und wiederverwenden.

## <a name="more-resources"></a>Weitere Ressourcen

- Weitere Informationen zu Markdown finden Sie auf [der Website][Markdown-Homepage].
- Weitere Informationen zur Verwendung von Git und GitHub finden Sie im [GitHub-Hilfeabschnitt] [GitHub-Hilfe]. Sie können sich auch an die Websiteadministratoren wenden.

[GitHub-Homepage]: http://github.com
[GitHub-Hilfe]: http://help.github.com/
[Set Up Git]: http://help.github.com/win-set-up-git/
[Markdown-Homepage]: http://daringfireball.net/projects/markdown/
[vscode]: https://code.visualstudio.com/
