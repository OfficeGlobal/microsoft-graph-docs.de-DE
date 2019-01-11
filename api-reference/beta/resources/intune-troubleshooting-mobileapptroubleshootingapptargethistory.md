---
title: Ressourcentyp mobileAppTroubleshootingAppTargetHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76595f4fd643e985d28bcb84ad1c4ea6d7be2ad6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810339"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="1a2c6-103">Ressourcentyp mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="1a2c6-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="1a2c6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a2c6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a2c6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a2c6-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="1a2c6-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a2c6-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a2c6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1a2c6-109">Properties</span></span>
|<span data-ttu-id="1a2c6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a2c6-110">Property</span></span>|<span data-ttu-id="1a2c6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1a2c6-111">Type</span></span>|<span data-ttu-id="1a2c6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a2c6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a2c6-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2c6-113">occurrenceDateTime</span></span>|<span data-ttu-id="1a2c6-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2c6-114">DateTimeOffset</span></span>|<span data-ttu-id="1a2c6-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-115">Time when the history item occurred.</span></span> <span data-ttu-id="1a2c6-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a2c6-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="1a2c6-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="1a2c6-117">securityGroupId</span></span>|<span data-ttu-id="1a2c6-118">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-118">String</span></span>|<span data-ttu-id="1a2c6-119">AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="1a2c6-120">runState</span><span class="sxs-lookup"><span data-stu-id="1a2c6-120">runState</span></span>|[<span data-ttu-id="1a2c6-121">runState</span><span class="sxs-lookup"><span data-stu-id="1a2c6-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="1a2c6-122">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-122">Status of the item.</span></span> <span data-ttu-id="1a2c6-123">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="1a2c6-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="1a2c6-124">errorCode</span></span>|<span data-ttu-id="1a2c6-125">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-125">String</span></span>|<span data-ttu-id="1a2c6-126">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a2c6-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1a2c6-127">Relationships</span></span>
<span data-ttu-id="1a2c6-128">Keine</span><span class="sxs-lookup"><span data-stu-id="1a2c6-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a2c6-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1a2c6-129">JSON Representation</span></span>
<span data-ttu-id="1a2c6-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```





