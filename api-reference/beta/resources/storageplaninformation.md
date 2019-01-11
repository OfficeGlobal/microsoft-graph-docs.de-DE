---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: bbe4faaffbf53c24d4d0f5b8ea1f5ee1e1966a2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860123"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="7e2aa-102">Ressourcentyp storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="7e2aa-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="7e2aa-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e2aa-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e2aa-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e2aa-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e2aa-105">Die **StoragePlanInformation** Ressource enthält Informationen über das Laufwerk Speicherung Kontingent Pläne.</span><span class="sxs-lookup"><span data-stu-id="7e2aa-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="7e2aa-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e2aa-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a><span data-ttu-id="7e2aa-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e2aa-107">Properties</span></span>

| <span data-ttu-id="7e2aa-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7e2aa-108">Property name</span></span>     | <span data-ttu-id="7e2aa-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7e2aa-109">Type</span></span>      | <span data-ttu-id="7e2aa-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e2aa-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="7e2aa-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="7e2aa-111">upgradeAvailable</span></span>  | <span data-ttu-id="7e2aa-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2aa-112">Boolean</span></span>   | <span data-ttu-id="7e2aa-113">Gibt an, ob einer höheren Speicherung Kontingent Plänen verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="7e2aa-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="7e2aa-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7e2aa-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

