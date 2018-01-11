# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>Erste Schritte mit Microsoft Graph in einer Python-App 

Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens aus dem Azure AD und zum Aufrufen von Microsoft Graph. Sie werden durch das [Senden von E-Mails über Microsoft Graph aus Python](https://github.com/microsoftgraph/python-sample-send-mail) geführt und erhalten Informationen zu den Hauptkonzepten, die Sie zur Verwendung der Microsoft Graph-API implementieren. In diesem Artikel wird beschrieben, wie Sie mithilfe von direkten REST-Aufrufen auf Microsoft Graph zugreifen.

![Formular zum Senden von E-Mails](https://raw.githubusercontent.com/microsoftgraph/python-sample-send-mail/master/static/images/sendmail.png)

## <a name="choosing-an-authentication-library"></a>Auswählen einer Authentifizierungsbibliothek

Um Aufrufe an Microsoft Graph ausführen zu können, muss Ihre App ein gültiges Zugriffstoken aus Azure Active Directory (Azure AD), dem Microsoft-Cloudidentitätsdienst, abrufen, und das Token muss in einem HTTP-Header bei jedem Aufruf der Microsoft Graph-REST-API übergeben werden. Der Authentifizierungsansatz von Graph basiert auf den OAuth 2.0- und Open ID Connect-Standards, es gibt also eine große Auswahl an [Authentifizierungsbibliotheken](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-libraries) zum Implementieren der Authentifizierung in Ihre Anwendung.

Im folgenden Beispiel wird die [Flask-OAuthlib](https://flask-oauthlib.readthedocs.io/en/latest/)-Bibliothek zum Implementieren des OAuth 2.0-Workflows [Autorisierungscodegenehmigung](https://tools.ietf.org/html/rfc6749#section-4.1) verwendet; dies ist der empfohlene Authentifizierungsworkflow für in Python geschriebene Webanwendungen. Informationen zu anderen Authentifizierungsoptionen finden Sie unter [Python-Authentifizierungsbeispiele für Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth).

## <a name="installing-and-running-the-send-mail-sample"></a>Installieren und Ausführen des Beispiels zum Senden von E-Mails

Zum Installieren und Konfigurieren der Beispiel-App folgen Sie den Anweisungen unter [Installation der Python-REST-Beispiele]((https://github.com/microsoftgraph/python-sample-auth)/blob/master/installation.md). Verwenden Sie in dem unten dargestellten Beispiel zum Senden von E-Mails den folgenden Befehl zum Klonen des Repositorys.

```git clone https://github.com/microsoftgraph/python-sample-send-mail.git```

Wenn Sie die Anwendung wie in den [Installationsanweisungen]((https://github.com/microsoftgraph/python-sample-auth)/blob/master/installation.md) beschrieben registrieren, müssen Sie unbedingt die Berechtigungen **User.Read** und **Mail.Send** einschließen, die für dieses Beispiel erforderlich sind.

Nach Abschluss der Installation/Konfiguration,können Sie die Beispiel-App ausführen, indem Sie die Anweisungen zum [Ausführen des Beispiels]((https://github.com/microsoftgraph/python-sample-send-mail)#running-the-sample) befolgen.

## <a name="code-walkthrough"></a>Exemplarische Vorgehensweise

Nachfolgend finden Sie eine Übersicht des [Quellcodes]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py) für die Beispiel-App.

Die ersten Codezeilen sind die [Importe]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L4-L32) für die Python-Module und -Pakete, die in dem Beispiel verwendet werden:

* Das **base64**-Modul aus der Standardbibliothek wird zum Codieren von E-Mail-Anlagen verwendet.
* Das **mimetypes**-Modul wird verwendet, um den MIME-Typ für Dateianlagen zu ermitteln.
* Das **os**-Modul bietet allgemeine Dateisystemfunktionen.
* Das **pprint**-Modul aus der Standardbibliothek wird für den Schöndruck von Fehlermeldungen verwendet, die von Graph zurückgegeben werden. (Wenn Sie zum Beispiel eine ungültige E-Mail-Adresse als Empfänger verwenden.)
* Das **uuid**-Modul aus der Standardbibliothek wird zum Generieren einer zufälligen Zeichenfolge aus 36 Zeichen verwendet, um jede Graph-Anforderung eindeutig zu identifizieren. Dies kann für das Debuggen nützlich sein.
* Das **flask**-Paket ist das Webframework für das Beispiel.
* Die **OAuth**-Klasse von **flask_oauthlib.client** ist ein Wrapper um die Flask-App herum, die den OAuth 2.0-Authentifizierungsworkflow implementiert.
* Das **config**-Modul enthält die Einstellungen für die Anwendungsregistrierung, wie im obigen Installationsprozess konfiguriert.

Als Nächstes [erstellen wir eine Flask-App]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L15-L17) und dann das [Graph-Clientobjekt]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L19-L28) namens **MSGRAPH**.

Nach diesen ersten Einrichtungsschritten kommen drei Flask-Routenhandlerfunktionen, die den Authentifizierungsworkflow implementieren: [homepage()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L30-L33), [login()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L35-L39) und [authorized()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L41-L48). Weitere Informationen zum Authentifizierungsworkflow finden Sie im Abschnitt [Beispielarchitektur]((https://github.com/microsoftgraph/python-sample-auth)#sample-architecture) des Repositorys der Python-Authentifizierungsbeispiele.

Der nächste Routenhandler, [mailform()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L50-L83), ist das Formular, in dem Sie die E-Mail-Empfänger, den Betreff und den Text angeben. Beachten Sie, dass diese Funktion auch unsere ersten Aufrufe an Graph umfasst, einschließlich des Abrufens des Benutzerprofils und Profilfotos, Hochladens von Fotos auf OneDrive und Erstellens einer Freigabeverknüpfung. Die Daten werden an die [mailform.html-Vorlage übergeben]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L77-L83), wobei der Empfänger, der Betreff und der Text vor dem Senden der Nachricht bearbeitet werden können. 

Als Nächstes kommt die [send_mail()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L85-L107)-Funktion, die die E-Mail sendet und die Antwort von der Graph-API anzeigt. Diese verwendet eine sendmail()-Hilfsfunktion und übergibt diese an die Abfragezeichenfolgenparameter, die aus dem Formular veröffentlicht wurden:

```python
response = sendmail(client=MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    body=flask.request.args['body'],
                    attachments=[profile_pic])
```

Die [get_token()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L109-L123)-Funktion wird von der Flask-OAuthlib-Clientinstanz (```MSGRAPH```) verwendet, um immer dann ein Zugriffstoken abzurufen, wenn wir Aufrufe an Graph ausführen. Das Zugriffstoken wird in einem HTTP-Header mit dem Namen **Authorization** übergeben, Sie müssen sich darum aber in Ihrem Code nicht kümmern. Führen Sie einfach Anrufe von Graph über die HTTP-Verb-Methoden des Clients (z. B. get() oder post()) aus; die Clientinstanz weiß dann, dass ```get_token()``` aufgerufen werden muss, um ein Token zu erhalten, da die Funktion ```tokengetter``` [aufweist]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L109-L109).

Der Rest des Beispiels besteht aus Helper-Funktionen, die allgemeine Graph-Aktivitäten vereinfachen:

* [request_headers()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L114-L123) gibt ein Wörterbuch von HTTP-Headern zurück, die mit jedem Aufruf von Graph gesendet werden.
* [profile_photo()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L125-L154) gibt das Profilfoto des Benutzers zurück und speichert optional eine Kopie in einer lokalen Datei.
* [sendmail()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L156-L202) sendet eine Nachricht über den ```me/microsoft.graph.sendMail```-Endpunkt.
* [sharing_link()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L204-L221) erstellt eine Freigabeverknüpfung für ein angegebenes Element in OneDrive.
* [upload_file()]((https://github.com/microsoftgraph/python-sample-send-mail)/blob/master/sample.py#L223-L255) lädt eine Datei auf OneDrive hoch.

Diese Helper-Funktionen können in anderen Anwendung hilfreich sein.

## <a name="other-python-rest-samples"></a>Weitere Python-REST-Beispiele

Nachfolgend finden Sie einige weitere Python-Beispiele, die veranschaulichen, wie Sie mit verschiedenen Aspekten von Microsoft Graph arbeiten:

* [Python-Authentifizierungsbeispiele für Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth)
* [Arbeiten mit paginierten Microsoft Graph-Antworten in Python](https://github.com/microsoftgraph/python-sample-pagination)
* [Arbeiten mit offenen Graph-Erweiterungen in Python](https://github.com/microsoftgraph/python-sample-open-extensions)

Wenn Sie nach einem bestimmten Beispiel suchen, teilen Sie uns das mit, indem Sie uns [ein Problem übermitteln]((https://github.com/microsoftgraph/python-sample-auth)/issues). Wir schätzen Ihr Feedback zu allen Microsoft Graph-Szenarien, die Sie in Python entwickeln möchten!

Die Microsoft Graph-API ist eine leistungsfähige einheitliche API, die für die Interaktion mit beliebigen Microsoft-Daten verwendet werden kann. Schauen Sie sich die [Entwicklerdokumentationen](https://developer.microsoft.com/de-DE/graph/docs/concepts/overview) oder den [Graph-Explorer](https://developer.microsoft.com/de-DE/graph/graph-explorer) an, um sich von den Vorteilen von Microsoft Graph zu überzeugen.
