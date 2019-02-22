---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf91e1a86955612aa590bee68057e1a7adb2d823
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169006"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="f1977-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f1977-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="f1977-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1977-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1977-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f1977-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1977-106">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="f1977-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="f1977-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1977-107">Properties</span></span>
|<span data-ttu-id="f1977-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1977-108">Property</span></span>|<span data-ttu-id="f1977-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f1977-109">Type</span></span>|<span data-ttu-id="f1977-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1977-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1977-111">validationName</span><span class="sxs-lookup"><span data-stu-id="f1977-111">validationName</span></span>|<span data-ttu-id="f1977-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1977-112">String</span></span>|<span data-ttu-id="f1977-113">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="f1977-113">The validation friendly name</span></span>|
|<span data-ttu-id="f1977-114">state</span><span class="sxs-lookup"><span data-stu-id="f1977-114">state</span></span>|<span data-ttu-id="f1977-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1977-115">String</span></span>|<span data-ttu-id="f1977-116">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="f1977-116">The state of the operation</span></span>|
|<span data-ttu-id="f1977-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="f1977-117">mitigationInstruction</span></span>|<span data-ttu-id="f1977-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1977-118">String</span></span>|<span data-ttu-id="f1977-119">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="f1977-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1977-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f1977-120">Relationships</span></span>
<span data-ttu-id="f1977-121">Keine</span><span class="sxs-lookup"><span data-stu-id="f1977-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1977-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1977-122">JSON Representation</span></span>
<span data-ttu-id="f1977-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1977-123">Here is a JSON representation of the resource.</span></span>
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




