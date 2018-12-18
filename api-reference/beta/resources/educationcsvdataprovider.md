---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
ms.openlocfilehash: 1a816d4e176147d549381465154e35cf0a821b98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317899"
---
# <a name="educationcsvdataprovider-resource-type"></a>Ressourcentyp educationCsvDataProvider

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **Anpassungen** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Optional Anpassungen Synchronisierung Profil angewendet werden soll.|

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
