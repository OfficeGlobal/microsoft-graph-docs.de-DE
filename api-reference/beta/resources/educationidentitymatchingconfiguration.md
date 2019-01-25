---
title: Ressourcentyp educationIdentityMatchingConfiguration
description: Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520312"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="08ff6-105">Ressourcentyp educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="08ff6-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08ff6-106">Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten.</span><span class="sxs-lookup"><span data-stu-id="08ff6-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="08ff6-107">Diese Identitäten enthalten Schüler und Lehrer.</span><span class="sxs-lookup"><span data-stu-id="08ff6-107">These identities include students and teachers.</span></span> <span data-ttu-id="08ff6-108">Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="08ff6-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="08ff6-109">**Hinweis:** Wenn diese Ressource ausgewählt ist, werden keine Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="08ff6-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="08ff6-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08ff6-110">Properties</span></span>

| <span data-ttu-id="08ff6-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08ff6-111">Property</span></span> | <span data-ttu-id="08ff6-112">Typ</span><span class="sxs-lookup"><span data-stu-id="08ff6-112">Type</span></span> | <span data-ttu-id="08ff6-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08ff6-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="08ff6-114">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="08ff6-114">**matchingOptions**</span></span> | <span data-ttu-id="08ff6-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="08ff6-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="08ff6-116">Zuordnung zwischen dem Benutzerkonto und Optionen, die zur eindeutigen Identifizierung den Benutzer zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="08ff6-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08ff6-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08ff6-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
