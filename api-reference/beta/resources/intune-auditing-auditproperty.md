---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3425c59ae4f30b30b04bd22f74cb1b27ad99191f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416643"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="f7845-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f7845-103">auditProperty resource type</span></span>

> <span data-ttu-id="f7845-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f7845-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7845-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7845-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7845-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7845-107">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="f7845-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="f7845-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7845-108">Properties</span></span>
|<span data-ttu-id="f7845-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7845-109">Property</span></span>|<span data-ttu-id="f7845-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f7845-110">Type</span></span>|<span data-ttu-id="f7845-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7845-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7845-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f7845-112">displayName</span></span>|<span data-ttu-id="f7845-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7845-113">String</span></span>|<span data-ttu-id="f7845-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="f7845-114">Display name.</span></span>|
|<span data-ttu-id="f7845-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="f7845-115">oldValue</span></span>|<span data-ttu-id="f7845-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7845-116">String</span></span>|<span data-ttu-id="f7845-117">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="f7845-117">Old value.</span></span>|
|<span data-ttu-id="f7845-118">newValue</span><span class="sxs-lookup"><span data-stu-id="f7845-118">newValue</span></span>|<span data-ttu-id="f7845-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7845-119">String</span></span>|<span data-ttu-id="f7845-120">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="f7845-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7845-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f7845-121">Relationships</span></span>
<span data-ttu-id="f7845-122">Keine</span><span class="sxs-lookup"><span data-stu-id="f7845-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7845-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7845-123">JSON Representation</span></span>
<span data-ttu-id="f7845-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7845-124">Here is a JSON representation of the resource.</span></span>
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




