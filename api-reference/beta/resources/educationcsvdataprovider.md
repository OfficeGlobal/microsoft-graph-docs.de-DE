---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ef77671f862a0b59b5697b76bb54dc20e42856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952755"
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
