---
title: Ressourcentyp mobileAppTroubleshootingAppPolicyCreationHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e81f7f39cac934a89cf06d77fbcb80581267097b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394558"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="6b421-103">Ressourcentyp mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="6b421-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="6b421-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6b421-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6b421-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b421-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b421-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b421-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b421-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="6b421-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="6b421-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b421-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b421-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b421-109">Properties</span></span>
|<span data-ttu-id="6b421-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b421-110">Property</span></span>|<span data-ttu-id="6b421-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6b421-111">Type</span></span>|<span data-ttu-id="6b421-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b421-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b421-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="6b421-113">occurrenceDateTime</span></span>|<span data-ttu-id="6b421-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b421-114">DateTimeOffset</span></span>|<span data-ttu-id="6b421-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="6b421-115">Time when the history item occurred.</span></span> <span data-ttu-id="6b421-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b421-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="6b421-117">runState</span><span class="sxs-lookup"><span data-stu-id="6b421-117">runState</span></span>|[<span data-ttu-id="6b421-118">runState</span><span class="sxs-lookup"><span data-stu-id="6b421-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="6b421-119">Status des Elements.</span><span class="sxs-lookup"><span data-stu-id="6b421-119">Status of the item.</span></span> <span data-ttu-id="6b421-120">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="6b421-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="6b421-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="6b421-121">errorCode</span></span>|<span data-ttu-id="6b421-122">String</span><span class="sxs-lookup"><span data-stu-id="6b421-122">String</span></span>|<span data-ttu-id="6b421-123">Der Fehlercode des Fehlers, leer, wenn kein Fehler.</span><span class="sxs-lookup"><span data-stu-id="6b421-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b421-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6b421-124">Relationships</span></span>
<span data-ttu-id="6b421-125">Keine</span><span class="sxs-lookup"><span data-stu-id="6b421-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b421-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b421-126">JSON Representation</span></span>
<span data-ttu-id="6b421-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b421-127">Here is a JSON representation of the resource.</span></span>
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




