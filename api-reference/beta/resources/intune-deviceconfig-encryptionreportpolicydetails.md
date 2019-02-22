---
title: encryptionReportPolicyDetails-Ressourcentyp
description: Richtlinien Details für den Verschlüsselungs Bericht
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177917"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="dfb63-103">encryptionReportPolicyDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dfb63-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="dfb63-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dfb63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfb63-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dfb63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfb63-106">Richtlinien Details für den Verschlüsselungs Bericht</span><span class="sxs-lookup"><span data-stu-id="dfb63-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="dfb63-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dfb63-107">Properties</span></span>
|<span data-ttu-id="dfb63-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dfb63-108">Property</span></span>|<span data-ttu-id="dfb63-109">Typ</span><span class="sxs-lookup"><span data-stu-id="dfb63-109">Type</span></span>|<span data-ttu-id="dfb63-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfb63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb63-111">Richtlinien-Nr</span><span class="sxs-lookup"><span data-stu-id="dfb63-111">policyId</span></span>|<span data-ttu-id="dfb63-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfb63-112">String</span></span>|<span data-ttu-id="dfb63-113">Richtlinien-ID für Verschlüsselungs Bericht</span><span class="sxs-lookup"><span data-stu-id="dfb63-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="dfb63-114">policyName</span><span class="sxs-lookup"><span data-stu-id="dfb63-114">policyName</span></span>|<span data-ttu-id="dfb63-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfb63-115">String</span></span>|<span data-ttu-id="dfb63-116">Richtlinien Name für Verschlüsselungs Bericht</span><span class="sxs-lookup"><span data-stu-id="dfb63-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb63-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dfb63-117">Relationships</span></span>
<span data-ttu-id="dfb63-118">Keine</span><span class="sxs-lookup"><span data-stu-id="dfb63-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb63-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dfb63-119">JSON Representation</span></span>
<span data-ttu-id="dfb63-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dfb63-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




