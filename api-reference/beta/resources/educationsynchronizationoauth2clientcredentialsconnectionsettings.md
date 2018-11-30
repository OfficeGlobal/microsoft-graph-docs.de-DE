---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource
description: Wenn OAuth2 Client Anmeldeinformationen Grant in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.
ms.openlocfilehash: 901fabb802d4ed5fa0c99538e52b9a07199eb298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063873"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wenn [OAuth2 Client Anmeldeinformationen Grant](https://tools.ietf.org/html/rfc6749#section-4.4) in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.

[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **tokenUrl** | String | Die URL für den Datenanbieter Zugriffstoken abgerufen. |
| **scope** | String | [Der Bereich der Access-Anforderung](https://tools.ietf.org/html/rfc6749#section-3.3). |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
