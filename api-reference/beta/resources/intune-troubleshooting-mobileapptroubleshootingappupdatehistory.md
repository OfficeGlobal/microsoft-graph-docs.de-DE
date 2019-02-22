---
title: mobileAppTroubleshootingAppUpdateHistory-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eadbec77e95dd90fd9ef819e468241bf8ef5c9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153641"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="57dce-103">mobileAppTroubleshootingAppUpdateHistory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="57dce-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="57dce-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57dce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57dce-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="57dce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57dce-106">Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="57dce-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="57dce-107">Erbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="57dce-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57dce-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="57dce-108">Properties</span></span>
|<span data-ttu-id="57dce-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57dce-109">Property</span></span>|<span data-ttu-id="57dce-110">Typ</span><span class="sxs-lookup"><span data-stu-id="57dce-110">Type</span></span>|<span data-ttu-id="57dce-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57dce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57dce-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="57dce-112">occurrenceDateTime</span></span>|<span data-ttu-id="57dce-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dce-113">DateTimeOffset</span></span>|<span data-ttu-id="57dce-114">Zeitpunkt, zu dem das Verlaufselement aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="57dce-114">Time when the history item occurred.</span></span> <span data-ttu-id="57dce-115">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="57dce-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="57dce-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="57dce-116">Relationships</span></span>
<span data-ttu-id="57dce-117">Keine</span><span class="sxs-lookup"><span data-stu-id="57dce-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57dce-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="57dce-118">JSON Representation</span></span>
<span data-ttu-id="57dce-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="57dce-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




