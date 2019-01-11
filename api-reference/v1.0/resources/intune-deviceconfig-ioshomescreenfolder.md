---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1a4f7f4180bce05d331fcc116826956f4feed70c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844576"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="f001f-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f001f-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="f001f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f001f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f001f-105">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="f001f-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="f001f-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f001f-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f001f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f001f-107">Properties</span></span>
|<span data-ttu-id="f001f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f001f-108">Property</span></span>|<span data-ttu-id="f001f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f001f-109">Type</span></span>|<span data-ttu-id="f001f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f001f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f001f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f001f-111">displayName</span></span>|<span data-ttu-id="f001f-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f001f-112">String</span></span>|<span data-ttu-id="f001f-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="f001f-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="f001f-114">Seiten</span><span class="sxs-lookup"><span data-stu-id="f001f-114">pages</span></span>|<span data-ttu-id="f001f-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f001f-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="f001f-116">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="f001f-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="f001f-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f001f-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f001f-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f001f-118">Relationships</span></span>
<span data-ttu-id="f001f-119">Keine</span><span class="sxs-lookup"><span data-stu-id="f001f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f001f-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f001f-120">JSON Representation</span></span>
<span data-ttu-id="f001f-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f001f-121">Here is a JSON representation of the resource.</span></span>
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



