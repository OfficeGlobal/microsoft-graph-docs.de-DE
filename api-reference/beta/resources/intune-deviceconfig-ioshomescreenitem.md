---
title: iosHomeScreenItem-Ressourcentyp
description: Stellt ein Element auf dem iOS-Startbildschirm dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 477be5c509ab4d062a695c4b8df7eb00af6f51fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962604"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="c52b5-103">iosHomeScreenItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c52b5-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="c52b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c52b5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c52b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c52b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c52b5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c52b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c52b5-107">Stellt ein Element auf dem iOS-Startbildschirm dar.</span><span class="sxs-lookup"><span data-stu-id="c52b5-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="c52b5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c52b5-108">Properties</span></span>
|<span data-ttu-id="c52b5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c52b5-109">Property</span></span>|<span data-ttu-id="c52b5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c52b5-110">Type</span></span>|<span data-ttu-id="c52b5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c52b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c52b5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c52b5-112">displayName</span></span>|<span data-ttu-id="c52b5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c52b5-113">String</span></span>|<span data-ttu-id="c52b5-114">Name der App</span><span class="sxs-lookup"><span data-stu-id="c52b5-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c52b5-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c52b5-115">Relationships</span></span>
<span data-ttu-id="c52b5-116">Keine</span><span class="sxs-lookup"><span data-stu-id="c52b5-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c52b5-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c52b5-117">JSON Representation</span></span>
<span data-ttu-id="c52b5-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c52b5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





