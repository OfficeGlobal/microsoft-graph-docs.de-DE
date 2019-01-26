---
title: Ressourcentyp privilegedRoleSettings
description: Stellt die Einstellungen für eine privilegierten Rolle.
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577151"
---
# <a name="privilegedrolesettings-resource-type"></a>Ressourcentyp privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Einstellungen für eine privilegierten Rolle.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSettings-Objekts.|
|[PrivilegedRoleSettings aktualisieren](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings-Objekt zu aktualisieren.|
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|elevationDuration| Zeichenfolge (Zeitstempel) |Die Dauer, wenn die Rolle aktiviert ist.|
|id| Zeichenfolge (ID)| Der eindeutige Bezeichner für die rolleneinstellungen. Schreibgeschützt.|
|isMfaOnElevationConfigurable|Boolescher Wert|**true,** Wenn MfaOnElevation konfigurierbar ist. **false,** Wenn MfaOnElevation nicht konfigurierbar ist.|
|lastGlobalAdmin|Boolescher Wert|Verwendet nur intern.|
|maxElavationDuration| Zeichenfolge (ID)| |Maximale Dauer für die aktivierte Rolle.|
|mfaOnElevation|Boolescher Wert|**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren. **false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.|
|minElevationDuration|Zeichenfolge (ID)||Minimale Dauer für die aktivierte Rolle.|
|notificationToUserOnElevation|Boolescher Wert|**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist. **false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.|
|ticketingInfoOnElevation|Boolescher Wert|**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren. **false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.|
|approvalOnElevation|Boolescher Wert|**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren. **false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.|
|approverIds| Zeichenfolgenauflistung |Liste der Genehmigung-Ids, wenn die Genehmigung für die Aktivierung erforderlich ist.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": [ "String (identifier)" ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
