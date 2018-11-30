---
title: Ressourcentyp educationSynchronizationProfileStatus
description: 'Stellt den Synchronisierungsstatus eines Profils Schule Daten-Synchronisierung. '
ms.openlocfilehash: 6d2c638e1f92a6c3e090cb2bf3bb55e8482bbc4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065947"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Ressourcentyp educationSynchronizationProfileStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Synchronisierungsstatus eines Schule Daten [Synchronisierung Profil](educationsynchronizationprofile.md). 

> **Hinweis:** Updates für die **EducationSynchronizationProfileStatus** möglicherweise aufgrund der asynchrone Verarbeitung im Hintergrund Sync verzögert.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-|:-|:-|
| [Abrufen des Status der Synchronisierung](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Der Status eines bestimmten Synchronisierungsprofils zurückgegeben. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **status** | string | Der Status der Synchronisierung. Mögliche Werte sind: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`. |
| **lastSynchronizationDateTime** | DateTimeOffset | Gibt die Zeit, die beim letzten Änderung im Verzeichnis beobachtet wurden.  |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```