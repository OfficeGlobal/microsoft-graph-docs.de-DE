# <a name="build-cross-device-apps-powered-by-project-rome"></a>Erstellen geräteübergreifender Apps mit Project Rome 

Sie können Project Rome verwenden, um Benutzeroberflächen geräte- und plattformübergreifend zu erstellen und dabei Reibungspunkte für Benutzer zu reduzieren und App-Bindung zu fördern. Für Anwendungen, die Daten geräte- und plattformübergreifend mithilfe von Project Rome freigeben, müssen Sie eine geräteübergreifende App konfigurieren, die Informationen über Ihre plattformspezifischen Apps enthält. 

Eine geräteübergreifende App ermöglicht Folgendes: 

- Verwenden der Project Rome-Aktivitätsfeed-API in Microsoft Graph  
- Lesen und Schreiben von mit einer Gruppe von plattformspezifischen Anwendungen veröffentlichten Benutzeraktivitäten unter Verwendung des Project Rome SDK für Windows, Android und/oder iOS
-  Festlegen von Zielapps über Geräte-Relay-Funktionen in Project Rome unter Verwendung des Project Rome SDK für Android oder iOS

**Geräteübergreifendes Wiederaufnehmen der Tätigkeit mit der Aktivitätsfeed-API**

Sie können eine geräteübergreifende App für die Zuordnung Ihrer Apps für Windows, iOS, Android und das Web konfigurieren, sodass die App auf jeder Plattform von einer beliebigen App in der Gruppe veröffentlichte Benutzeraktivitäten lesen und schreiben kann. 

Beispiel: Ein Benutzer stellt an seinem PC am Arbeitsplatz eine Pressemitteilung vor dem Abendessen mit Freunden fertig. Im Restaurant erhält er von seinem Check eine Benachrichtigung über einen Tippfehler, der so schnell wie möglich korrigiert werden muss. Der Benutzer öffnet eine App auf seinem Android-Telefon und sieht eine Karte mit der Pressemitteilung, die er zuvor bearbeitet hat. Er tippt zum Öffnen auf die Karte, um die Pressemitteilung sofort zu korrigieren und zu seinen Freunden zurückzukehren. 
 
Mit dieser geräteübergreifenden App-Konfiguration wird der Aktivitätsfeed des Benutzers mit allen Geräten und Plattformen problemlos synchronisiert, damit Sie Benutzeroberflächen erstellen können, mit denen Benutzer die Arbeit an wichtigen Aufgaben von jeder App-Oberfläche aus wiederaufnehmen können. 

**Auswählen des richtigen Bildschirms zum richtigen Zeitpunkt mit der Geräte-Relay-API**

Sie können eine geräteübergreifende App mit Anmeldeinformationen für Pushbenachrichtigungen für jede Plattform konfigurieren, auf denen Ihrer App verfügbar ist, sodass ein Befehl oder eine Benachrichtigung auf jedem Gerät, auf dem Sie die App verwenden, unabhängig von der Plattform an Sie übermittelt wird. 

Beispiel: Ein Benutzer schaut sich im Bus auf dem Weg von der Arbeit nach Hause ein Video an. Nachdem er zuhause angekommen ist, tippt er auf die App, um das Video auf der Xbox One zu starten und mit der Wiedergabe auf dem großen Bildschirm fortzufahren. 

Wenn Sie für jede Plattform, auf der Ihre App verfügbar ist, Anmeldeinformationen für Pushbenachrichtigungen Ihrer geräteübergreifenden App zuordnen, kann die App des Benutzer Befehle geräteübergreifed senden. So können Sie eine Benutzererfahrung über mehrere Bildschirme hinweg oder den Wechsel beim Arbeitsablauf von einem Gerät zum nächsten in Echtzeit gewährleisten. 

