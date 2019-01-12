---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dd47562660f2941fbf722f92976817f310ff304f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930418"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="68130-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="68130-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="68130-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="68130-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68130-105">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="68130-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="68130-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="68130-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68130-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68130-107">Properties</span></span>
|<span data-ttu-id="68130-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68130-108">Property</span></span>|<span data-ttu-id="68130-109">Typ</span><span class="sxs-lookup"><span data-stu-id="68130-109">Type</span></span>|<span data-ttu-id="68130-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68130-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68130-111">displayName</span><span class="sxs-lookup"><span data-stu-id="68130-111">displayName</span></span>|<span data-ttu-id="68130-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68130-112">String</span></span>|<span data-ttu-id="68130-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="68130-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="68130-114">Seiten</span><span class="sxs-lookup"><span data-stu-id="68130-114">pages</span></span>|<span data-ttu-id="68130-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="68130-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="68130-116">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="68130-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="68130-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="68130-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68130-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68130-118">Relationships</span></span>
<span data-ttu-id="68130-119">Keine</span><span class="sxs-lookup"><span data-stu-id="68130-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68130-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68130-120">JSON Representation</span></span>
<span data-ttu-id="68130-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68130-121">Here is a JSON representation of the resource.</span></span>
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



