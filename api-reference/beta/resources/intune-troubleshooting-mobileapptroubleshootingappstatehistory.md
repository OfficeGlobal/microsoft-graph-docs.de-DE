---
title: Ressourcentyp mobileAppTroubleshootingAppStateHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57e10fcabc0aa3def07872c0e520f09c6ee90fc3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411239"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="5160d-103">Ressourcentyp mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="5160d-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="5160d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5160d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5160d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5160d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5160d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5160d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5160d-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="5160d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5160d-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5160d-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5160d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5160d-109">Properties</span></span>
|<span data-ttu-id="5160d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5160d-110">Property</span></span>|<span data-ttu-id="5160d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5160d-111">Type</span></span>|<span data-ttu-id="5160d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5160d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5160d-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5160d-113">occurrenceDateTime</span></span>|<span data-ttu-id="5160d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5160d-114">DateTimeOffset</span></span>|<span data-ttu-id="5160d-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="5160d-115">Time when the history item occurred.</span></span> <span data-ttu-id="5160d-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5160d-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5160d-117">actionType</span><span class="sxs-lookup"><span data-stu-id="5160d-117">actionType</span></span>|[<span data-ttu-id="5160d-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="5160d-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="5160d-119">AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="5160d-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="5160d-120">Mögliche Werte sind: `unknown`, `installCommandSent`, `installed`, `uninstalled` und `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="5160d-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="5160d-121">runState</span><span class="sxs-lookup"><span data-stu-id="5160d-121">runState</span></span>|[<span data-ttu-id="5160d-122">runState</span><span class="sxs-lookup"><span data-stu-id="5160d-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5160d-123">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="5160d-123">Status of the item.</span></span> <span data-ttu-id="5160d-124">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="5160d-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="5160d-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="5160d-125">errorCode</span></span>|<span data-ttu-id="5160d-126">String</span><span class="sxs-lookup"><span data-stu-id="5160d-126">String</span></span>|<span data-ttu-id="5160d-127">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="5160d-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5160d-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5160d-128">Relationships</span></span>
<span data-ttu-id="5160d-129">Keine</span><span class="sxs-lookup"><span data-stu-id="5160d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5160d-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5160d-130">JSON Representation</span></span>
<span data-ttu-id="5160d-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5160d-131">Here is a JSON representation of the resource.</span></span>
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