## <a name="select-the-right-hosting-method-for-your-cross-device-app-configuration"></a>Auswählen der richtigen Hostingmethode für Ihre geräteübergreifende App-Konfiguration
Sie können Ihre geräteübergreifende App-Konfiguration entweder als JSON-Datei in Ihrer Domäne oder als konfigurierbares Profil über das [Windows Dev Center](https://developer.microsoft.com/de-DE/windows) hosten. Wählen Sie eine Hostingoption basierend auf den Project Rome-Funktionen aus, die Sie in Ihren Apps verwenden möchten. 

### <a name="windows-dev-center-profile-recommended"></a>Windows Dev Center-Profil (empfohlen) 
Sie können auf alle Project Rome-Funktionen zugreifen, indem Sie eine geräteübergreifende App verwenden, die im [Windows Dev Center](https://developer.microsoft.com/de-DE/windows) verwaltet wird. Das Windows Dev Center stellt auch die *beste* Art für die Verwaltung aller Änderungen an der geräteübergreifenden App-Konfiguration dar. Sie können an dem vorhandenen Profil vorgenommene Änderungen sicher speichern, bevor Sie diese für die Produktion veröffentlichen. Wenn Sie Änderungen an einer vorhandenen geräteübergreifenden App im Dev Center veröffentlichen, wird das neue Profil etwa nach **einer Stunde** wirksam.  

### <a name="externally-hosted-json-file-limited"></a>Extern gehostete JSON-Datei (eingeschränkt) 
Sie können die folgenden Project Rome-Funktionen auf allen unterstützten Plattformen unter Verwendung einer geräteübergreifender App verwenden, die als extern gehostete JSON-Datei verwaltet wird:  

* Lesen und Schreiben von Benutzeraktivitäten von allen Plattformen mithilfe der [Aktivitätsfeed-API](../api-reference/v1.0/resources/activity-feed-api-overview.md)
* Schreiben von Benutzeraktivitäten von allen Plattformen (Windows, iOS, Android, Web) mithilfe von Project Rome SDKs

Wenn Sie **nur** Zugriff auf diese Funktionen haben, können Sie Ihre geräteübergreifende App-Konfiguration extern in Ihrer Domäne als JSON-Datei hosten.

## <a name="configure-a-cross-device-app-using-the-windows-dev-center"></a>Konfigurieren einer geräteübergreifenden App mithilfe des Windows Dev Center
Eine geräteübergreifende App-ID wird als Domäne angegeben, die Sie besitzen. Die Domäne verweist auf die Zuordnung Ihrer plattformspezifischen App-IDs, die entweder als in Ihrer Domäne gehostete JSON-Datei gespeichert oder über das Windows Dev Center konfigurierbar sind. Nachdem Sie die Domäne für die Angabe Ihrer geräteübergreifenden App-ID ermittelt haben, müssen Sie die Informationen zum Konfigurieren des zugeordneten Profils sammeln. 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id-and-enable-domain-verification"></a>Schritt 1: Auswählen einer sicheren Domäne für Ihre geräteübergreifende App-ID and Aktivieren der Domänenüberprüfung
Bei der als geräteübergreifende App-ID verwendeten Domäne muss es sich um eine Domäne der obersten Ebene oder eine Unterdomäne handeln, die über TLS geschützt ist. Zum Beispiel: https://contoso.com oder https://myapp.contoso.com, jedoch NICHT https://myapp.contoso.com/somepath. **Sie müssen über eine eindeutige Domäne (oder Unterdomäne) pro geräteübergreifende App verfügen.** Sie entscheiden jedoch, welche Apps basierend auf dem zu unterstützenden plattformübergreifenden Verhalten einer einzelnen geräteübergreifenden App zugeordnet werden sollen. 

Beispiel: Ein App-Entwickler mit einer Reihe von Spiel-Apps verwendet möglicherweise eine separate Unterdomäne für jede dieser Apps, um sicherzustellen, dass jede App nur die Benutzeraktivitäten abonniert hat, die sie beim geräte- und plattformübergreifenden Lesen von Daten fortsetzen kann. Andererseits verwendet ein App-Entwickler mit einer Reihe von Produktivitäts-Apps für die Zusammenarbeit möglicherweise eine einzelne Domäne für alle dieser App, damit jede App ein Mitglied geräteübergreifend starten kann.  

#### <a name="assert-domain-ownership-with-the-windows-dev-center"></a>Bestätigen des Domänenbesitzes mit dem Windows Dev Center
Wenn Sie das Windows Dev Center zum Verwalten Ihrer geräteübergreifenden App-Konfiguration verwenden, ist die Domäne, die Ihre geräteübergreifende App-ID darstellt, als Teil Ihres geräteübergreifenden App-Profils gespeichert, sodass Microsoft überprüfen kann, ob Sie der Domänenbesitzer sind. Der Domänenbesitz **muss überprüft werden**, damit die Veröffentlichung Ihrer geräteübergreifenden App-Konfiguration fertig gestellt werden kann. Es wird daher empfohlen, sich zunächst damit zu befassen. Wenn Ihre Domäne noch nicht überprüft wurde, können Sie die Details Ihrer geräteübergreifenden Apps speichern und die Überprüfung nach Abschluss dieses Schritts erneut ausführen, damit Sie Ihre geräteübergreifende App veröffentlichen können.

Um Ihren Domänenbesitz für Ihre geräteübergreifende App zu bestätigen, müssen Sie einen [DNS-TXT](https://go.microsoft.com/fwlink/?linkid=871417)-Eintrag für Ihre Domäne mit einem eindeutigen Wert hinzufügen, der im Dev Center bereitgestellt wurde. Dieser Wert ist pro geräteübergreifende App eindeutig. Um den eindeutigen Wert für Ihre App zu ermitteln, melden Sie sich im Windows Dev Center an, und wählen Sie im linken Menü **Geräteübergreifende Oberflächen** aus, um mit der Konfiguration einer neuen geräteübergreifenden App zu beginnen. Wählen Sie nach Benennen Ihrer neuen geräteübergreifenden App im Untermenü die Option **Domäne der geräteübergreifenden App überprüfen** aus. Diese Seite enthält Anweisungen mit einem eindeutigen Wert **Inline** (z. B. MS=95ff4557-813f-45a5-b2f6-1f94170b979f). Stellen Sie sicher, dass Sie den gesamten Wert einschließlich „MS=“ kopieren.

### <a name="step-2-collect-your-platform-specific-application-ids"></a>Schritt 2: Sammeln der plattformspezifischen Anwendungs-IDs
Sammeln Sie die plattformspezifischen Anwendungs-IDs für jede Anwendung und Plattform, die die [Project Rome-APIs](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/project_rome_overview) verwendet.

Sie müssen alle plattformspezifischen Anwendungs-IDs sammeln, damit sie diese Ihrer geräteübergreifenden App-Identität zuordnen können. Mit dem Windows Dev Center können Sie aus Apps für die universelle Windows-Plattform wählen, die mit Ihrem Entwicklerkonto verknüpft sind, Sie müssen jedoch die Anwendungs-IDs für jede win32-, iOS- oder Android-App manuell angeben und die primäre URL für jede verknüpfte Web-App identifizieren. Sie können bis zu 10 IDs pro Plattform zuordnen. 

So suchen Sie nach den IDs

* **windows_universal** – Geben Sie eine AUMID für jede UWP-App an. Weitere Informationen hierzu finden Sie unter [Suche der Anwendungsbenutzermodell-ID einer installierten App (Branche 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82)) und [Anwendung](https://docs.microsoft.com/de-DE/uwp/schemas/appxpackage/appxmanifestschema/element-application).
* **windows_win32** – Geben Sie eine AUMID für jede App an. Für win32-Apps müssen Sie ein Skript verwenden, um diese Informationen abzurufen. Weitere Informationen hierzu finden Sie unter [Suche der Anwendungsbenutzermodell-ID einer installierten App (Branche 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82)).
* **Android-** – Weitere Informationen finden Sie unter [Ändern des Paketnamens](https://developer.android.com/studio/build/application-id.html#change_the_package_name). 
* **IOS** – Weitere Informationen finden Sie unter [Paket](https://developer.apple.com/documentation/foundation/bundle) und [Erforderliche, lokalisierbare und bearbeitbare Eigenschaften](https://help.apple.com/itunes-connect/developer/#/devfc3066644).
* **msa** – Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com) an. Sie können die App-ID/Client-ID für Ihre Apps anzeigen. Sowohl Live SDK (Hexadezimalwerte) als auch zusammengeführte App-IDs (GUIDs) werden unterstützt.   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>Schritt 3: Konfigurieren der Unterstützung für Microsoft-Konto oder Azure AD
Um eine geräteübergreifende Benutzererfahrung zu ermöglichen, müssen sich App-Benutzer entweder mit einem [Microsoft-Konto](https://account.microsoft.com/account) oder einem [Azure Active Directory](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-developers-guide) (Azure AD)-Konto anmelden. Sie geben die App-ID/Client-IDs zur Unterstützung der Authentifizierung als Teil Ihrer geräteübergreifenden App-Konfiguration an, um die plattformübergreifende Unterstützung zu aktivieren. Sie können bis zu 10 Instanzen angeben.

Sie können nach Ihren vorhandenen App-IDs/Client-IDs suchen, oder neue IDs angeben, indem Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com) mit Ihrem Entwicklerkonto anmelden. Nach Anmelden beim Portal können Sie die App-ID/Client-ID für Ihre Apps anzeigen. Sowohl Live SDK (Hexadezimalwerte) als auch zusammengeführte App-IDs (GUIDs) werden unterstützt.   

Wenn Sie eine Anwendung erstellen, in der Azure AD-Benutzer unterstützt werden, und keine zusammengeführte Anwendungs-ID verwenden, die über das [App-Registrierungsportal](https://apps.dev.microsoft.com) ausgestellt wurde, müssen Sie die GUID für die Anwendungs-ID der Azure-App angeben. So suchen Sie nach der GUID für Ihren Mandanten 

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com) an. 
2. Wählen Sie **Azure Active Directory** aus.
3. Wählen Sie unter **Verwalten** die Option **App-Registrierungen** aus. 
4. Wählen Sie in der Liste Ihre App aus, und zeigen Sie Ihre Anwendungs-ID (GUID) an, die unter **Essentials** aufgeführt wird.

### <a name="step-4-configure-support-for-cross-platform-push-notifications-optional"></a>Schritt 4: Konfigurieren der Unterstützung für plattformübergreifende Pushbenachrichtigungen (optional) 
Wenn Sie Ihre geräteübergreifende App im Windows Dev Center konfigurieren möchten, können Sie die Unterstützung für plattformübergreifende Pushbenachrichtigungen aktivieren, indem Sie die Anmeldeinformationen angeben, die Sie mit den APIs für Android- und iOS-Plattformen für Pushbenachrichtigungen verwenden. Diese sind erforderlich, wenn Sie die Project Rome SDKs für IOS und Android verwenden und mehr als die Veröffentlichung von Benutzeraktivitäten wünschen. Wenn Sie Project Rome-APIs nur für Microsoft Graph verwenden, müssen Sie diesen Schritt nicht ausführen. Sie können bis zu 10 Sätze von Anmeldeinformationen pro Plattform zuordnen. 

>**Wichtig:** Speichern Sie die Anmeldeinformationen für Pushbenachrichtigungen nicht in einer extern gehosteten JSON-Datei.

So suchen Sie nach den IDs

* 
  **Windows-Benachrichtigungsdienst** – Informationen dazu finden Sie unter [Registrieren Ihrer App und Empfangen der Anmeldeinformationen für Ihren Clouddienst ](https://docs.microsoft.com/en-us/previous-versions/windows/apps/hh913756(v=win.10)#registering-your-app-and-receiving-the-credentials-for-your-cloud-service) und [App-Registrierungsportal](https://apps.dev.microsoft.com).
* **Apple Push Notification Service** – Informationen dazu finden Sie unter [APNs Overview](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/APNSOverview.html).
* **Google Cloud Messaging** – Informationen dazu finden Sie unter [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/).

**Hinweis:** Wenn Sie Firebase für Pushbenachrichtigungen auf iOS-Geräten mit Android-Anmeldeinformationen verwenden, müssen Sie Ihre APNs-Anmeldeinformationen als Teil der geräteübergreifenden App bereitstellen. 

## <a name="configure-a-cross-device-app-using-an-externally-hosted-json-file"></a>Konfigurieren einer geräteübergreifenden App mithilfe einer extern gehosteten JSON-Datei
Eine geräteübergreifende App-ID wird als Domäne angegeben, die Sie besitzen. Die Domäne verweist auf die Zuordnung Ihrer plattformspezifischen App-IDs, die entweder als in Ihrer Domäne gehostete JSON-Datei gespeichert oder über das Windows Dev Center konfigurierbar sind. Nachdem Sie die Domäne für die Angabe Ihrer geräteübergreifenden App-ID ermittelt haben, müssen Sie die Informationen zum Konfigurieren des zugeordneten Profils sammeln. 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id"></a>Schritt 1: Auswählen einer sicheren Domäne für Ihre geräteübergreifende App-ID
Eine geräteübergreifende App-ID wird als Domäne angegeben, die Sie besitzen. Dies muss eine Domäne der obersten Ebene oder eine Unterdomäne sein, die über TLS geschützt ist. Zum Beispiel: https://contoso.com oder https://myapp.contoso.com, jedoch NICHT https://myapp.contoso.com/somepath. Sie müssen über eine eindeutige Domäne (oder Unterdomäne) pro geräteübergreifende App verfügen. Sie entscheiden jedoch, welche Apps basierend auf dem zu unterstützenden plattformübergreifenden Verhalten einer einzelnen geräteübergreifenden App zugeordnet werden sollen. 

Beispiel: Ein App-Entwickler mit einer Reihe von Spiel-Apps verwendet möglicherweise eine separate Unterdomäne für jede dieser Apps, um sicherzustellen, dass jede App nur die Benutzeraktivitäten abonniert hat, die sie beim geräte- und plattformübergreifenden Lesen von Daten fortsetzen kann. Ein App-Entwickler mit einer Reihe von Produktivitäts-Apps für die Zusammenarbeit verwendet möglicherweise eine einzelne Domäne für alle diese Apps, damit jede App ein Mitglied geräteübergreifend starten kann.  

#### <a name="assert-domain-ownership-with-an-externally-hosted-json-file"></a>Bestätigen des Domänenbesitzes mithilfe einer extern gehosteten JSON-Datei 
Wenn Sie eine extern gehostete JSON-Datei zum Verwalten Ihrer geräteübergreifenden App verwenden, können Sie den Domänenbesitz bestätigen, indem Sie Ihr Microsoft-Konto oder Ihre Azure AD-App-IDs in der Datei mit den plattformübergreifenden App-IDs hinzufügen. Der Domänenbesitz wird im Rahmen des Veröffentlichungsprozesses überprüft, wenn Sie die Aktivitätsfeed-API zum Erstellen von Benutzeraktivitäten verwenden.

Das System speichert die Inhalte der Datei im Cache, um das Generieren häufiger Anforderungen in Ihrer Domäne zu vermeiden. Falls konfiguriert, werden HTTP-Cache-Header vom Dienst während der Auswertung berücksichtigt, wann der Cache zu aktualisieren ist. Falls nicht konfiguriert, führt der Dienst alle 24 Stunden eine Aktualisierung durch. 

### <a name="step-2-collect-your-platform-specific-application-ids-and-construct-your-json-file"></a>Schritt 2: Sammeln der plattformspezifischen Anwendungs-IDs und Erstellen der JSON-Datei
Sammeln Sie die plattformspezifischen Anwendungs-IDs für jede Anwendung und Plattform, die den Aktivitätsfeed und/oder die Geräte-Relay-API verwenden soll. 

Sie müssen alle plattformspezifischen Anwendungs-IDs sammeln, damit sie diese Ihrer geräteübergreifenden App-Identität zuordnen können. Beim Verwenden einer extern gehosteten JSON-Datei müssen Sie die App-IDs für jede plattformspezifische App für die Konfiguration im Rahmen der geräteübergreifenden App sammeln und diese im angegebenen Format zusammenstellen. Sie können bis zu 10 IDs pro Plattform zuordnen. 

#### <a name="constructing-your-cross-platform-app-identifiers-file"></a>Erstellen Ihrer Datei mit plattformübergreifenden App-IDs
Die JSON-Datei selbst muss den Namen **cross-platform-app-identifiers** aufweisen und im Stamm Ihrer HTTPS-Domäne gehostet werden. Bei den Inhalten der Datei handelt es sich um ein JSON-Array von Zuordnungen zwischen den von der Anwendung unterstützten Plattformen und den Anwendungs-IDs für diese Plattformen. Fügen Sie beim Erstellen der Datei ein JSON-Objekt für jede Anwendung und Plattform hinzu, die die Project Rome-APIs verwenden soll. 
 
Mit dieser Datei sind mehrere JSON-Objekte mit derselben Plattform-ID zulässig. Eine iPhone-App und eine iPad-App sollten zum Beispiel als separate JSON-Objekte jeweils mit einem Plattformwert für iOS aufgeführt sein. Im folgenden Beispiel wird die Web-Plattform-ID angezeigt.
 
Sie müssen nicht für alle Plattformen ein JSON-Objekt hinzufügen. Fügen Sie JSON-Objekte nur für Plattformen hinzu, auf denen Ihre Anwendung Project Rome-APIs verwenden soll. Wenn Sie über keinen App-Client für die Android-Plattform verfügen, benötigen Sie beispielsweise keinen Eintrag in der Datei für Android.
 
Im folgende Beispiel sind alle gültigen Plattform-IDs enthalten, die aktuell zulässig sind. JSON-Objekte, die einen ungültigen Plattformwert enthalten, werden entfernt.  

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

So suchen Sie nach den IDs

* **windows_universal** – Geben Sie eine AUMID für jede UWP-App an. Weitere Informationen hierzu finden Sie unter [Suche der Anwendungsbenutzermodell-ID einer installierten App (Branche 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82)) und [Anwendung](https://docs.microsoft.com/de-DE/uwp/schemas/appxpackage/appxmanifestschema/element-application).
* **windows_win32** – Geben Sie eine AUMID für jede App an. Für win32-Apps müssen Sie ein Skript verwenden, um diese Informationen abzurufen. Weitere Informationen hierzu finden Sie unter [Suche der Anwendungsbenutzermodell-ID einer installierten App (Branche 8.1)](https://docs.microsoft.com/en-us/previous-versions/windows/embedded/dn449300(v=winembedded.82)).
* **Android-** – Weitere Informationen finden Sie unter [Ändern des Paketnamens](https://developer.android.com/studio/build/application-id.html#change_the_package_name). 
* **IOS** – Weitere Informationen finden Sie unter [Paket](https://developer.apple.com/documentation/foundation/bundle) und [Erforderliche, lokalisierbare und bearbeitbare Eigenschaften](https://help.apple.com/itunes-connect/developer/#/devfc3066644).
* **msa** – Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com) an. Sie können die App-ID/Client-ID für Ihre Apps anzeigen. Sowohl Live SDK (Hexadezimalwerte) als auch zusammengeführte App-IDs (GUIDs) werden unterstützt.   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>Schritt 3: Konfigurieren der Unterstützung für Microsoft-Konto oder Azure AD
Um eine geräteübergreifende Benutzererfahrung zu ermöglichen, müssen sich App-Benutzer entweder mit einem Microsoft-Konto oder einem Azure AD-Konto anmelden. Sie geben die App-ID/Client-IDs zur Unterstützung der Authentifizierung als Teil Ihrer geräteübergreifenden App-Konfiguration an, um die plattformübergreifende Unterstützung zu aktivieren. Sie können bis zu 10 Instanzen angeben.

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

Sie können nach Ihren vorhandenen App-IDs/Client-IDs suchen, oder neue IDs angeben, indem Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com) mit Ihrem Entwicklerkonto anmelden. Nach Anmeldung können Sie die App-ID/Client-ID für Ihre Apps anzeigen. Sowohl Live SDK (Hexadezimalwerte) als auch zusammengeführte App-IDs (GUIDs) werden unterstützt. Verwenden Sie den Plattformtyp „msa“, wenn Sie die zum Aktivieren der Unterstützung für ein Microsoft-Konto oder Azure AD zu verwendenden IDs hinzufügen, wie im vorherigen Beispiel gezeigt.  

>[Hinweis:](https://apps.dev.microsoft.com) Wenn Sie eine Anwendung erstellen, in der Azure AD-Benutzer unterstützt werden, und keine zusammengeführte Anwendungs-ID verwenden, die über das **App-Registrierungsportal** ausgestellt wurde, müssen Sie die GUID für die Anwendungs-ID der Azure-App angeben. Dieser Typ von ID sollte auch als Plattformtyp „msa“ konfiguriert werden. 

So suchen Sie nach der GUID für Ihren Mandanten im Azure-Portal 

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com) an.
2. Wählen Sie **Azure Active Directory** aus. 
3. Wählen Sie unter **Verwalten** die Option **App-Registrierungen** aus.
4. Wählen Sie Ihre App aus der Liste aus. Sie können Ihre Anwendungs-ID (GUID) unter **Essentials** anzeigen.

#### <a name="encoding-the-cross-platform-app-identifiers-file"></a>Codieren der Datei mit plattformübergreifenden App-IDs 
Wenn die Aktivitäten in den richtigen systemeigenen Clientanwendungen nicht plattformübergreifend fortgesetzt werden, oder Sie keine von Mitgliedern der Gruppe veröffentlichten Aktivitäten lesen können, wird Ihre JSON-Datei möglicherweise nicht ordnungsgemäß analysiert. Stellen Sie bei der Ausgabe dieser Datei sicher, dass Sie die Datei mit den plattformübergreifenden App-IDs mit der Codierung „Unicode (UTF-8 ohne Signatur) – Codepage 65001“ speichern.

#### <a name="updating-the-cross-platform-app-identifiers-json-file"></a>Aktualisieren der JSON-Datei mit plattformübergreifenden App-IDs 
Das System speichert die Inhalte der Datei im Cache, um das Generieren häufiger Anforderungen in Ihrer Domäne zu vermeiden. Falls konfiguriert, werden HTTP-Cache-Header vom Dienst während der Auswertung berücksichtigt, wann der Cache zu aktualisieren ist. Falls nicht konfiguriert, führt der Dienst alle 24 Stunden eine Aktualisierung durch. 

## <a name="configure-your-app-client"></a>Konfigurieren Ihres App-Clients 
Wenn Sie die clientseitigen APIs für Windows, iOS oder Android verwenden, müssen Sie sicherstellen, dass Ihr App-Client mit dem Hostwert konfiguriert ist, der Ihre geräteübergreifende App-Identität (z. B. „contoso.com“) darstellt.

### <a name="microsoft-graph-apps"></a>Microsoft Graph-Apps 
Wenn eine App die Aktivitätsfeed-API in Microsoft Graph verwendet, muss Ihr Hostwert in der **activitySourceHost**-Eigenschaft angegeben werden. Einzelheiten hierzu finden Sie unter [Aktivitätsressourcentyp](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/projectrome_activity).

### <a name="universal-windows-apps"></a>Universelle Windows-Apps
Wenn Sie über eine Windows-App verfügen, müssen Sie den Hostwert im App-Manifest vor der Veröffentlichung von Daten konfigurieren. Einzelheiten hierzu finden Sie unter [uap5:UserActivity](https://docs.microsoft.com/de-DE/uwp/schemas/appxpackage/uapmanifestschema/element-uap5-useractivity). 

<!-- Removing until we add the details.
### iOS & Android apps
*Details coming soon.*
-->

## <a name="maintaining-your-cross-device-app-configuration"></a>Verwalten der geräteübergreifenden App-Konfiguration
Wenn eine neue Anwendung veröffentlichen, die Benutzeraktivitäten generiert, ist es wichtig, dass Sie für die geräteübergreifende App die Konfigurationswerte im Vorfeld aktualisieren, damit alle neuen veröffentlichten Aktivitäten der geräteübergreifenden App ordnungsgemäß zugeordnet sind. Die den Benutzeraktivitäten, die vor einer Änderung an der Konfiguration veröffentlicht wurden, zugeordnete geräteübergreifende App-Konfiguration wird nicht automatisch aktualisiert. Die Aktualisierung einer Aktivität mit einer alten Konfiguration wird jedoch auf die neueste Version in der Datei aktualisiert.  

## <a name="troubleshooting"></a>Problembehandlung

Im Folgenden werden einige häufige Probleme erläutert, die mit der Aktivitätsfeed-API auftreten können.

### <a name="activities-are-not-available-to-read-and-write-for-all-apps-in-the-cross-device-app-configuration"></a>Aktivitäten stehen nicht zum Lesen und Schreiben für alle Apps in der geräteübergreifenden App-Konfiguration zur Verfügung.
Die Aktivitätsfeed-API erfasst die geräteübergreifende App-Konfiguration asynchron, sodass Konfigurationsfehler möglicherweise nicht ohne Weiteres beim Veröffentlichen von Benutzeraktivitäten erkennbar sind. Falls der Dienst die JSON-Datei nicht erfassen kann, entweder aufgrund eines TLS- oder Formatierungsfehlers, werden alle veröffentlichten Aktivitäten nur der App-ID zugeschrieben, die die Aktivität bereitgestellt hat. Wenn Aktivitäten über Microsoft Graph veröffentlicht wurden, wird die Microsoft-Konto-App-ID zum Autorisieren von Anforderungen an Microsoft Graph verwendet. Wenn Aktivitäten über clientseitige APIs veröffentlicht wurden, zeichnet die activity.applicationId nur die ID der plattformspezifischen App auf, die die Aktivität bereitgestellt hat. Dadurch können keine Lese- und Schreibvorgänge für Aktivitäten von einer anderen identifizierten plattformspezifischen App in der geräteübergreifenden App-Konfiguration durchgeführt werden. 

### <a name="platform-will-not-initialize-on-android-or-ios"></a>Plattform wird unter Android oder iOS nicht initialisiert
Für die Geräte-Relay-API für Android oder iOS ist die geräteübergreifende App-Konfiguration erforderlich, um Verbindungen mit der Android- oder iOS-App zu instanziieren. Stellen Sie für den Fall, dass die Plattform die Initialisierung nicht durchführen kann sicher, dass Sie die Microsoft-Konto-App-IDs und die Anmeldeinformationen für Pushbenachrichtigungen zum Konfigurieren Ihrer geräteübergreifenden App im Windows Dev Center korrekt ermittelt haben, und konfigurieren Sie den Hostwert Ihrer Client-Apps mit der Domäne, die Ihre geräteübergreifende App identifiziert. 
