---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kontingent
localization_priority: Normal
ms.openlocfilehash: ce07852592317568254217c7e869f1da7f296a2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525486"
---
# <a name="quota-resource-type"></a>Quota-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **quota**-Ressource enthält Details zu Leerzeichenbeschränkungen auf einer[Laufwerk](drive.md)-Ressource.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| gesamt         | Int64  | Zulässige Speicherplatz in Byte. Schreibgeschützt.                           |
| verwendet          | Int64  | Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.                                      |
| verbleibende     | Int64  | Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt. |
| gelöscht       | Int64  | Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.      |
| state         | string | Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt. |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | Informationen über das Laufwerk Speicherung Kontingent Pläne. Nur in der persönlichen OneDrive.|

### <a name="state-enumeration-values"></a>State Enumerationswerte

| Wert      | Beschreibung                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.                                                                                                                               |
| `nearing`  | Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.                                                                                                                      |
| `critical` | Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.                                                                                                                       |
| `exceeded` | Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird. |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": [
    "Error: /api-reference/beta/resources/quota.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
