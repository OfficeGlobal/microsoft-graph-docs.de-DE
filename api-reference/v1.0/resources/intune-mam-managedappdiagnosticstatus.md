---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2477039c3a0ebca3de09a4042691045782848b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261551"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="3e933-103">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3e933-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="3e933-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3e933-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e933-105">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="3e933-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="3e933-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3e933-106">Properties</span></span>
|<span data-ttu-id="3e933-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e933-107">Property</span></span>|<span data-ttu-id="3e933-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3e933-108">Type</span></span>|<span data-ttu-id="3e933-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e933-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e933-110">validationName</span><span class="sxs-lookup"><span data-stu-id="3e933-110">validationName</span></span>|<span data-ttu-id="3e933-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e933-111">String</span></span>|<span data-ttu-id="3e933-112">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="3e933-112">The validation friendly name</span></span>|
|<span data-ttu-id="3e933-113">state</span><span class="sxs-lookup"><span data-stu-id="3e933-113">state</span></span>|<span data-ttu-id="3e933-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e933-114">String</span></span>|<span data-ttu-id="3e933-115">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="3e933-115">The state of the operation</span></span>|
|<span data-ttu-id="3e933-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="3e933-116">mitigationInstruction</span></span>|<span data-ttu-id="3e933-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e933-117">String</span></span>|<span data-ttu-id="3e933-118">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="3e933-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e933-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3e933-119">Relationships</span></span>
<span data-ttu-id="3e933-120">Keine</span><span class="sxs-lookup"><span data-stu-id="3e933-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e933-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3e933-121">JSON Representation</span></span>
<span data-ttu-id="3e933-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3e933-122">Here is a JSON representation of the resource.</span></span>
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



