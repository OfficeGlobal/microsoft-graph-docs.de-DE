---
title: EducationPowerSchoolDataProvider-Ressource
description: Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn PowerSchool als Eingabe Quelle verwendet wird.
ms.openlocfilehash: 4c58d3b8baf1569aaeff68375b2dd3643db8b063
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063536"
---
# <a name="educationpowerschooldataprovider-resource"></a>EducationPowerSchoolDataProvider-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) als Eingabe Quelle verwendet wird.

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **connectionUrl** | String | Die Verbindungs-URL für die PowerSchool-Instanz. |
| **clientId** | String |  Die Client-ID, die zum Verbinden mit PowerSchool. |
| **clientSecret** | String |  Der geheime Clientschlüssel zum Authentifizieren der Verbindungs zu der Instanz PowerSchool. |
| **schoolsIds** | Collection von Objekten des Typs „String“ |  Die Liste der Schulen synchronisieren. |
| **schoolYear** | String |  Das Jahr Schule synchronisieren. |
| **allowTeachersInMultipleSchools** | Boolesch |  Gibt an, ob die Quelle mehrere Bezeichner für eine einzelne Student oder Lehrer verfügt. |
| **Anpassungen** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Optional Anpassung der Synchronisierung Profil angewendet werden soll.|

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
