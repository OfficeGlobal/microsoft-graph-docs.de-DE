---
title: Ressourcentyp mobileAppTroubleshootingAppTargetHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a1d37f86ebb43b7d697a9407ce0e3a479b2350
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402965"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="6e866-103">Ressourcentyp mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="6e866-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="6e866-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6e866-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e866-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e866-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e866-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e866-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e866-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="6e866-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="6e866-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6e866-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e866-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6e866-109">Properties</span></span>
|<span data-ttu-id="6e866-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6e866-110">Property</span></span>|<span data-ttu-id="6e866-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6e866-111">Type</span></span>|<span data-ttu-id="6e866-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e866-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e866-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="6e866-113">occurrenceDateTime</span></span>|<span data-ttu-id="6e866-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e866-114">DateTimeOffset</span></span>|<span data-ttu-id="6e866-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="6e866-115">Time when the history item occurred.</span></span> <span data-ttu-id="6e866-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6e866-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="6e866-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="6e866-117">securityGroupId</span></span>|<span data-ttu-id="6e866-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e866-118">String</span></span>|<span data-ttu-id="6e866-119">AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="6e866-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="6e866-120">runState</span><span class="sxs-lookup"><span data-stu-id="6e866-120">runState</span></span>|[<span data-ttu-id="6e866-121">runState</span><span class="sxs-lookup"><span data-stu-id="6e866-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="6e866-122">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="6e866-122">Status of the item.</span></span> <span data-ttu-id="6e866-123">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="6e866-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="6e866-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="6e866-124">errorCode</span></span>|<span data-ttu-id="6e866-125">String</span><span class="sxs-lookup"><span data-stu-id="6e866-125">String</span></span>|<span data-ttu-id="6e866-126">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="6e866-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e866-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6e866-127">Relationships</span></span>
<span data-ttu-id="6e866-128">Keine</span><span class="sxs-lookup"><span data-stu-id="6e866-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e866-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6e866-129">JSON Representation</span></span>
<span data-ttu-id="6e866-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6e866-130">Here is a JSON representation of the resource.</span></span>
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




