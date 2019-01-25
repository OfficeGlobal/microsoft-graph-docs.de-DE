---
title: Ressourcentyp oAuth2Permission
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510813"
---
# <a name="oauth2permission-resource-type"></a>Ressourcentyp oAuth2Permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **oAuth2Permission**.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|adminConsentDescription|String|Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.|
|adminConsentDisplayName|String|Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.|
|id|Guid|Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung.|
|isEnabled|Boolescher Wert|Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist). Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden.  An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden.|
|type|String|Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die ein Unternehmensadministrator zugestimmt werden muss.  Mögliche Werte sind "User" oder "Admin".|
|userConsentDescription|String|Berechtigung Hilfe in Zustimmung des Endbenutzers angezeigte Text.|
|userConsentDisplayName|String|Der Anzeigename für die Berechtigung, die in Zustimmung des Endbenutzers angezeigt wird.|
|Wert|Zeichenfolge|Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
