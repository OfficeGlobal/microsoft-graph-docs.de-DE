---
title: iosHomeScreenFolderPage-Ressourcentyp
description: Ein Ordner mit Apps auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2808adaa99787efb96c7b21deaddf4c855e799d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165527"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="5de30-103">iosHomeScreenFolderPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5de30-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="5de30-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5de30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5de30-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5de30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5de30-106">Ein Ordner mit Apps auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="5de30-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="5de30-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5de30-107">Properties</span></span>
|<span data-ttu-id="5de30-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5de30-108">Property</span></span>|<span data-ttu-id="5de30-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5de30-109">Type</span></span>|<span data-ttu-id="5de30-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5de30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de30-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5de30-111">displayName</span></span>|<span data-ttu-id="5de30-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5de30-112">String</span></span>|<span data-ttu-id="5de30-113">Name des Ordnerseite</span><span class="sxs-lookup"><span data-stu-id="5de30-113">Name of the folder page</span></span>|
|<span data-ttu-id="5de30-114">Apps</span><span class="sxs-lookup"><span data-stu-id="5de30-114">apps</span></span>|<span data-ttu-id="5de30-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5de30-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="5de30-116">Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="5de30-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="5de30-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5de30-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5de30-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5de30-118">Relationships</span></span>
<span data-ttu-id="5de30-119">Keine</span><span class="sxs-lookup"><span data-stu-id="5de30-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5de30-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5de30-120">JSON Representation</span></span>
<span data-ttu-id="5de30-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5de30-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```




