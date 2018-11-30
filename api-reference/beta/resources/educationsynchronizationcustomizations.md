---
title: Ressourcentyp educationSynchronizationCustomizations
description: Enthält die Liste der Entitäten, Synchronisierung und ihre Anpassungen an, sofern vorhanden.
ms.openlocfilehash: d694c5ea1136d38e11ff3f1aca0ad0fde34b9d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062407"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>Ressourcentyp educationSynchronizationCustomizations

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| **student** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für eine Student-Entität.         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für eine Entität Lehrer.         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Anpassung für die Student-Registrierung.           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       Anpassung für eine Teilnehmerliste Lehrer.    |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
