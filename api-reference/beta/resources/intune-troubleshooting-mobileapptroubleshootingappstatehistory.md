---
title: mobileAppTroubleshootingAppStateHistory-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd39115de207532b42d1554da54e154a5066eb76
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150960"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="089d3-103">mobileAppTroubleshootingAppStateHistory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="089d3-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="089d3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="089d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="089d3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="089d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089d3-106">Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="089d3-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="089d3-107">Erbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="089d3-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="089d3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="089d3-108">Properties</span></span>
|<span data-ttu-id="089d3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="089d3-109">Property</span></span>|<span data-ttu-id="089d3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="089d3-110">Type</span></span>|<span data-ttu-id="089d3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="089d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089d3-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="089d3-112">occurrenceDateTime</span></span>|<span data-ttu-id="089d3-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="089d3-113">DateTimeOffset</span></span>|<span data-ttu-id="089d3-114">Zeitpunkt, zu dem das Verlaufselement aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="089d3-114">Time when the history item occurred.</span></span> <span data-ttu-id="089d3-115">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="089d3-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="089d3-116">actionType</span><span class="sxs-lookup"><span data-stu-id="089d3-116">actionType</span></span>|[<span data-ttu-id="089d3-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="089d3-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="089d3-118">AAD-Sicherheitsgruppen-ID, auf die Sie gezielt wurde.</span><span class="sxs-lookup"><span data-stu-id="089d3-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="089d3-119">Mögliche Werte: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="089d3-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="089d3-120">runState</span><span class="sxs-lookup"><span data-stu-id="089d3-120">runState</span></span>|[<span data-ttu-id="089d3-121">runState</span><span class="sxs-lookup"><span data-stu-id="089d3-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="089d3-122">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="089d3-122">Status of the item.</span></span> <span data-ttu-id="089d3-123">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="089d3-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="089d3-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="089d3-124">errorCode</span></span>|<span data-ttu-id="089d3-125">String</span><span class="sxs-lookup"><span data-stu-id="089d3-125">String</span></span>|<span data-ttu-id="089d3-126">Fehlercode für den Fehler, leer, wenn kein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="089d3-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="089d3-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="089d3-127">Relationships</span></span>
<span data-ttu-id="089d3-128">Keine</span><span class="sxs-lookup"><span data-stu-id="089d3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="089d3-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="089d3-129">JSON Representation</span></span>
<span data-ttu-id="089d3-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="089d3-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```




