---
title: Ressourcentyp mobileAppTroubleshootingAppTargetHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9da17e4a03d1a28c32215b8616dad2ea3700ef4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969422"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="f1451-103">Ressourcentyp mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="f1451-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="f1451-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1451-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1451-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1451-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1451-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1451-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1451-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="f1451-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="f1451-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f1451-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1451-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1451-109">Properties</span></span>
|<span data-ttu-id="f1451-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1451-110">Property</span></span>|<span data-ttu-id="f1451-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f1451-111">Type</span></span>|<span data-ttu-id="f1451-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1451-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1451-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="f1451-113">occurrenceDateTime</span></span>|<span data-ttu-id="f1451-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1451-114">DateTimeOffset</span></span>|<span data-ttu-id="f1451-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="f1451-115">Time when the history item occurred.</span></span> <span data-ttu-id="f1451-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f1451-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="f1451-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="f1451-117">securityGroupId</span></span>|<span data-ttu-id="f1451-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1451-118">String</span></span>|<span data-ttu-id="f1451-119">AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="f1451-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="f1451-120">runState</span><span class="sxs-lookup"><span data-stu-id="f1451-120">runState</span></span>|[<span data-ttu-id="f1451-121">runState</span><span class="sxs-lookup"><span data-stu-id="f1451-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f1451-122">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="f1451-122">Status of the item.</span></span> <span data-ttu-id="f1451-123">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="f1451-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="f1451-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="f1451-124">errorCode</span></span>|<span data-ttu-id="f1451-125">String</span><span class="sxs-lookup"><span data-stu-id="f1451-125">String</span></span>|<span data-ttu-id="f1451-126">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="f1451-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1451-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f1451-127">Relationships</span></span>
<span data-ttu-id="f1451-128">Keine</span><span class="sxs-lookup"><span data-stu-id="f1451-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1451-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1451-129">JSON Representation</span></span>
<span data-ttu-id="f1451-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1451-130">Here is a JSON representation of the resource.</span></span>
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





