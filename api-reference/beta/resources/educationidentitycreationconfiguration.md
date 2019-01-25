---
title: Ressourcentyp educationIdentityCreationConfiguration
description: Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511401"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>Ressourcentyp educationIdentityCreationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.

> **Hinweis:** Wenn Sie die verzeichnissynchronisierung aktiviert die Synchronisierung zwischen der lokalen Active Directory und Azure Active Directory (AD Azure) haben, verwenden Sie stattdessen die [EducationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) -Ressource.

[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)abgeleitet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **userDomains** | [EducationIdentityDomain](educationidentitydomain.md) -Auflistung |  Stellt die Liste der Domänen pro Benutzertyp verwenden.  |


## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
