---
title: Ressourcentyp educationIdentityMatchingConfiguration
description: Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.
ms.openlocfilehash: b189735340c121a56c48ae21518989cf8e1634f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065284"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="8861d-105">Ressourcentyp educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="8861d-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="8861d-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8861d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8861d-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8861d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8861d-108">Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten.</span><span class="sxs-lookup"><span data-stu-id="8861d-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="8861d-109">Diese Identitäten enthalten Schüler und Lehrer.</span><span class="sxs-lookup"><span data-stu-id="8861d-109">These identities include students and teachers.</span></span> <span data-ttu-id="8861d-110">Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="8861d-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="8861d-111">**Hinweis:** Wenn diese Ressource ausgewählt ist, werden keine Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="8861d-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="8861d-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8861d-112">Properties</span></span>

| <span data-ttu-id="8861d-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8861d-113">Property</span></span> | <span data-ttu-id="8861d-114">Typ</span><span class="sxs-lookup"><span data-stu-id="8861d-114">Type</span></span> | <span data-ttu-id="8861d-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8861d-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8861d-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="8861d-116">**matchingOptions**</span></span> | <span data-ttu-id="8861d-117">[EducationIdentityMatchingOptions](educationidentitymatchingoptions.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8861d-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="8861d-118">Zuordnung zwischen dem Benutzerkonto und Optionen, die zur eindeutigen Identifizierung den Benutzer zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="8861d-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8861d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8861d-119">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
