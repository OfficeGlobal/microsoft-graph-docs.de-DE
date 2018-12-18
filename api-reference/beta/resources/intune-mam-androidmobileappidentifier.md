---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
author: tfitzmac
ms.openlocfilehash: c8f590deb33faf1782e3e2ad38f0b65ab4f58eed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306881"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="8afd8-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8afd8-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="8afd8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8afd8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8afd8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8afd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8afd8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8afd8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8afd8-107">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="8afd8-107">The identifier for an Android app.</span></span>

<span data-ttu-id="8afd8-108">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="8afd8-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8afd8-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8afd8-109">Properties</span></span>
|<span data-ttu-id="8afd8-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8afd8-110">Property</span></span>|<span data-ttu-id="8afd8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8afd8-111">Type</span></span>|<span data-ttu-id="8afd8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8afd8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8afd8-113">packageId</span><span class="sxs-lookup"><span data-stu-id="8afd8-113">packageId</span></span>|<span data-ttu-id="8afd8-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8afd8-114">String</span></span>|<span data-ttu-id="8afd8-115">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="8afd8-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8afd8-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8afd8-116">Relationships</span></span>
<span data-ttu-id="8afd8-117">Keine</span><span class="sxs-lookup"><span data-stu-id="8afd8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8afd8-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8afd8-118">JSON Representation</span></span>
<span data-ttu-id="8afd8-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8afd8-119">Here is a JSON representation of the resource.</span></span>
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





