---
title: Ressourcentyp mobileAppTroubleshootingAppPolicyCreationHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0ee2088856c9c47771b3e647615f82fe26dfd552
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924391"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="ad835-103">Ressourcentyp mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="ad835-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="ad835-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ad835-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad835-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad835-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ad835-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad835-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="ad835-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="ad835-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ad835-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad835-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad835-109">Properties</span></span>
|<span data-ttu-id="ad835-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad835-110">Property</span></span>|<span data-ttu-id="ad835-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ad835-111">Type</span></span>|<span data-ttu-id="ad835-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad835-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad835-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ad835-113">occurrenceDateTime</span></span>|<span data-ttu-id="ad835-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad835-114">DateTimeOffset</span></span>|<span data-ttu-id="ad835-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="ad835-115">Time when the history item occurred.</span></span> <span data-ttu-id="ad835-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ad835-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="ad835-117">runState</span><span class="sxs-lookup"><span data-stu-id="ad835-117">runState</span></span>|[<span data-ttu-id="ad835-118">runState</span><span class="sxs-lookup"><span data-stu-id="ad835-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="ad835-119">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="ad835-119">Status of the item.</span></span> <span data-ttu-id="ad835-120">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="ad835-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="ad835-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="ad835-121">errorCode</span></span>|<span data-ttu-id="ad835-122">String</span><span class="sxs-lookup"><span data-stu-id="ad835-122">String</span></span>|<span data-ttu-id="ad835-123">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="ad835-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad835-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ad835-124">Relationships</span></span>
<span data-ttu-id="ad835-125">Keine</span><span class="sxs-lookup"><span data-stu-id="ad835-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad835-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad835-126">JSON Representation</span></span>
<span data-ttu-id="ad835-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad835-127">Here is a JSON representation of the resource.</span></span>
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





