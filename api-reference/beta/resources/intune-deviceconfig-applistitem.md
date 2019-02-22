---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7e005681917f0edffe00b33947d2bd2bd5b2ff5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172247"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="7ffd3-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7ffd3-103">appListItem resource type</span></span>

> <span data-ttu-id="7ffd3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ffd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ffd3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7ffd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ffd3-106">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="7ffd3-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="7ffd3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7ffd3-107">Properties</span></span>
|<span data-ttu-id="7ffd3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ffd3-108">Property</span></span>|<span data-ttu-id="7ffd3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7ffd3-109">Type</span></span>|<span data-ttu-id="7ffd3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ffd3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ffd3-111">name</span><span class="sxs-lookup"><span data-stu-id="7ffd3-111">name</span></span>|<span data-ttu-id="7ffd3-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ffd3-112">String</span></span>|<span data-ttu-id="7ffd3-113">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="7ffd3-113">The application name</span></span>|
|<span data-ttu-id="7ffd3-114">publisher</span><span class="sxs-lookup"><span data-stu-id="7ffd3-114">publisher</span></span>|<span data-ttu-id="7ffd3-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ffd3-115">String</span></span>|<span data-ttu-id="7ffd3-116">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="7ffd3-116">The publisher of the application</span></span>|
|<span data-ttu-id="7ffd3-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7ffd3-117">appStoreUrl</span></span>|<span data-ttu-id="7ffd3-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ffd3-118">String</span></span>|<span data-ttu-id="7ffd3-119">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ffd3-119">The Store URL of the application</span></span>|
|<span data-ttu-id="7ffd3-120">appId</span><span class="sxs-lookup"><span data-stu-id="7ffd3-120">appId</span></span>|<span data-ttu-id="7ffd3-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ffd3-121">String</span></span>|<span data-ttu-id="7ffd3-122">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ffd3-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ffd3-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7ffd3-123">Relationships</span></span>
<span data-ttu-id="7ffd3-124">Keine</span><span class="sxs-lookup"><span data-stu-id="7ffd3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ffd3-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7ffd3-125">JSON Representation</span></span>
<span data-ttu-id="7ffd3-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7ffd3-126">Here is a JSON representation of the resource.</span></span>
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




