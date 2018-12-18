---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
ms.openlocfilehash: 7f0cd0d5b11c4d902f51dd422add2373e8e8df9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340684"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="3c037-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c037-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="3c037-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3c037-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c037-105">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="3c037-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="3c037-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c037-106">Properties</span></span>
|<span data-ttu-id="3c037-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c037-107">Property</span></span>|<span data-ttu-id="3c037-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3c037-108">Type</span></span>|<span data-ttu-id="3c037-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c037-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c037-110">validationName</span><span class="sxs-lookup"><span data-stu-id="3c037-110">validationName</span></span>|<span data-ttu-id="3c037-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c037-111">String</span></span>|<span data-ttu-id="3c037-112">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="3c037-112">The validation friendly name</span></span>|
|<span data-ttu-id="3c037-113">state</span><span class="sxs-lookup"><span data-stu-id="3c037-113">state</span></span>|<span data-ttu-id="3c037-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c037-114">String</span></span>|<span data-ttu-id="3c037-115">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="3c037-115">The state of the operation</span></span>|
|<span data-ttu-id="3c037-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="3c037-116">mitigationInstruction</span></span>|<span data-ttu-id="3c037-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c037-117">String</span></span>|<span data-ttu-id="3c037-118">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="3c037-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c037-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3c037-119">Relationships</span></span>
<span data-ttu-id="3c037-120">Keine</span><span class="sxs-lookup"><span data-stu-id="3c037-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c037-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c037-121">JSON Representation</span></span>
<span data-ttu-id="3c037-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c037-122">Here is a JSON representation of the resource.</span></span>
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



