---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
ms.openlocfilehash: 44284b54692e4a123b1837bbfb0f5f04a2b01a2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065608"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="93425-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93425-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="93425-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93425-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93425-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93425-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93425-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93425-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93425-107">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="93425-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="93425-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93425-108">Properties</span></span>
|<span data-ttu-id="93425-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93425-109">Property</span></span>|<span data-ttu-id="93425-110">Typ</span><span class="sxs-lookup"><span data-stu-id="93425-110">Type</span></span>|<span data-ttu-id="93425-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93425-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93425-112">validationName</span><span class="sxs-lookup"><span data-stu-id="93425-112">validationName</span></span>|<span data-ttu-id="93425-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93425-113">String</span></span>|<span data-ttu-id="93425-114">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="93425-114">The validation friendly name</span></span>|
|<span data-ttu-id="93425-115">state</span><span class="sxs-lookup"><span data-stu-id="93425-115">state</span></span>|<span data-ttu-id="93425-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93425-116">String</span></span>|<span data-ttu-id="93425-117">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="93425-117">The state of the operation</span></span>|
|<span data-ttu-id="93425-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="93425-118">mitigationInstruction</span></span>|<span data-ttu-id="93425-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93425-119">String</span></span>|<span data-ttu-id="93425-120">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="93425-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="93425-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="93425-121">Relationships</span></span>
<span data-ttu-id="93425-122">Keine</span><span class="sxs-lookup"><span data-stu-id="93425-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="93425-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93425-123">JSON Representation</span></span>
<span data-ttu-id="93425-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93425-124">Here is a JSON representation of the resource.</span></span>
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





