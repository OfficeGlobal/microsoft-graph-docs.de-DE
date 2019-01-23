---
title: EducationPowerSchoolDataProvider-Ressource
description: Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn PowerSchool als Eingabe Quelle verwendet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4028170c2780cee426ec961a44b51e0362b0187f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406920"
---
# <a name="educationpowerschooldataprovider-resource"></a>EducationPowerSchoolDataProvider-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) als Eingabe Quelle verwendet wird.

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **connectionUrl** | Zeichenfolge | Die Verbindungs-URL für die PowerSchool-Instanz. |
| **clientId** | Zeichenfolge |  Die Client-ID, die zum Verbinden mit PowerSchool. |
| **clientSecret** | Zeichenfolge |  Der geheime Clientschlüssel zum Authentifizieren der Verbindungs zu der Instanz PowerSchool. |
| **schoolsIds** | Zeichenfolgenauflistung |  Die Liste der Schulen synchronisieren. |
| **schoolYear** | Zeichenfolge |  Das Jahr Schule synchronisieren. |
| **allowTeachersInMultipleSchools** | Boolean |  Gibt an, ob die Quelle mehrere Bezeichner für eine einzelne Student oder Lehrer verfügt. |
| **Anpassungen** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Optional Anpassung der Synchronisierung Profil angewendet werden soll.|

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
