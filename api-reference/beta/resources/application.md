---
title: Anwendung Ressourcentyp
description: 'Stellt eine Anwendung dar. Jede Anwendung, die Authentifizierung mit Azure Active Directory (AD Azure) mit dem Konfigurieren beauftragt muss in einem Verzeichnis registriert werden. Registrierung Anwendung umfasst darüber informiert Azure AD über die Anwendung, einschließlich der URL, in dem es wurde gefunden, die URL zum Senden von Antworten nach der Authentifizierung, den URI zum Identifizieren der Anwendung und vieles mehr. Weitere Informationen finden Sie unter Grundlagen der Registrieren einer Anwendung in Azure Active Directory. Erbt von directoryObject. '
ms.openlocfilehash: 66da35183b84d42d69d603cc840ba948d60d7bed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062798"
---
# <a name="application-resource-type"></a>Anwendung Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Anwendung dar. Jede Anwendung, die Authentifizierung mit Azure Active Directory (AD Azure) mit dem Konfigurieren beauftragt muss in einem Verzeichnis registriert werden. Registrierung Anwendung umfasst darüber informiert Azure AD über die Anwendung, einschließlich der URL, in dem es wurde gefunden, die URL zum Senden von Antworten nach der Authentifizierung, den URI zum Identifizieren der Anwendung und vieles mehr. Weitere Informationen finden Sie unter [Grundlagen der Registrieren einer Anwendung in Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Erbt von [directoryObject](directoryobject.md). 

