---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d27d632050a288966e5f1596e94243b08b40726e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981749"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="9e5f6-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e5f6-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="9e5f6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e5f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e5f6-105">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="9e5f6-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="9e5f6-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="9e5f6-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e5f6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e5f6-107">Properties</span></span>
|<span data-ttu-id="9e5f6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e5f6-108">Property</span></span>|<span data-ttu-id="9e5f6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9e5f6-109">Type</span></span>|<span data-ttu-id="9e5f6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e5f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e5f6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9e5f6-111">displayName</span></span>|<span data-ttu-id="9e5f6-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e5f6-112">String</span></span>|<span data-ttu-id="9e5f6-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="9e5f6-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="9e5f6-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="9e5f6-114">bundleID</span></span>|<span data-ttu-id="9e5f6-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e5f6-115">String</span></span>|<span data-ttu-id="9e5f6-116">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="9e5f6-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e5f6-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e5f6-117">Relationships</span></span>
<span data-ttu-id="9e5f6-118">Keine</span><span class="sxs-lookup"><span data-stu-id="9e5f6-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e5f6-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e5f6-119">JSON Representation</span></span>
<span data-ttu-id="9e5f6-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e5f6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



