---
title: Ressourcentyp educationSynchronizationCustomizations
description: Enthält die Liste der Entitäten, Synchronisierung und ihre Anpassungen an, sofern vorhanden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523253"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>Ressourcentyp educationSynchronizationCustomizations

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält die Liste der Entitäten, Synchronisierung und ihre [Anpassungen](educationsynchronizationcustomization.md), sofern vorhanden.

> **Hinweis:** Anpassung von Eigenschaften für die Synchronisierung gilt nicht für die **StudentEnrollment** und **TeacherRoster** -Entitäten.

Diese Ressource ist Mitglied der folgenden Datenanbieter:

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **School** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für eine Schule Entität.        |
| **section** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für eine Entität im Abschnitt.         |
| student | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für eine Student-Entität.         |
| teacher | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für eine Entität Lehrer.         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für die Student-Registrierung.           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       Anpassung für eine Teilnehmerliste Lehrer.    |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
