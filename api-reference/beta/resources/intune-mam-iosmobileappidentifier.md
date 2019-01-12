---
title: iosMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine iOS-App.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 134f6e27b6fb113516fd119211e245fd77b2ae75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919526"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="ebb55-103">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ebb55-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ebb55-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ebb55-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebb55-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebb55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebb55-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ebb55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebb55-107">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="ebb55-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="ebb55-108">Erbt von [MobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ebb55-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebb55-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ebb55-109">Properties</span></span>
|<span data-ttu-id="ebb55-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebb55-110">Property</span></span>|<span data-ttu-id="ebb55-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ebb55-111">Type</span></span>|<span data-ttu-id="ebb55-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebb55-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb55-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="ebb55-113">bundleId</span></span>|<span data-ttu-id="ebb55-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebb55-114">String</span></span>|<span data-ttu-id="ebb55-115">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="ebb55-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebb55-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ebb55-116">Relationships</span></span>
<span data-ttu-id="ebb55-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ebb55-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebb55-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ebb55-118">JSON Representation</span></span>
<span data-ttu-id="ebb55-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ebb55-119">Here is a JSON representation of the resource.</span></span>
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





