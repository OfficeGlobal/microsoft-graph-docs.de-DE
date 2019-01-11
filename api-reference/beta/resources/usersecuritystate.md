---
title: Ressourcentyp userSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: dd471b06f20327eb38734276ea0562ab35db6358
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810115"
---
# <a name="usersecuritystate-resource-type"></a>Ressourcentyp userSecurityState

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Statusinformationen über das Benutzerkonto enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|aadUserId|String|AAD Benutzer Objekt-ID (GUID) - die physische/multi-account Benutzerentität darstellt.|
|accountName|String|Kontoname des Benutzerkontos (ohne Active Directory-Domäne oder DNS-Domäne) - (auch als bezeichnet `mailNickName`).|
|Domänname|Zeichenfolge|NetBIOS/Active Directory-Domäne des Benutzerkontos (d. h., im Format Domäne\Konto).|
|emailRole|emailRole|Für e-Mail-bezogene Alerts - des Benutzerkontos e-Mail 'Role'. Mögliche Werte sind: `unknown`, `sender` und `recipient`.|
|isVpn|Boolean|Gibt an, ob der Benutzer über ein VPN angemeldet.|
|logonDateTime|DateTimeOffset|Zeitpunkt der Anmeldung bei der aufgetreten ist. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|logonId|String|Benutzer-ID|
|logonIp|String|IP-Adresse, die von die Anforderung-Anmeldung stammt.|
|logonLocation|String|Speicherort (nach Zuordnung von IP-Adresse) ein Benutzer anmelden Ereignis von diesem Benutzer zugeordnet.|
|logonType|logonType|-Methode des Benutzers anmelden. Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.|
|onPremisesSecurityIdentifier|String|Active Directory (lokal) Sicherheits-ID (SID) des Benutzers.|
|riskScore|String|Provider-generiert/berechnet Risiko Bewertung des Benutzerkontos. Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.|
|userAccountType|userAccountSecurityType|Typ des Benutzerkontos (Gruppenmitgliedschaft) pro Windows-Definition. Mögliche Werte: sind `unknown`, `standard`, `power` und `administrator`.|
|userPrincipalName|String|Benutzer-Anmeldename - Internetformat: (Benutzerkontonamen) @(Konto DNS-Domänennamen).|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
