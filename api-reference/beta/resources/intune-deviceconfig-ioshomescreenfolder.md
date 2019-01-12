---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 97d159b09d8484a88db46ec6d25fa9996127b484
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937950"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="4321f-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4321f-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="4321f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4321f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4321f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4321f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4321f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4321f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4321f-107">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="4321f-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="4321f-108">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4321f-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4321f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4321f-109">Properties</span></span>
|<span data-ttu-id="4321f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4321f-110">Property</span></span>|<span data-ttu-id="4321f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4321f-111">Type</span></span>|<span data-ttu-id="4321f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4321f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4321f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="4321f-113">displayName</span></span>|<span data-ttu-id="4321f-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4321f-114">String</span></span>|<span data-ttu-id="4321f-115">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="4321f-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="4321f-116">Seiten</span><span class="sxs-lookup"><span data-stu-id="4321f-116">pages</span></span>|<span data-ttu-id="4321f-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4321f-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="4321f-118">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="4321f-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="4321f-119">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4321f-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4321f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4321f-120">Relationships</span></span>
<span data-ttu-id="4321f-121">Keine</span><span class="sxs-lookup"><span data-stu-id="4321f-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4321f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4321f-122">JSON Representation</span></span>
<span data-ttu-id="4321f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4321f-123">Here is a JSON representation of the resource.</span></span>
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