> **Hinweis:** Änderungen an der Anwendung Ressourcentyp sind derzeit in der Entwicklung. Weitere Informationen finden Sie unter [bekannte Probleme mit Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/application-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Abrufen der Anwendung](../api/application-get.md) | Anwendung |Lesen Sie Eigenschaften und Beziehungen des Application-Objekts.|
|[Erstellen der Anwendung](../api/application-post-applications.md) | Anwendung | (Register) erstellt eine neue Anwendung.|
|[Liste applications](../api/application-list.md) | Anwendung | Abrufen der Liste der Programme in der Organisation. |
|[Aktualisieren der Anwendung](../api/application-update.md) | Anwendung |Application-Objekt zu aktualisieren. |
|[Löschen der Anwendung](../api/application-delete.md) | Keines |Application-Objekt zu löschen. |
|[Zugewiesen-Listenrichtlinien](../api/policy-list-assigned.md)| Auflistung von [Gruppenrichtlinien](policy.md)| Rufen Sie alle Richtlinien, die auf dieses Objekt zugewiesen.|
|[Ersteller-Besitzer](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Erstellen Sie einen neuen Besitzer durch die Veröffentlichung auf der Besitzer-Auflistung.|
|[Besitzer auflisten](../api/application-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Abrufen eines Besitzers Auflistung-Objekts.|
|[delta](../api/application-delta.md)|Application-Auflistung| Rufen Sie inkrementelle Änderungen für Applikationen. |
|[Erstellen von Anrufen](../api/application-post-calls.md)|[Anruf](call.md)|Erstellen Sie einen neuen Anruf, indem Sie das Veröffentlichen in der Auflistung Anrufe.|
|[Erstellen von online-Besprechung](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Erstellen einer neuen onlinebesprechung durch die Veröffentlichung auf der OnlineMeetings-Auflistung.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|API|[API](api.md)| Gibt die Einstellungen für eine API-Anwendung. |
|appId| Zeichenfolge | Der eindeutige Bezeichner für die Anwendung, die eine Anwendung von Azure AD zugewiesen ist. Lässt keine Nullwerte zu. Schreibgeschützt. |
|appRoles|[AppRole](approle.md) -Auflistung|Die Auflistung der Anwendungsrollen, die eine Anwendung deklarieren kann. Diese Funktionen können Benutzer, Gruppen oder Dienstprinzipale zugewiesen werden. Lässt keine Nullwerte zu.|
|createdDateTime|DateTimeOffset| Das Datum und die Zeit, die die Anwendung registriert wurde. |
|deletedDateTime|DateTimeOffset| Das Datum und die Zeit, die die Anwendung gelöscht wurde. |
|displayName|String|Der Anzeigename für die Anwendung. |
|id|String|Der eindeutige Bezeichner für die Anwendung. Geerbt von [directoryObject](directoryobject.md). Schlüssel. Lässt keine Nullwerte zu. Schreibgeschützt. |
|identifierUris|Collection von Objekten des Typs „String“| Die URIs, die die Anwendung zu bestimmen. Weitere Informationen finden Sie unter [Application Objects und Service Principal-Objekte](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Der *any* -Operator ist für Filterausdrücke auf mehrwertige Eigenschaften erforderlich. Lässt keine Nullwerte zu. |
|Info|[informationalUrl](informationalurl.md)| Grundlegende Profilinformationen der Anwendung. |
|isFallbackPublicClient|Boolesch| Gibt an, welche fallback app als öffentliche Client wie eine installierte app auf einem mobilen Gerät ausführen. Der Standardwert ist *false,* was den fallback-app-Typ bedeutet vertrauliche Client wie Web app. Es gibt bestimmte Szenarien Azure AD kann nicht, in dem den Client-app-Typ (z. B. [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) Fluss, in dem sie konfiguriert ist, ohne eine umleitungs-URI) ermitteln. In diesen Fällen wird Azure AD app Type basierend auf dem Wert dieser Eigenschaft interpretiert.|
|keyCredentials|[KeyCredential](keycredential.md) -Auflistung|Die Auflistung der wichtigsten Anmeldeinformationen der Anwendung nicht zugeordnete NULL-Werte zulässt. |
|logo|Stream|Das Hauptfenster Logo für die Anwendung. Lässt keine Nullwerte zu. |
|optionalClaims|optionalClaims| Reserviert für zukünftige Verwendung. |
|orgRestrictions|Collection von Objekten des Typs „String“| Reserviert für zukünftige Verwendung. |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |Gibt die Altersfreigabe Einstellungen für eine Anwendung.|
|passwordCredentials|[PasswordCredential](passwordcredential.md) -Auflistung|Die Auflistung von Anmeldeinformationen, die mit der Anwendung verbunden sind. Lässt keine Nullwerte zu.|
|publicClient|[publicClient](publicclient.md)| Gibt die Einstellungen für installierte Clients wie desktop oder mobilen Geräten. |
|publisherDomain| String | Die überprüften Publisher-Domäne für die Anwendung. Schreibgeschützt.|
|requiredResourceAccess|[RequiredResourceAccess](requiredresourceaccess.md) -Auflistung|Gibt die Ressourcen, die diese Anwendung benötigt Zugriff auf und den Satz von OAuth berechtigungsbereiche und Anwendungsrollen, die unter jeder dieser Ressourcen benötigt werden. Diese vor Konfiguration erforderlichen Ressourcenzugriff Laufwerke der Zustimmung wünschen. Lässt keine Nullwerte zu.|
|signInAudience | String | Gibt an, welche Microsoft-Konten für die aktuelle Anwendung unterstützt werden. Unterstützte Werte sind:<ul><li>**AzureADMyOrg**: Benutzer mit einer Microsoft arbeiten oder Schule Konto in meiner Organisation Azure AD-Mandanten (d. h. mit einem einzelnen Mandanten)</li><li>**AzureADMultipleOrgs**: Benutzer mit einer Microsoft arbeiten oder Schule Konto in der Organisation Azure AD-Mandanten (d. h. mit mehreren Mandanten)</li> <li>**AzureADandPersonalMicrosoftAccount**: Benutzer mit einem persönlichen Microsoft-Konto oder ein Konto arbeiten oder Schule in der Organisation Azure AD-Mandanten</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|-Tags hinzugefügtes Markup|Collection von Objekten des Typs „String“| Benutzerdefinierte Zeichenfolgen, die zum Kategorisieren und Identifizieren der Anwendung verwendet werden können. |
|web|[web](web.md)| Gibt die Einstellungen für eine Webanwendung. |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ | Beschreibung |
|:---------------|:--------|:----------|
|Anrufe           |[rufen Sie](call.md) -Auflistung                  |Schreibgeschützt. Lässt Nullwerte zu.|
|connectorGroup|[connectorGroup](connectorgroup.md)| Die ConnectorGroup ist die Anwendung mit Azure AD-Anwendungsproxy verwendet. Lässt Nullwerte zu.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Schreibgeschützt.|
|onlineMeetings  |[OnlineMeeting](onlinemeeting.md) -Auflistung|Schreibgeschützt. Lässt Nullwerte zu.|
|owners|[directoryObject](directoryobject.md)-Sammlung|Directory-Objekte, die Besitzer der Anwendung sind. Die Besitzer sind eine Reihe von nicht-Administrator-Benutzer, die berechtigt sind, dieses Objekt zu ändern. Erfordert Version 2013-11-08 oder höher. Schreibgeschützt. Lässt Nullwerte zu.|
|Richtlinie|Auflistung von [Gruppenrichtlinien](policy.md)|Die Richtlinien für diese Anwendung zugewiesen.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
