---
title: Ressourcentyp educationSynchronizationError
description: Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.
ms.openlocfilehash: 91a633ab4056e8e86854a0e2d45ae13e22da19a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058767"
---
# <a name="educationsynchronizationerror-resource-type"></a>Ressourcentyp educationSynchronizationError

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-|:-|:-|
| [Abrufen von Synchronisierungsfehler](../api/educationsynchronizationerrors-get.md) | **EducationSynchronizationError** -Auflistung| Gibt die Liste der Synchronisierungsfehler im Zusammenhang mit einem Profil. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **entryType** | string |  Stellt die Sync-Entität (Schule, Abschnitt, Student, Lehrer).       |
| **<ui>errorCode</ui>** | string |  Stellt den Fehlercode für diesen Fehler.         |
| **errorMessage** | string |  Enthält eine Beschreibung des Fehlers.        |
| **joiningValue** | string |  Der eindeutige Bezeichner für den Eintrag.         |
| **recordedDateTime** | DateTimeOffset | Der Zeitpunkt des Auftretens dieses Fehlers.         |
| **reportableIdentifier** | string | Der Bezeichner für diesen Fehlereintrag.       |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
