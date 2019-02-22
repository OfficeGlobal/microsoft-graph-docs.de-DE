---
title: mobileAppTroubleshootingAppPolicyCreationHistory-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a93b88f850e2fa220903362375774d8a6dded59c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160501"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="5d2d3-103">mobileAppTroubleshootingAppPolicyCreationHistory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5d2d3-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="5d2d3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d2d3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d2d3-106">Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5d2d3-107">Erbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d2d3-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d2d3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5d2d3-108">Properties</span></span>
|<span data-ttu-id="5d2d3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d2d3-109">Property</span></span>|<span data-ttu-id="5d2d3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="5d2d3-110">Type</span></span>|<span data-ttu-id="5d2d3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d2d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d2d3-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5d2d3-112">occurrenceDateTime</span></span>|<span data-ttu-id="5d2d3-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d2d3-113">DateTimeOffset</span></span>|<span data-ttu-id="5d2d3-114">Zeitpunkt, zu dem das Verlaufselement aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-114">Time when the history item occurred.</span></span> <span data-ttu-id="5d2d3-115">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d2d3-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5d2d3-116">runState</span><span class="sxs-lookup"><span data-stu-id="5d2d3-116">runState</span></span>|[<span data-ttu-id="5d2d3-117">runState</span><span class="sxs-lookup"><span data-stu-id="5d2d3-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5d2d3-118">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-118">Status of the item.</span></span> <span data-ttu-id="5d2d3-119">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="5d2d3-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="5d2d3-120">errorCode</span></span>|<span data-ttu-id="5d2d3-121">String</span><span class="sxs-lookup"><span data-stu-id="5d2d3-121">String</span></span>|<span data-ttu-id="5d2d3-122">Fehlercode für den Fehler, leer, wenn kein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d2d3-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5d2d3-123">Relationships</span></span>
<span data-ttu-id="5d2d3-124">Keine</span><span class="sxs-lookup"><span data-stu-id="5d2d3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d2d3-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5d2d3-125">JSON Representation</span></span>
<span data-ttu-id="5d2d3-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5d2d3-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```




