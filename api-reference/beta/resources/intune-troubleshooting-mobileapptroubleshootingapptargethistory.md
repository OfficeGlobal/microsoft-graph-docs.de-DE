---
title: mobileAppTroubleshootingAppTargetHistory-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a7171cdde4889ba97a9cd29c4cc8c81ab1a9d58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159353"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="6a60f-103">mobileAppTroubleshootingAppTargetHistory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6a60f-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="6a60f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a60f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a60f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6a60f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a60f-106">Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="6a60f-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="6a60f-107">Erbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a60f-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a60f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a60f-108">Properties</span></span>
|<span data-ttu-id="6a60f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a60f-109">Property</span></span>|<span data-ttu-id="6a60f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6a60f-110">Type</span></span>|<span data-ttu-id="6a60f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a60f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a60f-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="6a60f-112">occurrenceDateTime</span></span>|<span data-ttu-id="6a60f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a60f-113">DateTimeOffset</span></span>|<span data-ttu-id="6a60f-114">Zeitpunkt, zu dem das Verlaufselement aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="6a60f-114">Time when the history item occurred.</span></span> <span data-ttu-id="6a60f-115">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a60f-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="6a60f-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="6a60f-116">securityGroupId</span></span>|<span data-ttu-id="6a60f-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a60f-117">String</span></span>|<span data-ttu-id="6a60f-118">AAD-Sicherheitsgruppen-ID, auf die Sie gezielt wurde.</span><span class="sxs-lookup"><span data-stu-id="6a60f-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="6a60f-119">runState</span><span class="sxs-lookup"><span data-stu-id="6a60f-119">runState</span></span>|[<span data-ttu-id="6a60f-120">runState</span><span class="sxs-lookup"><span data-stu-id="6a60f-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="6a60f-121">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="6a60f-121">Status of the item.</span></span> <span data-ttu-id="6a60f-122">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="6a60f-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="6a60f-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="6a60f-123">errorCode</span></span>|<span data-ttu-id="6a60f-124">String</span><span class="sxs-lookup"><span data-stu-id="6a60f-124">String</span></span>|<span data-ttu-id="6a60f-125">Fehlercode für den Fehler, leer, wenn kein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="6a60f-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a60f-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a60f-126">Relationships</span></span>
<span data-ttu-id="6a60f-127">Keine</span><span class="sxs-lookup"><span data-stu-id="6a60f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a60f-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a60f-128">JSON Representation</span></span>
<span data-ttu-id="6a60f-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a60f-129">Here is a JSON representation of the resource.</span></span>
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




