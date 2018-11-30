---
title: Ressourcentyp educationFileSynchronizationVerificationMessage
description: Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum Starten der Synchronisierung für die CSV-basierte Schule datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.
ms.openlocfilehash: cf685e0619c5600340df68ba86ecaef11a8a435d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058527"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>Ressourcentyp educationFileSynchronizationVerificationMessage

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum [Starten Sie die Synchronisierung](../api/educationsynchronizationprofile-start.md) für Schule CSV-basierte datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **type** | string | Typ der Nachricht. Mögliche Werte sind: `error`, `warning` und `information`. | 
| **Dateiname** | string | Quelldatei, die den Fehler enthält. |
| **description** | string | Ausführliche Informationen zu den Nachrichtentyp. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```