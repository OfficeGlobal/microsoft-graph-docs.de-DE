---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb4d08a2a6750310a825f66ecfb0017abacd36fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878569"
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
