---
title: iosHomeScreenFolderPage-Ressourcentyp
description: Ein Ordner mit Apps auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0417e7109d95c87083034fa9f7522c0f81dbfb99
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965852"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="8f419-103">iosHomeScreenFolderPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f419-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="8f419-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8f419-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f419-105">Ein Ordner mit Apps auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="8f419-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="8f419-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f419-106">Properties</span></span>
|<span data-ttu-id="8f419-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f419-107">Property</span></span>|<span data-ttu-id="8f419-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8f419-108">Type</span></span>|<span data-ttu-id="8f419-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f419-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f419-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8f419-110">displayName</span></span>|<span data-ttu-id="8f419-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f419-111">String</span></span>|<span data-ttu-id="8f419-112">Name des Ordnerseite</span><span class="sxs-lookup"><span data-stu-id="8f419-112">Name of the folder page</span></span>|
|<span data-ttu-id="8f419-113">Apps</span><span class="sxs-lookup"><span data-stu-id="8f419-113">apps</span></span>|<span data-ttu-id="8f419-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f419-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="8f419-115">Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8f419-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="8f419-116">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8f419-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f419-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f419-117">Relationships</span></span>
<span data-ttu-id="8f419-118">Keine</span><span class="sxs-lookup"><span data-stu-id="8f419-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f419-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f419-119">JSON Representation</span></span>
<span data-ttu-id="8f419-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f419-120">Here is a JSON representation of the resource.</span></span>
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



