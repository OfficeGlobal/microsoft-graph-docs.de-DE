---
title: iosHomeScreenItem-Ressourcentyp
description: Stellt ein Element auf dem iOS-Startbildschirm dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff573a6f7ae0d78113a32514bc312c3920b216f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987622"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="0cc40-103">iosHomeScreenItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0cc40-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="0cc40-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0cc40-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cc40-105">Stellt ein Element auf dem iOS-Startbildschirm dar.</span><span class="sxs-lookup"><span data-stu-id="0cc40-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="0cc40-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0cc40-106">Properties</span></span>
|<span data-ttu-id="0cc40-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0cc40-107">Property</span></span>|<span data-ttu-id="0cc40-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0cc40-108">Type</span></span>|<span data-ttu-id="0cc40-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cc40-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc40-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0cc40-110">displayName</span></span>|<span data-ttu-id="0cc40-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0cc40-111">String</span></span>|<span data-ttu-id="0cc40-112">Name der App</span><span class="sxs-lookup"><span data-stu-id="0cc40-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cc40-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0cc40-113">Relationships</span></span>
<span data-ttu-id="0cc40-114">Keine</span><span class="sxs-lookup"><span data-stu-id="0cc40-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0cc40-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0cc40-115">JSON Representation</span></span>
<span data-ttu-id="0cc40-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0cc40-116">Here is a JSON representation of the resource.</span></span>
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



