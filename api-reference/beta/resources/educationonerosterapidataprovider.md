---
title: EducationOneRosterApiDataProvider-Ressource
description: Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die OneRoster-API als Eingabe Quelle verwendet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527983"
---
# <a name="educationonerosterapidataprovider-resource"></a>EducationOneRosterApiDataProvider-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die [OneRoster-API](https://www.imsglobal.org/activity/onerosterlis) als Eingabe Quelle verwendet wird.

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **connectionUrl** | String | Die Verbindungs-URL für die OneRoster-Instanz. |
| **schoolsIds** | Zeichenfolgenauflistung |  Die Liste der Schule SourcedIds synchronisieren. |
| ProviderName | String | Der Dienstanbieter OneRoster Name gemäß der [Spezifikation OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **connectionSettings** | [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | Verbindungseinstellungen für die OneRoster-Instanz. Muss vom Typ [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) oder [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)sein. |
| **Anpassungen** | [microsoft.graph.educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Optional Anpassung der Synchronisierung Profil angewendet werden soll.|

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
