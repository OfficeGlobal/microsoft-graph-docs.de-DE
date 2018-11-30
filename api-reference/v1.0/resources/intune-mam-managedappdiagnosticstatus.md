---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
ms.openlocfilehash: 8a462b49231323288d66a660c769ce7359cb5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018439"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="c452f-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c452f-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="c452f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c452f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c452f-105">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="c452f-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="c452f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c452f-106">Properties</span></span>
|<span data-ttu-id="c452f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c452f-107">Property</span></span>|<span data-ttu-id="c452f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c452f-108">Type</span></span>|<span data-ttu-id="c452f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c452f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c452f-110">validationName</span><span class="sxs-lookup"><span data-stu-id="c452f-110">validationName</span></span>|<span data-ttu-id="c452f-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c452f-111">String</span></span>|<span data-ttu-id="c452f-112">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="c452f-112">The validation friendly name</span></span>|
|<span data-ttu-id="c452f-113">state</span><span class="sxs-lookup"><span data-stu-id="c452f-113">state</span></span>|<span data-ttu-id="c452f-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c452f-114">String</span></span>|<span data-ttu-id="c452f-115">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="c452f-115">The state of the operation</span></span>|
|<span data-ttu-id="c452f-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="c452f-116">mitigationInstruction</span></span>|<span data-ttu-id="c452f-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c452f-117">String</span></span>|<span data-ttu-id="c452f-118">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="c452f-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="c452f-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c452f-119">Relationships</span></span>
<span data-ttu-id="c452f-120">Keine</span><span class="sxs-lookup"><span data-stu-id="c452f-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c452f-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c452f-121">JSON Representation</span></span>
<span data-ttu-id="c452f-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c452f-122">Here is a JSON representation of the resource.</span></span>
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



