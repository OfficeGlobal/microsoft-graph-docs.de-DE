---
title: Ressourcentyp mobileAppTroubleshootingAppPolicyCreationHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd7880a6d931fafda46ab4adf0668835438ddcb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870105"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="23ec4-103">Ressourcentyp mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="23ec4-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="23ec4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23ec4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23ec4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23ec4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23ec4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23ec4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23ec4-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="23ec4-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="23ec4-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="23ec4-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23ec4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23ec4-109">Properties</span></span>
|<span data-ttu-id="23ec4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23ec4-110">Property</span></span>|<span data-ttu-id="23ec4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="23ec4-111">Type</span></span>|<span data-ttu-id="23ec4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23ec4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ec4-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="23ec4-113">occurrenceDateTime</span></span>|<span data-ttu-id="23ec4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ec4-114">DateTimeOffset</span></span>|<span data-ttu-id="23ec4-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="23ec4-115">Time when the history item occurred.</span></span> <span data-ttu-id="23ec4-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="23ec4-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="23ec4-117">runState</span><span class="sxs-lookup"><span data-stu-id="23ec4-117">runState</span></span>|[<span data-ttu-id="23ec4-118">runState</span><span class="sxs-lookup"><span data-stu-id="23ec4-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="23ec4-119">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="23ec4-119">Status of the item.</span></span> <span data-ttu-id="23ec4-120">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="23ec4-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="23ec4-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="23ec4-121">errorCode</span></span>|<span data-ttu-id="23ec4-122">String</span><span class="sxs-lookup"><span data-stu-id="23ec4-122">String</span></span>|<span data-ttu-id="23ec4-123">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="23ec4-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23ec4-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23ec4-124">Relationships</span></span>
<span data-ttu-id="23ec4-125">Keine</span><span class="sxs-lookup"><span data-stu-id="23ec4-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23ec4-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23ec4-126">JSON Representation</span></span>
<span data-ttu-id="23ec4-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23ec4-127">Here is a JSON representation of the resource.</span></span>
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





