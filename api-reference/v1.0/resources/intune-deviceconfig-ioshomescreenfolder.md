---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
ms.openlocfilehash: 251f854a0038c905175b863e2c19dd638c49b452
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302800"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="a0852-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a0852-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="a0852-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a0852-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0852-105">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="a0852-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="a0852-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a0852-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0852-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a0852-107">Properties</span></span>
|<span data-ttu-id="a0852-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0852-108">Property</span></span>|<span data-ttu-id="a0852-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a0852-109">Type</span></span>|<span data-ttu-id="a0852-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0852-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0852-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a0852-111">displayName</span></span>|<span data-ttu-id="a0852-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0852-112">String</span></span>|<span data-ttu-id="a0852-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="a0852-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a0852-114">Seiten</span><span class="sxs-lookup"><span data-stu-id="a0852-114">pages</span></span>|<span data-ttu-id="a0852-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a0852-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="a0852-116">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="a0852-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="a0852-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a0852-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0852-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a0852-118">Relationships</span></span>
<span data-ttu-id="a0852-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a0852-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0852-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a0852-120">JSON Representation</span></span>
<span data-ttu-id="a0852-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a0852-121">Here is a JSON representation of the resource.</span></span>
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



