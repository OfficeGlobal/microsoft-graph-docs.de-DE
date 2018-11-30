---
title: Ressourcentyp educationIdentityCreationConfiguration
description: Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065161"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>Ressourcentyp educationIdentityCreationConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```