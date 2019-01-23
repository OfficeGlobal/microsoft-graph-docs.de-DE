---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba8aa9cfe10d17cefdcfe28d25c4d8c2dfa429f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412478"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="eed70-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eed70-103">auditResource resource type</span></span>

> <span data-ttu-id="eed70-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="eed70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eed70-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eed70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eed70-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eed70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eed70-107">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="eed70-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="eed70-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eed70-108">Properties</span></span>
|<span data-ttu-id="eed70-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eed70-109">Property</span></span>|<span data-ttu-id="eed70-110">Typ</span><span class="sxs-lookup"><span data-stu-id="eed70-110">Type</span></span>|<span data-ttu-id="eed70-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eed70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed70-112">displayName</span><span class="sxs-lookup"><span data-stu-id="eed70-112">displayName</span></span>|<span data-ttu-id="eed70-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eed70-113">String</span></span>|<span data-ttu-id="eed70-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="eed70-114">Display name.</span></span>|
|<span data-ttu-id="eed70-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="eed70-115">modifiedProperties</span></span>|<span data-ttu-id="eed70-116">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="eed70-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="eed70-117">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eed70-117">List of modified properties.</span></span>|
|<span data-ttu-id="eed70-118">Typ</span><span class="sxs-lookup"><span data-stu-id="eed70-118">type</span></span>|<span data-ttu-id="eed70-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eed70-119">String</span></span>|<span data-ttu-id="eed70-120">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="eed70-120">Audit resource's type.</span></span>|
|<span data-ttu-id="eed70-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="eed70-121">resourceId</span></span>|<span data-ttu-id="eed70-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eed70-122">String</span></span>|<span data-ttu-id="eed70-123">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="eed70-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eed70-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eed70-124">Relationships</span></span>
<span data-ttu-id="eed70-125">Keine</span><span class="sxs-lookup"><span data-stu-id="eed70-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eed70-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eed70-126">JSON Representation</span></span>
<span data-ttu-id="eed70-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eed70-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```




