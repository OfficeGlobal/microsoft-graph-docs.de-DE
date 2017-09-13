# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Grap-Schnellstart – häufig gestellte Fragen

In diesen häufig gestellten Fragen werden Fragen und Probleme behandelt, die bei [Microsoft Grap-Schnellstarts](https://developer.microsoft.com/en-us/graph/quick-start) auftreten können.

## <a name="what-do-the-quick-starts-do"></a>Welche Funktionen haben die Schnellstarts?

Unabhängig von der Plattform, die Sie auswählen, geschieht bei Schnellstarts Folgendes:

- Registrierung einer neuen Anwendung für Sie im [App-Registrierungsportal](https://apps.dev.microsoft.com). Daher bitten wir Sie, sich mit einem Microsoft-Konto anzumelden, wenn Sie **eine App-ID erhalten**. Wenn für Ihre Anwendung ein App-Geheimnis erforderlich ist, erstellt der Schnellstart eins für Sie. 
- Download einer Kopie des Beispielcodes, der in einem GitHub-Repository gespeichert ist. Sie können diese Repositorys in der [MicrosoftGraph-Organisation](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) auf GitHub anzeigen.
- Einfügen der neuen App-ID und, falls erforderlich, des App-Geheimnisses in eine Konfigurationsdatei innerhalb des Beispielcodes, der im GitHub-Repository gespeichert ist. Vertrauliche Informationen sollten nicht in einer HTTP-Anforderung gesendet werden. Daher bitten wir Sie, das App-Geheimnis zu kopieren, nachdem wir die neue Anwendung erstellt haben. Kopieren Sie es dann in ein Formular im Schnellstart, bevor Sie eine Kopie des Beispielcodes herunterladen.
- Aufforderung zum Herunterladen des vollständig konfigurierten Beispiels. Nachdem Sie den Beispielcode heruntergeladen und entzippt haben, sollte eine Client- oder Webanwendung ausgeführt werden, sofern Sie die angegebenen erforderlichen Komponenten (IDEs, Web-Frameworks usw.) in Ihrer Entwicklungsumgebung installiert haben.


## <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>Warum wird mein ASP.NET-, UWP- oder Xamarin-Projekt nicht erstellt?

Wenn ein Beispiel, das .NET-Bibliotheken verwendet, nicht in Visual Studio erstellt wird, überschreitet eines oder mehrere Ihrer Projekte eventuell die Windows-Pfadlängenbeschränkung von 260 Zeichen. Insbesondere bei Xamarin-Lösungen tritt dies häufig auf, vor allen Dingen bei Android-Projekten innerhalb von Xamarin Lösungen. Versuchen Sie, die Lösung zu einem Speicherort im oder in der Nähe des Stammverzeichnisses zu verschieben. 

## <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Wenn ein Webplattform-Schnellstart REST- und SDK-Beispiele bereitstellt, kann ich beide zur gleichen Zeit ausführen?

Ja, Sie können beide Beispiele zur gleichen Zeit ausführen. Stellen Sie nur sicher, dass einer von beiden nicht auf dem Standardport ausgeführt wird. Wenn Sie Ihren Testwebserver starten, müssen Sie also eine Portnummer für mindestens eine Version des Beispiels angeben.

## <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>Ich habe keine E-Mail erhalten, und es werden keine Fehler oder Ausnahmen angezeigt. Warum hat es nicht funktioniert?

Wenn das Beispiel augenscheinlich eine E-Mail sendet, aber sie nicht in Ihrem Posteingang angezeigt wird, überprüfen Sie den Junk-E-Mail- oder Spam-Ordner. Wenn Sie die Nachricht von einem Testmandanten senden, wird die Nachricht möglicherweise als Spam gekennzeichnet.

## <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>Ich erhalte eine Fehlermeldung, wenn ich versuche, mich anzumelden und die Beispiel-App zu autorisieren. Welche Schritte kann ich ausführen, um dieses Problem zu beheben? 

Versuchen Sie zuerst, die Beispiel-App in einem InPrivate- oder Inkognitofenster auszuführen. Manchmal können Cache-Einstellungen von Webbrowsern dazu führen, dass der Autorisierungsschritt fehlschlägt, insbesondere, wenn Sie sich mit mehreren Microsoft-Konten anmelden. Wenn das nicht funktioniert, kontaktieren Sie uns auf [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Achten Sie darauf, dass Sie Ihre Frage mit Microsoft Graph taggen, und kopieren Sie die Fehlerinformationen in die Frage.

## <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>Warum enthalten einige Schnellstarts ein App-Geheimnis und andere nicht?

Serverseitige Webanwendungen, die sichere Anfragen an die Microsoft Graph-API senden müssen, erfordern ein App-Geheimnis. Daher stellen die Schnellstarts für ASP.NET MVC, Node.js, PHP und Ruby ein App-Geheimnis bereit.

## <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>Warum stellt der Angular-Schnellstart kein App-Geheimnis bereit, obwohl alle anderen Schnellstarts für Webplattformen dies tun?

Ein App-Geheimnis ist nur für serverseitige Webanwendungen erforderlich.

## <a name="why-does-my-quick-start-contain-a-readme-file"></a>Warum enthält mein Schnellstart eine Readme-Datei?

Jeder Schnellstart registriert eine neue Anwendung und erstellt eine Zip-Datei, die den Inhalt eines GitHub-Repositorys enthält. Die Dateien im Repository werden aktualisiert, damit Sie die Beispielanwendung im Repository nicht konfigurieren müssen. Sie finden diese Repositorys in der [MicrosoftGraph-Organisation](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) auf GitHub.

Sie können sich die mit Schnellstarts verknüpften Repositorys gerne ansehen und Probleme melden, oder Sie befolgen die Anweisungen in der Readme-Datei zum Registrieren Ihrer eigenen Anwendung. Folgen Sie dem Link zum **Abfragen des Beispielcodes** unter Schritt 2 jedes Schnellstarts, um das zugehörige Repository aufzurufen.

## <a name="why-did-the-sample-give-me-an-image-containing-a-thought-bubble"></a>Warum ist im Beispiel ein Bild mit einer Gedankenblase enthalten?

Die meisten durch die Schnellstarts bereitgestellten Beispiele rufen Ihr Profilbild ab und laden es in das Stammverzeichnis Ihres OneDrive-Kontos hoch. Wenn Sie sich mit einem Microsoft-Konto (live.com, hotmail.com) anmelden, kann Microsoft Graph Ihr Profilbild aktuell nicht abrufen. Daher greifen wir auf das Bild mit der Gedankenblase zurück. Im Beispiel wird dieses Bild auch verwendet, wenn Ihr Konto nicht über ein Profilbild verfügt.

## <a name="why-do-you-provide-a-manage-your-apphttpsappsdevmicrosoftcom-link-after-i-get-an-app-id"></a>Warum wird ein Link zum **[Verwalten der App](https://apps.dev.microsoft.com)** bereitgestellt, nachdem ich eine App-ID erhalten habe?

Wir stellen diesen Link bereit, da im Rahmen des App-ID-Schritts eine neue Anwendung für Sie im [App-Registrierungsportal](https://apps.dev.microsoft.com) registriert wird. Über diesen Link können Sie die Einstellungen für diese Anwendung anzeigen, die Anwendung löschen oder sogar die Einstellungen für die Anwendung aktualisieren, nachdem Sie das Beispiel ausgeführt haben. 

## <a name="didnt-find-what-you-need"></a>Sie haben keine Antwort auf Ihre Frage gefunden?

Wenn diese häufig gestellten Fragen keine Antwort auf Ihre Frage oder keine Lösung für Ihr Problem mit einem oder mehreren der Schnellstarts bieten, melden Sie Ihre Frage oder Ihr Problem bitte auf [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). 

Wenn sich Ihr Problem auf das Codebeispiel bezieht, das vom Schnellstart zur Verfügung gestellt wird, können Sie auch ein Problem im GitHub-Beispiel-Repository melden. Sie finden das Repository, indem Sie dem Link zum **Abfragen des Beispielcodes** unter Schritt 2 jedes Schnellstarts folgen.
