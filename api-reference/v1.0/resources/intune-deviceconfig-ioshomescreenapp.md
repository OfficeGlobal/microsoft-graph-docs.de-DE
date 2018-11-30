---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
ms.openlocfilehash: ff749f7166da2d20bfd632e0c595b33f7b1e9fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018764"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="a2e13-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a2e13-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="a2e13-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2e13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2e13-105">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="a2e13-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="a2e13-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a2e13-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2e13-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a2e13-107">Properties</span></span>
|<span data-ttu-id="a2e13-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2e13-108">Property</span></span>|<span data-ttu-id="a2e13-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a2e13-109">Type</span></span>|<span data-ttu-id="a2e13-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2e13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e13-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a2e13-111">displayName</span></span>|<span data-ttu-id="a2e13-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2e13-112">String</span></span>|<span data-ttu-id="a2e13-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="a2e13-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a2e13-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="a2e13-114">bundleID</span></span>|<span data-ttu-id="a2e13-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2e13-115">String</span></span>|<span data-ttu-id="a2e13-116">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="a2e13-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2e13-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a2e13-117">Relationships</span></span>
<span data-ttu-id="a2e13-118">Keine</span><span class="sxs-lookup"><span data-stu-id="a2e13-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2e13-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a2e13-119">JSON Representation</span></span>
<span data-ttu-id="a2e13-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a2e13-120">Here is a JSON representation of the resource.</span></span>
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



