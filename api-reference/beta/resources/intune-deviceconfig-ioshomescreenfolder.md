---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 82e94f282e4d338c0422c613a0163a40ce76762e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835854"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="ff0e7-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ff0e7-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="ff0e7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff0e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff0e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff0e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff0e7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff0e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff0e7-107">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="ff0e7-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="ff0e7-108">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="ff0e7-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff0e7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff0e7-109">Properties</span></span>
|<span data-ttu-id="ff0e7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff0e7-110">Property</span></span>|<span data-ttu-id="ff0e7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ff0e7-111">Type</span></span>|<span data-ttu-id="ff0e7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff0e7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0e7-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ff0e7-113">displayName</span></span>|<span data-ttu-id="ff0e7-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0e7-114">String</span></span>|<span data-ttu-id="ff0e7-115">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="ff0e7-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="ff0e7-116">Seiten</span><span class="sxs-lookup"><span data-stu-id="ff0e7-116">pages</span></span>|<span data-ttu-id="ff0e7-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ff0e7-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="ff0e7-118">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="ff0e7-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="ff0e7-119">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ff0e7-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff0e7-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff0e7-120">Relationships</span></span>
<span data-ttu-id="ff0e7-121">Keine</span><span class="sxs-lookup"><span data-stu-id="ff0e7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff0e7-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff0e7-122">JSON Representation</span></span>
<span data-ttu-id="ff0e7-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff0e7-123">Here is a JSON representation of the resource.</span></span>
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





