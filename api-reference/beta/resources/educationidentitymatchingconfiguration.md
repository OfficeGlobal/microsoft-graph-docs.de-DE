---
title: Ressourcentyp educationIdentityMatchingConfiguration
description: Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ded27e432219a247bf9c03c21f8ebd0054183eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411330"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="b9f9f-105">Ressourcentyp educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9f9f-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="b9f9f-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9f9f-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9f9f-108">Definiert die Einstellungen für den Abgleich Schule Daten Profil Identitäten.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="b9f9f-109">Diese Identitäten enthalten Schüler und Lehrer.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-109">These identities include students and teachers.</span></span> <span data-ttu-id="b9f9f-110">Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="b9f9f-111">**Hinweis:** Wenn diese Ressource ausgewählt ist, werden keine Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="b9f9f-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9f9f-112">Properties</span></span>

| <span data-ttu-id="b9f9f-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9f9f-113">Property</span></span> | <span data-ttu-id="b9f9f-114">Typ</span><span class="sxs-lookup"><span data-stu-id="b9f9f-114">Type</span></span> | <span data-ttu-id="b9f9f-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9f9f-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b9f9f-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="b9f9f-116">**matchingOptions**</span></span> | <span data-ttu-id="b9f9f-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b9f9f-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="b9f9f-118">Zuordnung zwischen dem Benutzerkonto und Optionen, die zur eindeutigen Identifizierung den Benutzer zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="b9f9f-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9f9f-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9f9f-119">JSON representation</span></span>
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
