---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253078"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="ffd31-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ffd31-103">appListItem resource type</span></span>

> <span data-ttu-id="ffd31-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ffd31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffd31-105">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="ffd31-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="ffd31-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ffd31-106">Properties</span></span>
|<span data-ttu-id="ffd31-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ffd31-107">Property</span></span>|<span data-ttu-id="ffd31-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ffd31-108">Type</span></span>|<span data-ttu-id="ffd31-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffd31-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd31-110">name</span><span class="sxs-lookup"><span data-stu-id="ffd31-110">name</span></span>|<span data-ttu-id="ffd31-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffd31-111">String</span></span>|<span data-ttu-id="ffd31-112">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="ffd31-112">The application name</span></span>|
|<span data-ttu-id="ffd31-113">publisher</span><span class="sxs-lookup"><span data-stu-id="ffd31-113">publisher</span></span>|<span data-ttu-id="ffd31-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffd31-114">String</span></span>|<span data-ttu-id="ffd31-115">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="ffd31-115">The publisher of the application</span></span>|
|<span data-ttu-id="ffd31-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ffd31-116">appStoreUrl</span></span>|<span data-ttu-id="ffd31-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffd31-117">String</span></span>|<span data-ttu-id="ffd31-118">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffd31-118">The Store URL of the application</span></span>|
|<span data-ttu-id="ffd31-119">appId</span><span class="sxs-lookup"><span data-stu-id="ffd31-119">appId</span></span>|<span data-ttu-id="ffd31-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffd31-120">String</span></span>|<span data-ttu-id="ffd31-121">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffd31-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffd31-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ffd31-122">Relationships</span></span>
<span data-ttu-id="ffd31-123">Keine</span><span class="sxs-lookup"><span data-stu-id="ffd31-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffd31-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ffd31-124">JSON Representation</span></span>
<span data-ttu-id="ffd31-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ffd31-125">Here is a JSON representation of the resource.</span></span>
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



