---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f471a71c10a225f2bb5af77399932402f154538d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872121"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="abddd-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="abddd-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="abddd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="abddd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abddd-105">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="abddd-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="abddd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="abddd-106">Properties</span></span>
|<span data-ttu-id="abddd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abddd-107">Property</span></span>|<span data-ttu-id="abddd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="abddd-108">Type</span></span>|<span data-ttu-id="abddd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abddd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abddd-110">validationName</span><span class="sxs-lookup"><span data-stu-id="abddd-110">validationName</span></span>|<span data-ttu-id="abddd-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abddd-111">String</span></span>|<span data-ttu-id="abddd-112">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="abddd-112">The validation friendly name</span></span>|
|<span data-ttu-id="abddd-113">state</span><span class="sxs-lookup"><span data-stu-id="abddd-113">state</span></span>|<span data-ttu-id="abddd-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abddd-114">String</span></span>|<span data-ttu-id="abddd-115">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="abddd-115">The state of the operation</span></span>|
|<span data-ttu-id="abddd-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="abddd-116">mitigationInstruction</span></span>|<span data-ttu-id="abddd-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abddd-117">String</span></span>|<span data-ttu-id="abddd-118">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="abddd-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="abddd-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="abddd-119">Relationships</span></span>
<span data-ttu-id="abddd-120">Keine</span><span class="sxs-lookup"><span data-stu-id="abddd-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abddd-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="abddd-121">JSON Representation</span></span>
<span data-ttu-id="abddd-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="abddd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



