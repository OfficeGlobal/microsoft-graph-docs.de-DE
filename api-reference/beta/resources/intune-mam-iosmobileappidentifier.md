---
title: iosMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine iOS-App.
author: tfitzmac
ms.openlocfilehash: e68bfcca4b0873013c0c9e0fd0295483257ae52c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354173"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="579c5-103">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="579c5-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="579c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="579c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="579c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="579c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="579c5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="579c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="579c5-107">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="579c5-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="579c5-108">Erbt von [MobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="579c5-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="579c5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="579c5-109">Properties</span></span>
|<span data-ttu-id="579c5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="579c5-110">Property</span></span>|<span data-ttu-id="579c5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="579c5-111">Type</span></span>|<span data-ttu-id="579c5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="579c5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="579c5-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="579c5-113">bundleId</span></span>|<span data-ttu-id="579c5-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579c5-114">String</span></span>|<span data-ttu-id="579c5-115">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="579c5-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="579c5-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="579c5-116">Relationships</span></span>
<span data-ttu-id="579c5-117">Keine</span><span class="sxs-lookup"><span data-stu-id="579c5-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="579c5-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="579c5-118">JSON Representation</span></span>
<span data-ttu-id="579c5-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="579c5-119">Here is a JSON representation of the resource.</span></span>
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





