---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e2a6b2309e831a872c4cde04a951819cac292ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262083"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="36a04-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="36a04-103">auditResource resource type</span></span>

> <span data-ttu-id="36a04-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="36a04-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a04-105">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="36a04-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="36a04-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36a04-106">Properties</span></span>
|<span data-ttu-id="36a04-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36a04-107">Property</span></span>|<span data-ttu-id="36a04-108">Typ</span><span class="sxs-lookup"><span data-stu-id="36a04-108">Type</span></span>|<span data-ttu-id="36a04-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36a04-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36a04-110">displayName</span><span class="sxs-lookup"><span data-stu-id="36a04-110">displayName</span></span>|<span data-ttu-id="36a04-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36a04-111">String</span></span>|<span data-ttu-id="36a04-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="36a04-112">Display name.</span></span>|
|<span data-ttu-id="36a04-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="36a04-113">modifiedProperties</span></span>|<span data-ttu-id="36a04-114">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="36a04-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="36a04-115">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36a04-115">List of modified properties.</span></span>|
|<span data-ttu-id="36a04-116">Typ</span><span class="sxs-lookup"><span data-stu-id="36a04-116">type</span></span>|<span data-ttu-id="36a04-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36a04-117">String</span></span>|<span data-ttu-id="36a04-118">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="36a04-118">Audit resource's type.</span></span>|
|<span data-ttu-id="36a04-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="36a04-119">resourceId</span></span>|<span data-ttu-id="36a04-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36a04-120">String</span></span>|<span data-ttu-id="36a04-121">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="36a04-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36a04-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="36a04-122">Relationships</span></span>
<span data-ttu-id="36a04-123">Keine</span><span class="sxs-lookup"><span data-stu-id="36a04-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36a04-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36a04-124">JSON Representation</span></span>
<span data-ttu-id="36a04-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="36a04-125">Here is a JSON representation of the resource.</span></span>
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



