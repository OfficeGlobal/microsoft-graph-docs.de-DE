---
title: EducationOneRosterApiDataProvider-Ressource
description: Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die OneRoster-API als Eingabe Quelle verwendet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 681a3331aba7bc84ac80911c4be8076d104f8a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938146"
---
# <a name="educationonerosterapidataprovider-resource"></a>EducationOneRosterApiDataProvider-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die [OneRoster-API](https://www.imsglobal.org/activity/onerosterlis) als Eingabe Quelle verwendet wird.

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **connectionUrl** | Zeichenfolge | Die Verbindungs-URL für die OneRoster-Instanz. |
| **schoolsIds** | Collection von Objekten des Typs „String“ |  Die Liste der Schule SourcedIds synchronisieren. |
| **providerName** | Zeichenfolge | Der Dienstanbieter OneRoster Name gemäß der [Spezifikation OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **connectionSettings** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | Verbindungseinstellungen für die OneRoster-Instanz. Muss vom Typ [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) oder [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)sein. |
| **Anpassungen** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Optional Anpassung der Synchronisierung Profil angewendet werden soll.|

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
