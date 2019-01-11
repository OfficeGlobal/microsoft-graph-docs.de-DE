---
title: Ressourcentyp educationIdentityMatchingConfiguration
description: Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.
localization_priority: Normal
ms.openlocfilehash: 807029f45875bdcf7691a112d515831f2f2283dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877938"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>Ressourcentyp educationIdentityMatchingConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.

> **Hinweis:** Wenn diese Ressource ausgewählt ist, werden keine Benutzer erstellt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **matchingOptions** | [EducationIdentityMatchingOptions](educationidentitymatchingoptions.md) -Auflistung | Zuordnung zwischen dem Benutzerkonto und Optionen, die zur eindeutigen Identifizierung den Benutzer zu aktualisieren. |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
