---
title: Ressourcentyp permissionScope
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **oauth2Permissions** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **OAuth2Permission**.
ms.openlocfilehash: b15ee9901632fca113d944000847c953e85be58c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063641"
---
# <a name="permissionscope-resource-type"></a>Ressourcentyp permissionScope

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **oauth2Permissions** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **OAuth2Permission**.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|adminConsentDescription|String| Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird. |
|adminConsentDisplayName|String| Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird. |
|id|Guid| Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung. |
|isEnabled|Boolescher Wert| Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist). Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden. An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden. |
|Ursprung|String| Für die interne Verwendung. |
|Typ|String| Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die von einem Administrator der Firma zugestimmt werden muss. Mögliche Werte sind *Benutzer* oder *Administrator*. |
|userConsentDescription|String| Berechtigung Hilfetext, die in der Genehmigung durch den Endbenutzer angezeigt wird. |
|userConsentDisplayName|String| Der Anzeigename für die Berechtigung, die in der Genehmigung durch den Endbenutzer angezeigt wird. |
|Wert|Zeichenfolge| Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->