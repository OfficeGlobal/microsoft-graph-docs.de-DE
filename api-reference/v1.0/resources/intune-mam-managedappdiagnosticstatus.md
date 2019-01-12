---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a5204a4704eefc2d4e7c8e0d5b3b709e1750667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937481"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="b89dd-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b89dd-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="b89dd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b89dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b89dd-105">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="b89dd-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="b89dd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b89dd-106">Properties</span></span>
|<span data-ttu-id="b89dd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b89dd-107">Property</span></span>|<span data-ttu-id="b89dd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b89dd-108">Type</span></span>|<span data-ttu-id="b89dd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b89dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b89dd-110">validationName</span><span class="sxs-lookup"><span data-stu-id="b89dd-110">validationName</span></span>|<span data-ttu-id="b89dd-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b89dd-111">String</span></span>|<span data-ttu-id="b89dd-112">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="b89dd-112">The validation friendly name</span></span>|
|<span data-ttu-id="b89dd-113">state</span><span class="sxs-lookup"><span data-stu-id="b89dd-113">state</span></span>|<span data-ttu-id="b89dd-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b89dd-114">String</span></span>|<span data-ttu-id="b89dd-115">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="b89dd-115">The state of the operation</span></span>|
|<span data-ttu-id="b89dd-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="b89dd-116">mitigationInstruction</span></span>|<span data-ttu-id="b89dd-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b89dd-117">String</span></span>|<span data-ttu-id="b89dd-118">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="b89dd-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="b89dd-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b89dd-119">Relationships</span></span>
<span data-ttu-id="b89dd-120">Keine</span><span class="sxs-lookup"><span data-stu-id="b89dd-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b89dd-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b89dd-121">JSON Representation</span></span>
<span data-ttu-id="b89dd-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b89dd-122">Here is a JSON representation of the resource.</span></span>
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



