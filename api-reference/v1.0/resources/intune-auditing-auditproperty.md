---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260613"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="08803-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08803-103">auditProperty resource type</span></span>

> <span data-ttu-id="08803-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="08803-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08803-105">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="08803-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="08803-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08803-106">Properties</span></span>
|<span data-ttu-id="08803-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08803-107">Property</span></span>|<span data-ttu-id="08803-108">Typ</span><span class="sxs-lookup"><span data-stu-id="08803-108">Type</span></span>|<span data-ttu-id="08803-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08803-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08803-110">displayName</span><span class="sxs-lookup"><span data-stu-id="08803-110">displayName</span></span>|<span data-ttu-id="08803-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08803-111">String</span></span>|<span data-ttu-id="08803-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="08803-112">Display name.</span></span>|
|<span data-ttu-id="08803-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="08803-113">oldValue</span></span>|<span data-ttu-id="08803-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08803-114">String</span></span>|<span data-ttu-id="08803-115">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="08803-115">Old value.</span></span>|
|<span data-ttu-id="08803-116">newValue</span><span class="sxs-lookup"><span data-stu-id="08803-116">newValue</span></span>|<span data-ttu-id="08803-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08803-117">String</span></span>|<span data-ttu-id="08803-118">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="08803-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08803-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08803-119">Relationships</span></span>
<span data-ttu-id="08803-120">Keine</span><span class="sxs-lookup"><span data-stu-id="08803-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08803-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08803-121">JSON Representation</span></span>
<span data-ttu-id="08803-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08803-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



