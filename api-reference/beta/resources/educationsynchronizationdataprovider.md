---
title: Ressourcentyp educationSynchronizationDataProvider
description: 'SIS Quellschema darstellt. Dadurch wird das System wissen, wie Sie die eingehenden Daten das Schema Azure Active Directory (AD Azure) zuordnen. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515496"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>Ressourcentyp educationSynchronizationDataProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

SIS Quellschema darstellt. Dadurch wird das System wissen, wie Sie die eingehenden Daten das Schema Azure Active Directory (AD Azure) zuordnen.

> **Hinweis:** Dieser komplexe Typ ist abstrakt. Verweisen Sie auf bestimmten Typen von Datenprovidern aufgeführt.

## <a name="derived-types"></a>Abgeleitete Typen
| Typ | Beschreibung |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | Mit CSV-Dateien verwendet als Eingabe Quelle. |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | Mit PowerSchool verwendet als Eingabe Quelle. |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | Als Eingabe Quelle verwendet mit OneRoster-API. |

## <a name="properties"></a>Eigenschaften

Keine Eigenschaften werden von diesem Typ verfügbar gemacht.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
