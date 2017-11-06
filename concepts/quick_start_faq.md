# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph-Schnellstart – Häufig gestellte Fragen

In den häufig gestellten Fragen werden Fragen im Zusammenhang mit den [Microsoft Graph-Schnellstarts](https://developer.microsoft.com/en-us/graph/quick-start) beantwortet.

## <a name="what-do-the-quick-starts-do"></a>Welche Funktionen haben die Schnellstarts?

Die Schnellstart-Beispiele zeigen, wie Sie die Leistungsfähigkeit von Microsoft Graph nutzen können. 

Wenn Sie die Office 365-REST-APIs verwenden, müssen Sie sich bei jedem Dienst, den Sie aufrufen möchten, authentifizieren. Bei Microsoft Graph wird diese Komplexität beseitigt, indem die Authentifizierung vereinheitlicht wird und Sie Zugriff auf alle APIs über einen einzigen Einstiegspunkt erhalten. Sie können sich einmal authentifizieren und auf Informationen in mehreren Anwendungen und Diensten zugreifen. 

Die Microsoft Graph-Schnellstarts greifen mit einer Authentifizierung auf drei Dienste zu: Microsoft-Konto, OneDrive und Outlook. Bei jedem Schnellstart werden Informationen aus Benutzerprofilen von Microsoft-Konten abgerufen. Diese Daten (ein Foto) werden auf OneDrive geschrieben, und dann wird in Outlook eine E-Mail (mit einem Link zu dem Foto) generiert. 

Die Schnellstarts umfassen vier Schritte:
- Wählen Sie Ihre Plattform. 
- Rufen Sie Ihre App-ID (auch bekannt als Client-ID) ab.
- Erstellen Sie das Beispiel.
- Melden Sie sich an, und versenden Sie ein Profilfoto per E-Mail.

Wenn Sie den Schnellstart abgeschlossen haben, ist ihre App fertig.


## <a name="general-quick-start-sample-questions"></a>Allgemeine Schnellstart-Beispielfragen
In diesem Abschnitt werden Fragen zu der Organisation und zu Inhalten der Schnellstart-Beispiele beantwortet.

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>Warum enthält mein Schnellstart eine Readme-Datei?

Jeder Schnellstart registriert eine neue Anwendung und erstellt eine Zip-Datei, die den Inhalt eines GitHub-Repositorys enthält. Die Dateien im Repository werden aktualisiert, damit Sie die Beispielanwendung im Repository nicht konfigurieren müssen. Sie finden diese Repositorys in der [MicrosoftGraph-Organisation](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) auf GitHub.

Sie können sich die mit Schnellstarts verknüpften Repositorys gerne ansehen und Probleme melden, oder Sie befolgen die Anweisungen in der Readme-Datei zum Registrieren Ihrer eigenen Anwendung. Folgen Sie dem Link zum **Abfragen des Beispielcodes** unter Schritt 2 jedes Schnellstarts, um das Repository aufzurufen.

### <a name="which-microsoft-graph-features-do-the-quick-start-samples-use"></a>Welche Funktionen von Microsoft-Graph werden in den Schnellstart-Beispielen verwendet?

Die Schnellstart-Beispiele werden ständig aktualisiert. Um die Updates zu erhalten, sehen Sie sich das Repository für das gewünschte Beispiel an. Wenn Features hinzugefügt werden, aktualisieren wir die Beispiel-Readme-Datei mit den neuen Informationen. In der folgenden Tabelle sind die aktuellen Funktionen jedes Beispiels aufgeführt.
 +<!-- Replace the check mark images with an actual character that can be read by a screen reader. Or you could add alt text to each instance of the image. -->

|Beispiel|Authentifizieren|Profilfoto abrufen|Foto auf OneDrive hochladen|Link per E-Mail freigeben|Foto an E-Mail anhängen|E-Mail senden|
|-----:|-----:|-----:|------:|------:|------:|-----:|
|[Android Connect](https://github.com/microsoftgraph/android-java-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Angular 2 Connect](https://github.com/microsoftgraph/angular-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Angular 2 Connect REST](https://github.com/microsoftgraph/angular2-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[ASP.NET Connect](https://github.com/microsoftgraph/aspnet-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect - Swift](https://github.com/microsoftgraph/ios-swift-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect REST - Ziel C](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|[](./images/Check.PNG)|
|[Node.js Connect REST](https://github.com/microsoftgraph/nodejs-connect-rest-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)| |![](./images/Check.PNG)|
|[PHP Connect REST](https://github.com/microsoftgraph/php-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[PHP Connect](https://github.com/microsoftgraph/php-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Ruby Connect REST](https://github.com/microsoftgraph/ruby-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[UWP Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Xamarin Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|

## <a name="authentication-and-authorization"></a>Authentifizierung und Autorisierung
In diesem Abschnitt werden Fragen im Zusammenhang mit Authentifizierungs- und Autorisierungsproblemen beantwortet. 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Warum sind in den Schnellstart-Beispielen keine Anwendungsfälle für die erweiterte Authentifizierung enthalten?

Die Schnellstart-Beispiele bieten Ihnen eine Einführung in die Authentifizierung und Microsoft Graph-API-Aufrufe. Wenn Sie die Authentifizierung und Microsoft Graph-API-Aufrufe zu Ihrer Produktionsanwendung hinzufügen, müssen Sie wissen, wie Sie diese im Hinblick auf Sicherheit und bedingte Zugriffsprobleme für erweiterte Authentifizierungsszenarien entwickeln.

Weitere Informationen zu erweiterten Authentifizierungsszenarien für die verwendete Authentifizierungsbibliothek finden Sie auf der Seite des Publishers der Authentifizierungsbibliothek.

- [OAuth2Client für Android und iOS](https://github.com/nxtbgthng/OAuth2Client)
- [Passport für Node](http://passportjs.org/)
- [Illuminate Auth für PHP](https://github.com/illuminate/auth)
- [Flask für Python 3](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [OmniAuth für Ruby](https://github.com/omniauth/omniauth)
- [Microsoft Authentication Library (MSAL) für .NET](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [Microsoft Authentication Library für Android](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [Microsoft Authentication Library für JavaScript](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>Microsoft Graph-API
In diesem Abschnitt werden Fragen zu Codierungsanwendungen beantwortet, die Microsoft Graph-APIs verwenden.

### <a name="i-didnt-get-an-email-and-i-dont-see-any-errors-or-exceptions-why-didnt-this-work"></a>Ich habe keine E-Mail erhalten, und es werden keine Fehler oder Ausnahmen angezeigt. Warum hat es nicht funktioniert?

Wenn das Beispiel augenscheinlich eine E-Mail sendet, aber sie nicht in Ihrem Posteingang angezeigt wird, überprüfen Sie den Junk-E-Mail- oder Spam-Ordner. Wenn Sie die Nachricht von einem Testmandanten senden, wird die Nachricht möglicherweise als Spam gekennzeichnet.

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>Warum enthält die Beispiel-E-Mail nicht mein Profilbild?

Möglicherweise wurde Ihr Profil nicht mit einem Profilbild eingerichtet. Wenn Sie mit einem Microsoft angemeldet sind, erscheint das Profilbild auch dann nicht, wenn Sie eines besitzen. Die Microsoft Graph-API unterstützt derzeit keine Benutzerprofilbilder von Microsoft-Konten. Die meisten Schnellstart-Beispiele rufen Ihr Profilbild ab und laden es in das Stammverzeichnis Ihres OneDrive-Kontos hoch. Wenn Sie sich mit einem Microsoft-Konto (live.com, hotmail.com) anmelden, kann Microsoft Graph Ihr Profilbild aktuell nicht abrufen. Daher greifen wir auf das Bild mit der Gedankenblase zurück.

In den Node iOS Objective C-Beispielen werden keine Benutzerprofilbilder an die E-Mail-Nachricht angehängt. 

## <a name="aspnet"></a>ASP.NET
In diesem Abschnitt werden Fragen zum Programmieren, Erstellen oder Ausführen des ASP.NET-Schnellstart-Beispiels beantwortet.

### <a name="why-wont-my-aspnet-project-build"></a>Warum wird mein ASP.NET-Projekt nicht erstellt?
Wenn ein Beispiel, das .NET-Bibliotheken verwendet, nicht in Visual Studio erstellt wird, überschreitet eines oder mehrere Ihrer Projekte eventuell die Windows-Pfadlängenbeschränkung von 260 Zeichen. Versuchen Sie, die Lösung zu einem Speicherort im oder in der Nähe des Stammverzeichnisses zu verschieben. 

## <a name="universal-windows-platform-uwp"></a>Universelle Windows-Plattform (UWP)
In diesem Abschnitt werden Fragen zum Programmieren, Erstellen oder Ausführen des UWP-Schnellstart-Beispiels beantwortet.

### <a name="why-wont-my-uwp-project-build"></a>Warum wird mein UWP-Projekt nicht erstellt?
Wenn ein Beispiel, das .NET-Bibliotheken verwendet, nicht in Visual Studio erstellt wird, überschreitet eines oder mehrere Ihrer Projekte eventuell die Windows-Pfadlängenbeschränkung von 260 Zeichen. Versuchen Sie, die Lösung zu einem Speicherort im oder in der Nähe des Stammverzeichnisses zu verschieben. 

## <a name="xamarin"></a>Xamarin
In diesem Abschnitt werden Fragen zum Programmieren, Erstellen oder Ausführen des Xamarin-Schnellstart-Beispiels beantwortet.

### <a name="why-wont-my-xamarin-project-build"></a>Warum wird mein Xamarin-Projekt nicht erstellt?

Wenn ein Beispiel, das .NET-Bibliotheken verwendet, nicht in Visual Studio erstellt wird, überschreitet eines oder mehrere Ihrer Projekte eventuell die Windows-Pfadlängenbeschränkung von 260 Zeichen. Insbesondere bei Xamarin-Lösungen tritt dies häufig auf, vor allen Dingen bei Android-Projekten innerhalb von Xamarin Lösungen. Versuchen Sie, die Lösung zu einem Speicherort im oder in der Nähe des Stammverzeichnisses zu verschieben. 

## <a name="web-stack-samples"></a>Webstapel-Beispiele
In diesem Abschnitt werden Fragen zum Programmieren, Erstellen oder Ausführen des Schnellstart-Beispiels mit Web-Technologie beantwortet.

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>Wie erkenne ich, ob mein lokaler Computer einen lokalen Webserver unterstützt?
Die Schnellstart-Beispiele, die auf der Web-Technologie basieren, stellen die zum Starten und Hosten eines lokalen Webservers erforderliche Logik bereit. Beispielsweise enthält das auf der PHP 5.4.0+ Runtime basierende PHP-Beispiel einen [integrierten Webserver](http://php.net/manual/en/features.commandline.webserver.php), den Sie für die Entwicklung verwenden. Er ist nicht für die Verwendung in einer Produktionsumgebung vorgesehen. 

Wenn Sie das Node.js-Beispiel heruntergeladen haben, lesen Sie den [Leitfaden für die ersten Schritte mit Node.js](https://nodejs.org/en/docs/guides/getting-started-guide/), um mehr über den Start des Node-Webservers zu erfahren. 

Das ASP.NET-Beispiel, Visual Studio 2015 und neuere Versionen enthalten einen Entwicklungswebserver, der bei der Ausführung des Beispiels automatisch gestartet wird. Sie müssen das Beispielprojekt nicht konfigurieren, um den Webserver zu verwenden. 

Die [Infodatei](https://github.com/microsoftgraph/ruby-connect-rest-sample/blob/master/README.md) zum Ruby Connect-Beispiel enthält Anweisungen zum Start eines lokalen Ruby-Webservers. 

### <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Wenn ein Webplattform-Schnellstart REST- und SDK-Beispiele bereitstellt, kann ich beide zur gleichen Zeit ausführen?

Ja, Sie können beide Beispiele zur gleichen Zeit ausführen. Stellen Sie nur sicher, dass einer von beiden nicht auf dem Standardport ausgeführt wird. Wenn Sie Ihren Testwebserver starten, müssen Sie also eine Portnummer für mindestens eine Version des Beispiels angeben.

### <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>Warum enthalten einige Schnellstarts ein App-Geheimnis und andere nicht?

Serverseitige Webanwendungen, die sichere Anfragen an die Microsoft Graph-API senden müssen, erfordern ein App-Geheimnis. Daher stellen die Schnellstarts für ASP.NET MVC, Node.js, PHP und Ruby ein App-Geheimnis bereit.

### <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>Warum stellt der Angular-Schnellstart kein App-Geheimnis bereit, obwohl alle anderen Schnellstarts für Webplattformen dies tun?

Ein App-Geheimnis ist nur für serverseitige Webanwendungen erforderlich.

### <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>Ich erhalte eine Fehlermeldung, wenn ich versuche, mich anzumelden und die Beispiel-App zu autorisieren. Welche Schritte kann ich ausführen, um dieses Problem zu beheben? 

Versuchen Sie zuerst, die Beispiel-App in einem InPrivate- oder Inkognitofenster auszuführen. Manchmal können Cache-Einstellungen von Webbrowsern dazu führen, dass der Autorisierungsschritt fehlschlägt, insbesondere, wenn Sie sich mit mehreren Microsoft-Konten anmelden. Wenn das nicht funktioniert, kontaktieren Sie uns auf [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Achten Sie darauf, dass Sie Ihre Frage mit Microsoft Graph taggen, und kopieren Sie die Fehlerinformationen in die Frage.

## <a name="didnt-find-what-you-need"></a>Sie haben keine Antwort auf Ihre Frage gefunden?

Wenn diese häufig gestellten Fragen keine Antwort auf Ihre Frage oder keine Lösung für Ihr Problem mit einem oder mehreren der Schnellstarts bieten, melden Sie Ihre Frage oder Ihr Problem bitte auf [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Taggen Sie Ihre Fragen mit „microsoftgraph“.

Wenn sich Ihr Problem auf das Codebeispiel bezieht, das vom Schnellstart zur Verfügung gestellt wird, können Sie auch ein Problem im GitHub-Beispiel-Repository melden. Sie finden das Repository, indem Sie dem Link zum **Abfragen des Beispielcodes** unter Schritt 2 jedes Schnellstarts folgen.
