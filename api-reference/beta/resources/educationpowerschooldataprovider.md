---
title: EducationPowerSchoolDataProvider-Ressource
description: Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn PowerSchool als Eingabe Quelle verwendet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510463"
---
# <a name="educationpowerschooldataprovider-resource"></a>EducationPowerSchoolDataProvider-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) als Eingabe Quelle verwendet wird.

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **connectionUrl** | String | Die Verbindungs-URL für die PowerSchool-Instanz. |
| **clientId** | String |  Die Client-ID, die zum Verbinden mit PowerSchool. |
| client_secret | String |  Der geheime Clientschlüssel zum Authentifizieren der Verbindungs zu der Instanz PowerSchool. |
| **schoolsIds** | Zeichenfolgenauflistung |  Die Liste der Schulen synchronisieren. |
| **schoolYear** | String |  Das Jahr Schule synchronisieren. |
| **allowTeachersInMultipleSchools** | Boolescher Wert |  Gibt an, ob die Quelle mehrere Bezeichner für eine einzelne Student oder Lehrer verfügt. |
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
