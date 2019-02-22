---
title: iosMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine iOS-App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b62a6d9ca0a864f703ddb41eee4f147098e740a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154103"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="23b69-103">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23b69-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="23b69-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23b69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23b69-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="23b69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23b69-106">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="23b69-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="23b69-107">Erbt von [MobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="23b69-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23b69-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23b69-108">Properties</span></span>
|<span data-ttu-id="23b69-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23b69-109">Property</span></span>|<span data-ttu-id="23b69-110">Typ</span><span class="sxs-lookup"><span data-stu-id="23b69-110">Type</span></span>|<span data-ttu-id="23b69-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23b69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23b69-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="23b69-112">bundleId</span></span>|<span data-ttu-id="23b69-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23b69-113">String</span></span>|<span data-ttu-id="23b69-114">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="23b69-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23b69-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23b69-115">Relationships</span></span>
<span data-ttu-id="23b69-116">Keine</span><span class="sxs-lookup"><span data-stu-id="23b69-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23b69-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23b69-117">JSON Representation</span></span>
<span data-ttu-id="23b69-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23b69-118">Here is a JSON representation of the resource.</span></span>
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




