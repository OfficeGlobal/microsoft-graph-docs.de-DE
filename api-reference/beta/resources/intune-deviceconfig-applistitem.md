---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
ms.openlocfilehash: 16d191bb53f7546598b7869e8bc28be07cc4f604
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062559"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="f73f8-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f73f8-103">appListItem resource type</span></span>

> <span data-ttu-id="f73f8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f73f8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f73f8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f73f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f73f8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f73f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f73f8-107">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="f73f8-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="f73f8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f73f8-108">Properties</span></span>
|<span data-ttu-id="f73f8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f73f8-109">Property</span></span>|<span data-ttu-id="f73f8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f73f8-110">Type</span></span>|<span data-ttu-id="f73f8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f73f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f73f8-112">name</span><span class="sxs-lookup"><span data-stu-id="f73f8-112">name</span></span>|<span data-ttu-id="f73f8-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f73f8-113">String</span></span>|<span data-ttu-id="f73f8-114">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="f73f8-114">The application name</span></span>|
|<span data-ttu-id="f73f8-115">publisher</span><span class="sxs-lookup"><span data-stu-id="f73f8-115">publisher</span></span>|<span data-ttu-id="f73f8-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f73f8-116">String</span></span>|<span data-ttu-id="f73f8-117">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="f73f8-117">The publisher of the application</span></span>|
|<span data-ttu-id="f73f8-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f73f8-118">appStoreUrl</span></span>|<span data-ttu-id="f73f8-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f73f8-119">String</span></span>|<span data-ttu-id="f73f8-120">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f73f8-120">The Store URL of the application</span></span>|
|<span data-ttu-id="f73f8-121">appId</span><span class="sxs-lookup"><span data-stu-id="f73f8-121">appId</span></span>|<span data-ttu-id="f73f8-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f73f8-122">String</span></span>|<span data-ttu-id="f73f8-123">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f73f8-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f73f8-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f73f8-124">Relationships</span></span>
<span data-ttu-id="f73f8-125">Keine</span><span class="sxs-lookup"><span data-stu-id="f73f8-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f73f8-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f73f8-126">JSON Representation</span></span>
<span data-ttu-id="f73f8-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f73f8-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





