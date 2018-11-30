---
title: Ressourcentyp agreementAcceptance
description: Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.
ms.openlocfilehash: 23221fe88a65b003c8d26aca99eaf1f03d935722
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058145"
---
# <a name="agreementacceptance-resource-type"></a>Ressourcentyp agreementAcceptance

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|agreementFileId|String|Die ID der Vereinbarung-Datei, die vom Benutzer angenommen.|
|agreementId|String|ID des zu.|
|id|String| Schreibgeschützt.|
|recordedDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|state|string| Mögliche Werte sind: `accepted` und `declined`.|
|userDisplayName|String|Der Anzeigename des Benutzers, wenn die Annahme aufgezeichnet wurde.|
|userEmail|String|E-Mail des Benutzers, wenn die Annahme aufgezeichnet wurde.|
|userId|String|ID des Benutzers, der den Lizenzvertrag akzeptiert.|
|userPrincipalName|String|UPN des Benutzers, wenn die Annahme aufgezeichnet wurde.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
