---
title: Ressourcentyp educationFileSynchronizationVerificationMessage
description: Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum Starten der Synchronisierung für die CSV-basierte Schule datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845514"
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
