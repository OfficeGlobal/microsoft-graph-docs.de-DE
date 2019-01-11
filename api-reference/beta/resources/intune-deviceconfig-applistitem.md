---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7aab42e778ffb78db2fc85cec786d2cc25437b74
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876713"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="4231e-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4231e-103">appListItem resource type</span></span>

> <span data-ttu-id="4231e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4231e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4231e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4231e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4231e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4231e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4231e-107">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="4231e-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="4231e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4231e-108">Properties</span></span>
|<span data-ttu-id="4231e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4231e-109">Property</span></span>|<span data-ttu-id="4231e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4231e-110">Type</span></span>|<span data-ttu-id="4231e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4231e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4231e-112">name</span><span class="sxs-lookup"><span data-stu-id="4231e-112">name</span></span>|<span data-ttu-id="4231e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4231e-113">String</span></span>|<span data-ttu-id="4231e-114">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="4231e-114">The application name</span></span>|
|<span data-ttu-id="4231e-115">publisher</span><span class="sxs-lookup"><span data-stu-id="4231e-115">publisher</span></span>|<span data-ttu-id="4231e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4231e-116">String</span></span>|<span data-ttu-id="4231e-117">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="4231e-117">The publisher of the application</span></span>|
|<span data-ttu-id="4231e-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4231e-118">appStoreUrl</span></span>|<span data-ttu-id="4231e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4231e-119">String</span></span>|<span data-ttu-id="4231e-120">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="4231e-120">The Store URL of the application</span></span>|
|<span data-ttu-id="4231e-121">appId</span><span class="sxs-lookup"><span data-stu-id="4231e-121">appId</span></span>|<span data-ttu-id="4231e-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4231e-122">String</span></span>|<span data-ttu-id="4231e-123">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="4231e-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="4231e-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4231e-124">Relationships</span></span>
<span data-ttu-id="4231e-125">Keine</span><span class="sxs-lookup"><span data-stu-id="4231e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4231e-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4231e-126">JSON Representation</span></span>
<span data-ttu-id="4231e-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4231e-127">Here is a JSON representation of the resource.</span></span>
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





