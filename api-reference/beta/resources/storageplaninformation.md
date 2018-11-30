---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
ms.openlocfilehash: 07552f405ec8c5d6ae8345a8238cd8aec3763b11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063149"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="9b110-102">Ressourcentyp storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="9b110-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="9b110-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b110-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b110-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b110-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b110-105">Die **StoragePlanInformation** Ressource enthält Informationen über das Laufwerk Speicherung Kontingent Pläne.</span><span class="sxs-lookup"><span data-stu-id="9b110-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="9b110-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9b110-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="9b110-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9b110-107">Properties</span></span>

| <span data-ttu-id="9b110-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="9b110-108">Property name</span></span>     | <span data-ttu-id="9b110-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9b110-109">Type</span></span>      | <span data-ttu-id="9b110-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b110-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="9b110-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="9b110-111">upgradeAvailable</span></span>  | <span data-ttu-id="9b110-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9b110-112">Boolean</span></span>   | <span data-ttu-id="9b110-113">Gibt an, ob einer höheren Speicherung Kontingent Plänen verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="9b110-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="9b110-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9b110-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

