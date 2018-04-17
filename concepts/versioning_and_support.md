# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Versionsverwaltung, Support und Richtlinien für wesentliche Änderungen für Microsoft Graph 

In diesem Artikel werden der Support und die Richtlinien für wesentliche Änderungen für Microsoft Graph sowie die Versionen der Microsoft Graph-API beschrieben, die derzeit verfügbar sind.

## <a name="support-policy-and-deprecation-information"></a>Supportrichtlinie und Informationen zu veralteten Funktionen

Microsoft Graph folgt der [Microsoft-Lebenszyklusrichtlinie](https://support.microsoft.com/de-DE/lifecycle). 

Wenn neue Versionen der Microsoft Graph REST-APIs und Microsoft Graph-SDKs veröffentlicht werden, werden frühere Versionen eingestellt. Microsoft erklärt eine Version mindestens 24 Monate vor der Einstellung einer API oder eines SDKs als veraltet. 

Wenn wir die Hauptversion der API erhöhen (z. B. von v1.0 auf v2.0), wird angekündigt, dass die aktuelle Version (in diesem Beispiel v1.0) sofort veraltet ist und dass diese 24 Monate nach der Ankündigung nicht mehr unterstützt wird. Aus Gründen der Dienstsicherheit oder aufgrund von Problemen mit der Integritätszuverlässigkeit werden wir möglicherweise Ausnahmen im Hinblick auf diese Richtlinie machen.  

Wenn eine API als veraltet gekennzeichnet ist, wird dringend empfohlen, dass Sie so bald wie möglich zur neuesten Version migrieren. In einigen Fällen werden wir angeben, dass neue Anwendungen mit der Verwendung der neuen APIs beginnen müssen, kurz nachdem die ursprünglichen APIs veraltet sind. In diesen Fällen können nur aktive Anwendungen, die derzeit die veralteten APIs verwenden, diese weiterhin verwenden.   

### <a name="api-contract-and-non-backward-compatible-changes"></a>Änderungen am API-Vertrag und nicht abwärtskompatible Änderungen

Microsoft Graph verfügt über die unterschiedlichen Versionen hinweg über ein Änderungsprotokoll. Diese Änderungen sind im [Microsoft Graph-Änderungsprotokoll](changelog.md) aufgeführt. Wenn Microsoft Graph neue Funktionen und Daten hinzugefügt werden, wird die API-Versionsnummer für alle nicht abwärtskompatiblen Änderungen an der API erhöht. 

Nachfolgend finden Sie Beispiele für nicht abwärtskompatible Änderungen:

 - Änderungen an der URL oder an grundlegenden Anforderungen/Antworten im Zusammenhang mit einer Ressource    
 - Entfernen, Umbenennen oder Ändern des Typs einer deklarierten Eigenschaft
 - Entfernen oder Umbenennen von APIs oder API-Parametern
 - Hinzufügen eines erforderlichen Anforderungsheaders

Nachfolgend finden Sie Beispiele für abwärtskompatible Änderungen:

 - Hinzufügen von Eigenschaften, die Nullwerte zulassen oder einen Standardwert aufweisen
 - Hinzufügen eines Elements zu einer Aufzählung
 - Entfernen, Umbenennen oder Ändern des Typs einer offenen Erweiterung
 - Entfernen, Umbenennen oder Ändern des Typs einer Anmerkung
 - Einführung der Auslagerung in vorhandene Sammlungen
 - Änderungen an Fehlercodes
 - Änderungen an der Reihenfolge von Eigenschaften
 - Änderungen an der Länge oder am Format von verschlüsselten Zeichenfolgen, z. B. Ressourcen-IDs

>**Hinweis:** Die Liste von abwärtskompatiblen Änderungen wird im Laufe der Zeit aktualisiert. Wenn Sie Ihre eigenen Clientproxys (z. B. WCF-Clients) generieren, wird empfohlen, dass Ihre Clientanwendungen auf das Empfangen von Eigenschaften und abgeleiteten Typen vorbereitet sein sollten, die zuvor nicht vom Microsoft Graph-API-Dienst definiert wurden. Die Microsoft Graph-API befolgt die im Abschnitt [Modellversionsverwaltung](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) der [Microsoft REST-API-Richtlinien](https://github.com/microsoft/api-guidelines/) beschriebene Anleitung. 

## <a name="versions"></a>Versionen

Die folgenden Versionen der Microsoft Graph-API stehen derzeit zur Verfügung.

### <a name="beta-version"></a>Betaversion
Die Microsoft Graph-API-Betaversion, die unter `https://graph.microsoft.com/beta` verfügbar gemacht wird, enthält Features, die sich derzeit in der Vorschau befinden. Dokumentation zur Beta-API finden Sie in der [Microsoft Graph-Beta-Endpunktreferenz](../api-reference/beta/beta-overview.md). Von Zeit zu Zeit ist mit wesentlichen Änderungen an der Betaversion zu rechnen. Verwenden Sie keine Produktionsabhängigkeit in Beta-APIs.

Wir übernehmen keine Garantie dafür, dass eine Betafunktion für die aktuelle Version höher gestuft wird. Wenn das Microsoft Graph-API-Team der Meinung ist, dass eine Betafunktion für die allgemeine Verfügbarkeit (GA) bereit ist, wird diese Funktion der neuesten aktuellen Version hinzugefügt. Wenn die Höherstufung der Funktion zu einer wesentlichen Änderung an der aktuellen Version führen würde, wird die Versionsnummer erhöht, und die neue Version wird die aktuelle Version.
Unsere Entwickler-Community kann unter [UserVoice](https://officespdev.uservoice.com/) Featureanforderungen veröffentlichen, einschließlich Anforderungen für neue Features sowie Anforderungen zur Höherstufung vorhandener Beta-APIs in die aktuelle Version. 

### <a name="current-version"></a>Aktuelle Version

Die aktuelle Version von Microsoft Graph ist Version 1.0. Die Version Microsoft Graph-API /v1.0, die unter `https://graph.microsoft.com/v1.0` verfügbar gemacht wird, enthält Features, die allgemein verfügbar und bereit für die Produktionsverwendung sind. Sie können die Dokumentation nach den v1.0-APIs im Inhaltsverzeichnis durchsuchen.

### <a name="deprecated-and-unsupported-versions"></a>Veraltete und nicht unterstützte Versionen

Es gibt zurzeit keine veralteten Versionen von Microsoft Graph.

## <a name="terms-of-use"></a>Nutzungsbedingungen

Durch Verwendung der Microsoft Graph-APIs stimmen Sie den [Nutzungsbedingungen](https://msdn.microsoft.com/de-DE/cc300389) zu. 

Ihr Feedback ist uns wichtig. Nehmen Sie auf [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) Kontakt mit uns auf. Taggen Sie Ihre Fragen mit {MicrosoftGraph}.
