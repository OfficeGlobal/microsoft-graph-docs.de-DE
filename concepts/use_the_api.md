# <a name="use-the-microsoft-graph-api"></a>Verwenden der Microsoft Graph-API

Microsoft Graph ist eine RESTful-Web-API, mit der Sie auf Microsoft Cloud-Dienstressourcen zugreifen können. Nachdem Sie [Ihre App registriert](auth_register_app_v2.md) und [Authentifizierungstoken für einen Benutzer](auth_v2_user.md) oder einen [Dienst abgerufen haben](auth_v2_service.md), können Sie Anforderungen an die Microsoft Graph-API tätigen.

> **Wichtig:**  Die Anwendung der Richtlinien für bedingten Zugriff für Microsoft Graph wurde geändert. Anwendungen müssen aktualisiert werden, um Szenarien ausführen zu können, für die bedingte Richtlinien konfiguriert sind. Weitere Informationen und Anleitungen hierzu finden Sie unter [Developer-Leitfaden zum bedingten Zugriff in Azure Active Directory]((https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)).

Erstellen Sie eine Anforderung, die der folgenden ähnlich ist, um in eine Ressource zu schreiben bzw. daraus zu lesen. Ressourcen können z. B. Benutzer oder E-Mail-Nachrichten sein.

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

Die Komponenten einer Anforderung umfassen Folgendes:

* [HTTP-Methode](#http-methods) – Die HTTP-Methode, die in der Anforderung an Microsoft Graph verwendet wird.
* [`{version}`](#version) – Die Version der Microsoft Graph-API, die Ihre Anwendung verwendet.
* [`{resource}`](#resource) – Die Ressource in Microsoft Graph, auf die Sie verweisen.
* [Abfrageparameter](#query-parameters-optional) – Eine optionale Gruppe von Parametern zum Ändern der Anforderung oder der Antwort.

Nachdem Sie eine Anforderung vorgenommen haben, wird eine Antwort zurückgegeben, die Folgendes umfasst: 

* Statuscode – Ein HTTP-Statuscode, der eine erfolgreiche oder fehlerhafte Ausführung angibt. Informationen zu HTTP-Fehlercodes finden Sie unter [Fehler](errors.md).
* Antwortnachricht – Die angeforderten Daten oder das Ergebnis des Vorgangs. Die Antwortnachricht kann für einige Vorgänge leer sein.
* Der Link **Nächste** – Wenn Ihre Anforderung eine große Datenmenge zurückgibt, müssen Sie diese durch Auswählen von **Nächste** durchlaufen. Weitere Informationen finden Sie unter [Auslagern](paging.md).

## <a name="http-methods"></a>HTTP-Methoden

Microsoft Graph verwendet die HTTP-Methode in Ihrer Anforderung, um zu ermitteln, welche Aktion Ihre Anforderung ausführt. Die API unterstützt die folgenden Methoden.


|**Methode** |**Beschreibung**                             |
| :----- | :------------------------------------------- |
| GET    | Dient zum Lesen von Daten aus einer Ressource.                   |
| POST   | Dient zum Erstellen einer neuen Ressource oder Durchführen einer Aktion. |
| PATCH  | Dient zum Aktualisieren einer Ressource mit neuen Werten.           |
| PUT    | Dient zum Ersetzen einer Ressource durch eine neue.           |
| DELETE | Dient zum Entfernen einer Ressource.                           |

* Für die Methoden **GET** und **DELETE** ist kein Anforderungstext erforderlich.
* Die Methoden **POST**, **PATCH** und **PUT** erfordern einen Anforderungstext, in der Regel im JSON-Format, der zusätzliche Informationen enthält, z. B. die Werte für Eigenschaften der Ressource.

## <a name="version"></a>Version

Microsoft Graph unterstützt derzeit zwei Versionen: `v1.0` und `beta`.

* `v1.0` umfasst allgemein verfügbare APIs. Verwenden Sie die Version 1.0 für alle Produktions-Apps.
* `beta` umfasst APIs, die sich derzeit in der Vorschau befinden. Da möglicherweise grundlegende Änderungen an unseren Beta-APIs eingeführt werden, wird empfohlen, dass Sie die Betaversion nur zum Testen von Apps verwenden, die sich in der Entwicklung befinden; verwenden Sie keine Beta-APIs in Ihren Produktions-Apps.

Wir freuen uns immer über Feedback zu unseren Beta-APIs. Auf unserer [UserVoice]((https://officespdev.uservoice.com/))-Seite können Sie Feedback abgeben oder Features anfordern.

Weitere Informationen zu API-Versionen finden Sie unter [Versionsverwaltung und Support](versioning_and_support.md).

## <a name="resource"></a>Ressource

Ihre URL enthält die Ressourcen, mit denen Sie in der Anforderung interagieren, z. B. `me`, `users`, `groups`, `drives` und `sites`. Alle Ressourcen der obersten Ebene umfassen auch **Beziehungen**, die Sie verwenden können, um auf zusätzliche Ressourcen wie `me/messages` oder `me/drive` zuzugreifen. Sie können auch mithilfe von **Methoden** mit Ressourcen interagieren. Um beispielsweise eine E-Mail-Nachricht zu senden, verwenden Sie `me/sendMail`.

Weitere Informationen zum Navigieren in Ressourcenbeziehungen und Methoden finden Sie unter [Diagramm durchsuchen](traverse_the_graph.md). 

Für jede Ressource sind möglicherweise andere Berechtigungen für den Zugriff erforderlich. Häufig benötigen Sie zum Erstellen oder Aktualisieren einer Ressource eine höhere Ebene von Berechtigungen als zum Lesen. Ausführliche Informationen über die erforderlichen Berechtigungen finden Sie im Methodenreferenzthema. 

Weitere Informationen zu Berechtigungen finden Sie unter [Berechtigungsreferenz](permissions_reference.md).

## <a name="query-parameters-optional"></a>Abfrageparameter (optional)

Sie können optionale Abfrageparameter verwenden, um die Antwort in Ihrer Microsoft Graph-App anzupassen. Verwenden Sie Abfrageparameter, um mehr oder weniger Eigenschaften als in der Standardantwort einzuschließen, die Antwort auf Elemente zu filtern, die einer benutzerdefinierten Abfrage entsprechen, oder zusätzliche Parameter für eine Methode anzugeben.

Durch Hinzufügen der folgenden Filterparameter werden beispielsweise die zurückgegebenen Nachrichten so eingeschränkt, dass nur diejenigen mit der `emailAddress`-Eigenschaft von `jon@contoso.com` zurückgegeben werden.

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

Weitere Informationen zu Abfrageparametern finden Sie unter [Antworten anpassen](query_parameters.md).

## <a name="next-steps"></a>Nächste Schritte

Sie sind nun bereit für Ihre ersten Schritte mit Microsoft Graph. Um mehr zu erfahren, gehen Sie zu [Graph-Tester]((https://developer.microsoft.com/de-DE/graph/graph-explorer)), um ein paar Anforderungen auszuprobieren. Versuchen Sie den [Schnellstart]((https://developer.microsoft.com/de-DE/graph/quick-start)), oder beginnen Sie mit einem unserer [SDKs und Codebeispiele]((https://developer.microsoft.com/de-DE/graph/code-samples-and-sdks)).
