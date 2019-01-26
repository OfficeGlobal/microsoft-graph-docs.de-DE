---
title: Ressourcentyp synchronizationJobRestartCriteria
description: 'Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization_synchronizationjob_restart.md) Aktion.'
localization_priority: Normal
ms.openlocfilehash: 960bfa56d0bb6921ca971722d894d1b837bfab49
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572304"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Ressourcentyp synchronizationJobRestartCriteria

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization-synchronizationjob-restart.md) Aktion.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resetScope|String| Durch Trennzeichen getrennte Kombination der folgenden Werte: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`. Verwendung `Full` Wenn Sie alle Optionen möchten.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
