---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8afb80b9130356671d80e5ec52f96bf74ed53d7e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153739"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="985c7-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="985c7-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="985c7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="985c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="985c7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="985c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="985c7-106">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="985c7-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="985c7-107">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="985c7-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="985c7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="985c7-108">Properties</span></span>
|<span data-ttu-id="985c7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="985c7-109">Property</span></span>|<span data-ttu-id="985c7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="985c7-110">Type</span></span>|<span data-ttu-id="985c7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="985c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="985c7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="985c7-112">displayName</span></span>|<span data-ttu-id="985c7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="985c7-113">String</span></span>|<span data-ttu-id="985c7-114">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="985c7-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="985c7-115">Seiten</span><span class="sxs-lookup"><span data-stu-id="985c7-115">pages</span></span>|<span data-ttu-id="985c7-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="985c7-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="985c7-117">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="985c7-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="985c7-118">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="985c7-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="985c7-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="985c7-119">Relationships</span></span>
<span data-ttu-id="985c7-120">Keine</span><span class="sxs-lookup"><span data-stu-id="985c7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="985c7-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="985c7-121">JSON Representation</span></span>
<span data-ttu-id="985c7-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="985c7-122">Here is a JSON representation of the resource.</span></span>
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




