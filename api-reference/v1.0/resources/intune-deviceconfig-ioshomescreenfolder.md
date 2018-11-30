---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
ms.openlocfilehash: 1b3d4c75ec177eb4c277c7f5bc7f76ccf550d30b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016502"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="8cff6-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8cff6-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="8cff6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8cff6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cff6-105">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="8cff6-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="8cff6-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8cff6-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cff6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8cff6-107">Properties</span></span>
|<span data-ttu-id="8cff6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8cff6-108">Property</span></span>|<span data-ttu-id="8cff6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8cff6-109">Type</span></span>|<span data-ttu-id="8cff6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8cff6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cff6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8cff6-111">displayName</span></span>|<span data-ttu-id="8cff6-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8cff6-112">String</span></span>|<span data-ttu-id="8cff6-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="8cff6-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="8cff6-114">Seiten</span><span class="sxs-lookup"><span data-stu-id="8cff6-114">pages</span></span>|<span data-ttu-id="8cff6-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8cff6-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="8cff6-116">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="8cff6-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="8cff6-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8cff6-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cff6-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8cff6-118">Relationships</span></span>
<span data-ttu-id="8cff6-119">Keine</span><span class="sxs-lookup"><span data-stu-id="8cff6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8cff6-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8cff6-120">JSON Representation</span></span>
<span data-ttu-id="8cff6-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8cff6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```



