---
title: Ressourcentyp privilegedRoleSettings
description: Stellt die Einstellungen für eine privilegierten Rolle.
localization_priority: Normal
ms.openlocfilehash: 971c48ce3ecdd2a219a111f3a11884377e20430c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842742"
---
# <a name="privilegedrolesettings-resource-type"></a>Ressourcentyp privilegedRoleSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Einstellungen für eine privilegierten Rolle.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSettings-Objekts.|
|[PrivilegedRoleSettings aktualisieren](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings-Objekt zu aktualisieren.|
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|elevationDuration|duration|Die Dauer, wenn die Rolle aktiviert ist.|
|id|string| Der eindeutige Bezeichner für die rolleneinstellungen. Schreibgeschützt.|
|isMfaOnElevationConfigurable|Boolean|**true,** Wenn MfaOnElevation konfigurierbar ist. **false,** Wenn MfaOnElevation nicht konfigurierbar ist.|
|lastGlobalAdmin|Boolean|Verwendet nur intern.|
|maxElavationDuration|duration|Maximale Dauer für die aktivierte Rolle.|
|mfaOnElevation|Boolean|**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren. **false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.|
|minElevationDuration|duration|Minimale Dauer für die aktivierte Rolle.|
|notificationToUserOnElevation|Boolean|**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist. **false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.|
|ticketingInfoOnElevation|Boolean|**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren. **false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.|
|approvalOnElevation|Boolean|**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren. **false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.|
|approverIds|Array|Liste der Genehmigung-Ids, wenn die Genehmigung für die Aktivierung erforderlich ist.|

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
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
