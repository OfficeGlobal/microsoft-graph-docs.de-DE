---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
ms.openlocfilehash: 16f142c40083b9410f84e128951680ced269ea12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018438"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="c945a-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c945a-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c945a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c945a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c945a-105">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="c945a-105">The identifier for an Android app.</span></span>

<span data-ttu-id="c945a-106">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c945a-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c945a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c945a-107">Properties</span></span>
|<span data-ttu-id="c945a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c945a-108">Property</span></span>|<span data-ttu-id="c945a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c945a-109">Type</span></span>|<span data-ttu-id="c945a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c945a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c945a-111">packageId</span><span class="sxs-lookup"><span data-stu-id="c945a-111">packageId</span></span>|<span data-ttu-id="c945a-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c945a-112">String</span></span>|<span data-ttu-id="c945a-113">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="c945a-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c945a-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c945a-114">Relationships</span></span>
<span data-ttu-id="c945a-115">Keine</span><span class="sxs-lookup"><span data-stu-id="c945a-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c945a-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c945a-116">JSON Representation</span></span>
<span data-ttu-id="c945a-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c945a-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



