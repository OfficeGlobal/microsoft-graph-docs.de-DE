---
title: Ressourcentyp mobileAppTroubleshootingAppStateHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
ms.openlocfilehash: 415d018d3650819bce8defe651af8df77e3c6032
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060512"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="5b8bd-103">Ressourcentyp mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="5b8bd-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="5b8bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b8bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b8bd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b8bd-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="5b8bd-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5b8bd-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b8bd-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5b8bd-109">Properties</span></span>
|<span data-ttu-id="5b8bd-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b8bd-110">Property</span></span>|<span data-ttu-id="5b8bd-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5b8bd-111">Type</span></span>|<span data-ttu-id="5b8bd-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b8bd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b8bd-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5b8bd-113">occurrenceDateTime</span></span>|<span data-ttu-id="5b8bd-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b8bd-114">DateTimeOffset</span></span>|<span data-ttu-id="5b8bd-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-115">Time when the history item occurred.</span></span> <span data-ttu-id="5b8bd-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5b8bd-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5b8bd-117">actionType</span><span class="sxs-lookup"><span data-stu-id="5b8bd-117">actionType</span></span>|[<span data-ttu-id="5b8bd-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="5b8bd-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="5b8bd-119">AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="5b8bd-120">Mögliche Werte sind: `unknown`, `installCommandSent`, `installed`, `uninstalled` und `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="5b8bd-121">runState</span><span class="sxs-lookup"><span data-stu-id="5b8bd-121">runState</span></span>|[<span data-ttu-id="5b8bd-122">runState</span><span class="sxs-lookup"><span data-stu-id="5b8bd-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5b8bd-123">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-123">Status of the item.</span></span> <span data-ttu-id="5b8bd-124">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="5b8bd-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="5b8bd-125">errorCode</span></span>|<span data-ttu-id="5b8bd-126">String</span><span class="sxs-lookup"><span data-stu-id="5b8bd-126">String</span></span>|<span data-ttu-id="5b8bd-127">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b8bd-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5b8bd-128">Relationships</span></span>
<span data-ttu-id="5b8bd-129">Keine</span><span class="sxs-lookup"><span data-stu-id="5b8bd-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b8bd-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5b8bd-130">JSON Representation</span></span>
<span data-ttu-id="5b8bd-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5b8bd-131">Here is a JSON representation of the resource.</span></span>
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





