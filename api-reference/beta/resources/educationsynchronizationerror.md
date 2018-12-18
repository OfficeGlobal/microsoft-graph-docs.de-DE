---
title: Ressourcentyp educationSynchronizationError
description: Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.
author: mmast-msft
ms.openlocfilehash: d950e906a506c3cf1ee5bc5b627200dc79c1d0fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336001"
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
