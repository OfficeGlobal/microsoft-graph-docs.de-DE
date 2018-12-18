---
title: Ressourcentyp educationSynchronizationProfileStatus
description: 'Stellt den Synchronisierungsstatus eines Profils Schule Daten-Synchronisierung. '
author: mmast-msft
ms.openlocfilehash: c92ba2226b28896f8df89a7aee66602651344154
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325998"
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