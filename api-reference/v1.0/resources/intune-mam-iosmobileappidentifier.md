---
title: iosMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine iOS-App.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e9305963654356c56bff31f6ffb9f97129f4980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922788"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="5040c-103">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5040c-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5040c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5040c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5040c-105">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="5040c-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="5040c-106">Erbt von [MobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5040c-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5040c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5040c-107">Properties</span></span>
|<span data-ttu-id="5040c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5040c-108">Property</span></span>|<span data-ttu-id="5040c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5040c-109">Type</span></span>|<span data-ttu-id="5040c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5040c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5040c-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="5040c-111">bundleId</span></span>|<span data-ttu-id="5040c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5040c-112">String</span></span>|<span data-ttu-id="5040c-113">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="5040c-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5040c-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5040c-114">Relationships</span></span>
<span data-ttu-id="5040c-115">Keine</span><span class="sxs-lookup"><span data-stu-id="5040c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5040c-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5040c-116">JSON Representation</span></span>
<span data-ttu-id="5040c-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5040c-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



