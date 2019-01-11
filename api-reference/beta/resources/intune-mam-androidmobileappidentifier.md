---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 59c947192cf00e1f6852c51513692123595c975b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837591"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="121a5-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="121a5-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="121a5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="121a5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="121a5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="121a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="121a5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="121a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="121a5-107">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="121a5-107">The identifier for an Android app.</span></span>

<span data-ttu-id="121a5-108">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="121a5-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="121a5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="121a5-109">Properties</span></span>
|<span data-ttu-id="121a5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="121a5-110">Property</span></span>|<span data-ttu-id="121a5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="121a5-111">Type</span></span>|<span data-ttu-id="121a5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="121a5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="121a5-113">packageId</span><span class="sxs-lookup"><span data-stu-id="121a5-113">packageId</span></span>|<span data-ttu-id="121a5-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="121a5-114">String</span></span>|<span data-ttu-id="121a5-115">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="121a5-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="121a5-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="121a5-116">Relationships</span></span>
<span data-ttu-id="121a5-117">Keine</span><span class="sxs-lookup"><span data-stu-id="121a5-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="121a5-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="121a5-118">JSON Representation</span></span>
<span data-ttu-id="121a5-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="121a5-119">Here is a JSON representation of the resource.</span></span>
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





