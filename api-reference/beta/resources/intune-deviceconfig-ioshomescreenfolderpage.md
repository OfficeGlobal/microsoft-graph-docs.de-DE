---
title: iosHomeScreenFolderPage-Ressourcentyp
description: Ein Ordner mit Apps auf der Startseite
author: tfitzmac
ms.openlocfilehash: fc5f1899a9eadf88a1815558ed9c1dc9eff51114
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340635"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="6d152-103">iosHomeScreenFolderPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6d152-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="6d152-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6d152-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d152-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d152-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d152-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d152-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d152-107">Ein Ordner mit Apps auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="6d152-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="6d152-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d152-108">Properties</span></span>
|<span data-ttu-id="6d152-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d152-109">Property</span></span>|<span data-ttu-id="6d152-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6d152-110">Type</span></span>|<span data-ttu-id="6d152-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d152-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d152-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6d152-112">displayName</span></span>|<span data-ttu-id="6d152-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d152-113">String</span></span>|<span data-ttu-id="6d152-114">Name des Ordnerseite</span><span class="sxs-lookup"><span data-stu-id="6d152-114">Name of the folder page</span></span>|
|<span data-ttu-id="6d152-115">Apps</span><span class="sxs-lookup"><span data-stu-id="6d152-115">apps</span></span>|<span data-ttu-id="6d152-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d152-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="6d152-117">Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6d152-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="6d152-118">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6d152-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d152-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6d152-119">Relationships</span></span>
<span data-ttu-id="6d152-120">Keine</span><span class="sxs-lookup"><span data-stu-id="6d152-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d152-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d152-121">JSON Representation</span></span>
<span data-ttu-id="6d152-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d152-122">Here is a JSON representation of the resource.</span></span>
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





