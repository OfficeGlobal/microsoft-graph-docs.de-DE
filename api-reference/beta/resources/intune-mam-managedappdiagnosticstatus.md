---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 665ca55c67f5facb22eaf976e81737fed3dacf76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407361"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="fa12c-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fa12c-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="fa12c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fa12c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa12c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa12c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa12c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa12c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa12c-107">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="fa12c-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="fa12c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa12c-108">Properties</span></span>
|<span data-ttu-id="fa12c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa12c-109">Property</span></span>|<span data-ttu-id="fa12c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fa12c-110">Type</span></span>|<span data-ttu-id="fa12c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa12c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa12c-112">validationName</span><span class="sxs-lookup"><span data-stu-id="fa12c-112">validationName</span></span>|<span data-ttu-id="fa12c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa12c-113">String</span></span>|<span data-ttu-id="fa12c-114">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="fa12c-114">The validation friendly name</span></span>|
|<span data-ttu-id="fa12c-115">state</span><span class="sxs-lookup"><span data-stu-id="fa12c-115">state</span></span>|<span data-ttu-id="fa12c-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa12c-116">String</span></span>|<span data-ttu-id="fa12c-117">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="fa12c-117">The state of the operation</span></span>|
|<span data-ttu-id="fa12c-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="fa12c-118">mitigationInstruction</span></span>|<span data-ttu-id="fa12c-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa12c-119">String</span></span>|<span data-ttu-id="fa12c-120">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="fa12c-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa12c-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fa12c-121">Relationships</span></span>
<span data-ttu-id="fa12c-122">Keine</span><span class="sxs-lookup"><span data-stu-id="fa12c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa12c-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa12c-123">JSON Representation</span></span>
<span data-ttu-id="fa12c-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa12c-124">Here is a JSON representation of the resource.</span></span>
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




