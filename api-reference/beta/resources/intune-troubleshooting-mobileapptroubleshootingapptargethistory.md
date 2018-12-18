---
title: Ressourcentyp mobileAppTroubleshootingAppTargetHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
ms.openlocfilehash: cdb901d4c532b57025837a2fb0cc0975ceba3f8c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312733"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="dcca3-103">Ressourcentyp mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="dcca3-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="dcca3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dcca3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcca3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcca3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcca3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dcca3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dcca3-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="dcca3-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="dcca3-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dcca3-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dcca3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dcca3-109">Properties</span></span>
|<span data-ttu-id="dcca3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dcca3-110">Property</span></span>|<span data-ttu-id="dcca3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dcca3-111">Type</span></span>|<span data-ttu-id="dcca3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcca3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcca3-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="dcca3-113">occurrenceDateTime</span></span>|<span data-ttu-id="dcca3-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcca3-114">DateTimeOffset</span></span>|<span data-ttu-id="dcca3-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="dcca3-115">Time when the history item occurred.</span></span> <span data-ttu-id="dcca3-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dcca3-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="dcca3-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="dcca3-117">securityGroupId</span></span>|<span data-ttu-id="dcca3-118">String</span><span class="sxs-lookup"><span data-stu-id="dcca3-118">String</span></span>|<span data-ttu-id="dcca3-119">AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="dcca3-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="dcca3-120">runState</span><span class="sxs-lookup"><span data-stu-id="dcca3-120">runState</span></span>|[<span data-ttu-id="dcca3-121">runState</span><span class="sxs-lookup"><span data-stu-id="dcca3-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="dcca3-122">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="dcca3-122">Status of the item.</span></span> <span data-ttu-id="dcca3-123">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="dcca3-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="dcca3-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="dcca3-124">errorCode</span></span>|<span data-ttu-id="dcca3-125">String</span><span class="sxs-lookup"><span data-stu-id="dcca3-125">String</span></span>|<span data-ttu-id="dcca3-126">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="dcca3-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcca3-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dcca3-127">Relationships</span></span>
<span data-ttu-id="dcca3-128">Keine</span><span class="sxs-lookup"><span data-stu-id="dcca3-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dcca3-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dcca3-129">JSON Representation</span></span>
<span data-ttu-id="dcca3-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dcca3-130">Here is a JSON representation of the resource.</span></span>
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





