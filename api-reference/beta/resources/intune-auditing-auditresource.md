---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f22ace5fa4c381584325ffc8434f0e09faaaaeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156014"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="b8e6c-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8e6c-103">auditResource resource type</span></span>

> <span data-ttu-id="b8e6c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8e6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8e6c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8e6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e6c-106">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="b8e6c-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="b8e6c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8e6c-107">Properties</span></span>
|<span data-ttu-id="b8e6c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8e6c-108">Property</span></span>|<span data-ttu-id="b8e6c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b8e6c-109">Type</span></span>|<span data-ttu-id="b8e6c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8e6c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e6c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b8e6c-111">displayName</span></span>|<span data-ttu-id="b8e6c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8e6c-112">String</span></span>|<span data-ttu-id="b8e6c-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b8e6c-113">Display name.</span></span>|
|<span data-ttu-id="b8e6c-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b8e6c-114">modifiedProperties</span></span>|<span data-ttu-id="b8e6c-115">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b8e6c-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="b8e6c-116">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8e6c-116">List of modified properties.</span></span>|
|<span data-ttu-id="b8e6c-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b8e6c-117">type</span></span>|<span data-ttu-id="b8e6c-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8e6c-118">String</span></span>|<span data-ttu-id="b8e6c-119">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="b8e6c-119">Audit resource's type.</span></span>|
|<span data-ttu-id="b8e6c-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="b8e6c-120">resourceId</span></span>|<span data-ttu-id="b8e6c-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8e6c-121">String</span></span>|<span data-ttu-id="b8e6c-122">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="b8e6c-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e6c-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8e6c-123">Relationships</span></span>
<span data-ttu-id="b8e6c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="b8e6c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8e6c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8e6c-125">JSON Representation</span></span>
<span data-ttu-id="b8e6c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8e6c-126">Here is a JSON representation of the resource.</span></span>
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




