---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2cdaf6c263b041547056f8f6bd82e21ca880ebaa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949174"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="cdd61-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cdd61-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="cdd61-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cdd61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdd61-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cdd61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdd61-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cdd61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdd61-107">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="cdd61-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="cdd61-108">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdd61-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cdd61-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cdd61-109">Properties</span></span>
|<span data-ttu-id="cdd61-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cdd61-110">Property</span></span>|<span data-ttu-id="cdd61-111">Typ</span><span class="sxs-lookup"><span data-stu-id="cdd61-111">Type</span></span>|<span data-ttu-id="cdd61-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cdd61-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdd61-113">displayName</span><span class="sxs-lookup"><span data-stu-id="cdd61-113">displayName</span></span>|<span data-ttu-id="cdd61-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cdd61-114">String</span></span>|<span data-ttu-id="cdd61-115">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="cdd61-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="cdd61-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="cdd61-116">bundleID</span></span>|<span data-ttu-id="cdd61-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cdd61-117">String</span></span>|<span data-ttu-id="cdd61-118">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="cdd61-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdd61-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cdd61-119">Relationships</span></span>
<span data-ttu-id="cdd61-120">Keine</span><span class="sxs-lookup"><span data-stu-id="cdd61-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cdd61-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cdd61-121">JSON Representation</span></span>
<span data-ttu-id="cdd61-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cdd61-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```





