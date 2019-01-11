---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b9d7df95ce8ddb71439763eb02b205772e06300
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820321"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="f54fd-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f54fd-103">appListItem resource type</span></span>

> <span data-ttu-id="f54fd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f54fd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f54fd-105">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="f54fd-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="f54fd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f54fd-106">Properties</span></span>
|<span data-ttu-id="f54fd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f54fd-107">Property</span></span>|<span data-ttu-id="f54fd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f54fd-108">Type</span></span>|<span data-ttu-id="f54fd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f54fd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f54fd-110">name</span><span class="sxs-lookup"><span data-stu-id="f54fd-110">name</span></span>|<span data-ttu-id="f54fd-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f54fd-111">String</span></span>|<span data-ttu-id="f54fd-112">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="f54fd-112">The application name</span></span>|
|<span data-ttu-id="f54fd-113">publisher</span><span class="sxs-lookup"><span data-stu-id="f54fd-113">publisher</span></span>|<span data-ttu-id="f54fd-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f54fd-114">String</span></span>|<span data-ttu-id="f54fd-115">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="f54fd-115">The publisher of the application</span></span>|
|<span data-ttu-id="f54fd-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f54fd-116">appStoreUrl</span></span>|<span data-ttu-id="f54fd-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f54fd-117">String</span></span>|<span data-ttu-id="f54fd-118">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f54fd-118">The Store URL of the application</span></span>|
|<span data-ttu-id="f54fd-119">appId</span><span class="sxs-lookup"><span data-stu-id="f54fd-119">appId</span></span>|<span data-ttu-id="f54fd-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f54fd-120">String</span></span>|<span data-ttu-id="f54fd-121">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f54fd-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f54fd-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f54fd-122">Relationships</span></span>
<span data-ttu-id="f54fd-123">Keine</span><span class="sxs-lookup"><span data-stu-id="f54fd-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f54fd-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f54fd-124">JSON Representation</span></span>
<span data-ttu-id="f54fd-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f54fd-125">Here is a JSON representation of the resource.</span></span>
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



