---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
ms.openlocfilehash: 1618c65b46654832fc7706f01cb6d6a9f78926e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314777"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="3c983-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c983-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="3c983-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3c983-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c983-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c983-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c983-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3c983-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c983-107">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="3c983-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="3c983-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c983-108">Properties</span></span>
|<span data-ttu-id="3c983-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c983-109">Property</span></span>|<span data-ttu-id="3c983-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3c983-110">Type</span></span>|<span data-ttu-id="3c983-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c983-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c983-112">validationName</span><span class="sxs-lookup"><span data-stu-id="3c983-112">validationName</span></span>|<span data-ttu-id="3c983-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c983-113">String</span></span>|<span data-ttu-id="3c983-114">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="3c983-114">The validation friendly name</span></span>|
|<span data-ttu-id="3c983-115">state</span><span class="sxs-lookup"><span data-stu-id="3c983-115">state</span></span>|<span data-ttu-id="3c983-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c983-116">String</span></span>|<span data-ttu-id="3c983-117">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="3c983-117">The state of the operation</span></span>|
|<span data-ttu-id="3c983-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="3c983-118">mitigationInstruction</span></span>|<span data-ttu-id="3c983-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c983-119">String</span></span>|<span data-ttu-id="3c983-120">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="3c983-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c983-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3c983-121">Relationships</span></span>
<span data-ttu-id="3c983-122">Keine</span><span class="sxs-lookup"><span data-stu-id="3c983-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c983-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c983-123">JSON Representation</span></span>
<span data-ttu-id="3c983-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c983-124">Here is a JSON representation of the resource.</span></span>
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





