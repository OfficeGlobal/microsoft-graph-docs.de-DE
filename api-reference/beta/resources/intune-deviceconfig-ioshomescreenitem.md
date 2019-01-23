---
title: iosHomeScreenItem-Ressourcentyp
description: Stellt ein Element auf dem iOS-Startbildschirm dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 190726b8ee7411a5ce53f8e2802ddf38e0e6b9ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408418"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="aed58-103">iosHomeScreenItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aed58-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="aed58-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="aed58-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aed58-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aed58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aed58-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aed58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aed58-107">Stellt ein Element auf dem iOS-Startbildschirm dar.</span><span class="sxs-lookup"><span data-stu-id="aed58-107">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="aed58-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aed58-108">Properties</span></span>
|<span data-ttu-id="aed58-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aed58-109">Property</span></span>|<span data-ttu-id="aed58-110">Typ</span><span class="sxs-lookup"><span data-stu-id="aed58-110">Type</span></span>|<span data-ttu-id="aed58-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aed58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed58-112">displayName</span><span class="sxs-lookup"><span data-stu-id="aed58-112">displayName</span></span>|<span data-ttu-id="aed58-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aed58-113">String</span></span>|<span data-ttu-id="aed58-114">Name der App</span><span class="sxs-lookup"><span data-stu-id="aed58-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="aed58-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aed58-115">Relationships</span></span>
<span data-ttu-id="aed58-116">Keine</span><span class="sxs-lookup"><span data-stu-id="aed58-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aed58-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aed58-117">JSON Representation</span></span>
<span data-ttu-id="aed58-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aed58-118">Here is a JSON representation of the resource.</span></span>
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




