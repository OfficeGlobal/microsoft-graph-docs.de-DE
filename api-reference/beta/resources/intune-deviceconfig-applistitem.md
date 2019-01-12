---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 492828fdef95815704083ec8f496e38a10dc3559
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923334"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="091e0-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="091e0-103">appListItem resource type</span></span>

> <span data-ttu-id="091e0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="091e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="091e0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="091e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="091e0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="091e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="091e0-107">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="091e0-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="091e0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="091e0-108">Properties</span></span>
|<span data-ttu-id="091e0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="091e0-109">Property</span></span>|<span data-ttu-id="091e0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="091e0-110">Type</span></span>|<span data-ttu-id="091e0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="091e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="091e0-112">name</span><span class="sxs-lookup"><span data-stu-id="091e0-112">name</span></span>|<span data-ttu-id="091e0-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="091e0-113">String</span></span>|<span data-ttu-id="091e0-114">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="091e0-114">The application name</span></span>|
|<span data-ttu-id="091e0-115">publisher</span><span class="sxs-lookup"><span data-stu-id="091e0-115">publisher</span></span>|<span data-ttu-id="091e0-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="091e0-116">String</span></span>|<span data-ttu-id="091e0-117">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="091e0-117">The publisher of the application</span></span>|
|<span data-ttu-id="091e0-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="091e0-118">appStoreUrl</span></span>|<span data-ttu-id="091e0-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="091e0-119">String</span></span>|<span data-ttu-id="091e0-120">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="091e0-120">The Store URL of the application</span></span>|
|<span data-ttu-id="091e0-121">appId</span><span class="sxs-lookup"><span data-stu-id="091e0-121">appId</span></span>|<span data-ttu-id="091e0-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="091e0-122">String</span></span>|<span data-ttu-id="091e0-123">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="091e0-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="091e0-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="091e0-124">Relationships</span></span>
<span data-ttu-id="091e0-125">Keine</span><span class="sxs-lookup"><span data-stu-id="091e0-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="091e0-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="091e0-126">JSON Representation</span></span>
<span data-ttu-id="091e0-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="091e0-127">Here is a JSON representation of the resource.</span></span>
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





