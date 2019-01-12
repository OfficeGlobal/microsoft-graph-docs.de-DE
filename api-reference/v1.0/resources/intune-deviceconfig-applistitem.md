---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a70f68d291036a7a01823c1946aac655aee6e71c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954428"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="ff762-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ff762-103">appListItem resource type</span></span>

> <span data-ttu-id="ff762-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff762-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff762-105">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="ff762-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="ff762-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff762-106">Properties</span></span>
|<span data-ttu-id="ff762-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff762-107">Property</span></span>|<span data-ttu-id="ff762-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ff762-108">Type</span></span>|<span data-ttu-id="ff762-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff762-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff762-110">name</span><span class="sxs-lookup"><span data-stu-id="ff762-110">name</span></span>|<span data-ttu-id="ff762-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff762-111">String</span></span>|<span data-ttu-id="ff762-112">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="ff762-112">The application name</span></span>|
|<span data-ttu-id="ff762-113">publisher</span><span class="sxs-lookup"><span data-stu-id="ff762-113">publisher</span></span>|<span data-ttu-id="ff762-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff762-114">String</span></span>|<span data-ttu-id="ff762-115">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="ff762-115">The publisher of the application</span></span>|
|<span data-ttu-id="ff762-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ff762-116">appStoreUrl</span></span>|<span data-ttu-id="ff762-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff762-117">String</span></span>|<span data-ttu-id="ff762-118">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff762-118">The Store URL of the application</span></span>|
|<span data-ttu-id="ff762-119">appId</span><span class="sxs-lookup"><span data-stu-id="ff762-119">appId</span></span>|<span data-ttu-id="ff762-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff762-120">String</span></span>|<span data-ttu-id="ff762-121">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff762-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff762-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff762-122">Relationships</span></span>
<span data-ttu-id="ff762-123">Keine</span><span class="sxs-lookup"><span data-stu-id="ff762-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff762-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff762-124">JSON Representation</span></span>
<span data-ttu-id="ff762-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff762-125">Here is a JSON representation of the resource.</span></span>
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



