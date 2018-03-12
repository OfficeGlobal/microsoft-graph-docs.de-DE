# <a name="getting-started-building-microsoft-graph-apps"></a>Erste Schritte zum Entwickeln von Microsoft Graph-Apps

Die Artikel in diesem Abschnitt bieten detaillierte Angaben dazu, wie Apps erstellt werden, die aus einer Palette von Sprachen und Entwicklungsplattformen mit Microsoft Graph verbunden werden. Jeder Artikel geht von einem Startprojekt aus und führt Sie durch die grundlegenden Schritte zum Herstellen einer Verbindung mit Microsoft Graph:

 1. Registrieren der App
 2. Authentifizieren des Benutzers und Abrufen eines Zugriffstokens in der App
 3. Aufrufen von Microsoft Graph in der App
 4. Ausführen der App

Wenn Sie schneller zu einer funktionierenden Lösung gelangen möchten, probieren Sie den [Schnellstart](https://developer.microsoft.com/graph/quick-start) aus.

Jedes fertige Projekt ist identisch mit dem [Connect-Beispiel im Microsoft Graph-Repository](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) für die betreffende Plattform.

Möchten Sie noch mehr Code sehen?

Erkunden Sie alle [Microsoft Graph-Beispiele](https://github.com/microsoftgraph) in GitHub. Die folgende Tabelle enthält zusätzliche Versionen der Beispiele aus diesem Abschnitt. Sie zeigen, wie der Benutzer bei beiden ADAL-Endpunkten (v1.0 und v2.0) authentifiziert wird, und verwenden entweder rohe REST-Aufrufe oder die Microsoft Graph-Clientbibliothek (SDK) zum Herstellen einer Verbindung mit Microsoft Graph.

(Wählen Sie den Artikel, der sich mit dem Authentifizierungsanbieter und der Entwicklungsplattform Ihrer Wahl befasst, und unternehmen Sie die ersten Schritte zum Herstellen einer Verbindung mit Microsoft Graph. Weitere Informationen finden Sie unter [Wo liegen die Unterschiede beim v2.0-Endpunkt?](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-compare))


|Plattform |Dem Azure AD-Endpunkt |Dem Azure AD v2.0-Endpunkt |
|:--- |:--- |:---|
|Android |<a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK-Beispiel</a> |<a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST-Beispiel</a> |
|AngularJS |<a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/angular-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST-Beispiel</a> |
|ASP.NET |<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST-Beispiel</a> |
|iOS (Obj-C) |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK-Beispiel</a> |
|iOS (Swift) |<a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK-Beispiel</a> |
|NodeJS |<a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST-Beispiel</a> |
|PHP |<a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/php-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST-Beispiel</a> |
|Python |<a href="https://github.com/microsoftgraph/python-sample-auth/blob/master/sample_adal.py">REST-Beispiel</a> |<a href="https://aka.ms/graph-python-samples">REST-Beispiel</a>
|Ruby |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST-Beispiel</a> |
|UWP |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a> |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST-Beispiel</a> |
|Xamarin | |<a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK-Beispiel</a> |

<br/>

## <a name="see-also"></a>Siehe auch

- Probieren Sie REST-Beispielaufrufe in unserem [Graph-Tester](https://developer.microsoft.com/de-DE/graph/graph-explorer) aus.
- [Azure AD-Endpunkt-Dokumentation](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-developers-guide)
- [Azure AD v2.0-Endpunkt-Dokumentation](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-appmodel-v2-overview)
