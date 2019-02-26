---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a44800da46d771251a47df676af84ceb778cbbd6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257687"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="713d8-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="713d8-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="713d8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="713d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="713d8-105">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="713d8-105">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="713d8-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="713d8-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="713d8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="713d8-107">Properties</span></span>
|<span data-ttu-id="713d8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="713d8-108">Property</span></span>|<span data-ttu-id="713d8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="713d8-109">Type</span></span>|<span data-ttu-id="713d8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="713d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="713d8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="713d8-111">displayName</span></span>|<span data-ttu-id="713d8-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="713d8-112">String</span></span>|<span data-ttu-id="713d8-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="713d8-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="713d8-114">Seiten</span><span class="sxs-lookup"><span data-stu-id="713d8-114">pages</span></span>|<span data-ttu-id="713d8-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="713d8-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="713d8-116">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="713d8-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="713d8-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="713d8-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="713d8-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="713d8-118">Relationships</span></span>
<span data-ttu-id="713d8-119">Keine</span><span class="sxs-lookup"><span data-stu-id="713d8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="713d8-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="713d8-120">JSON Representation</span></span>
<span data-ttu-id="713d8-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="713d8-121">Here is a JSON representation of the resource.</span></span>
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



