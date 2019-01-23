---
title: Ressourcentyp educationIdentityCreationConfiguration
description: Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 7c05d810c017f57f738d188a8edef5d0560415fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395685"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>Ressourcentyp educationIdentityCreationConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
