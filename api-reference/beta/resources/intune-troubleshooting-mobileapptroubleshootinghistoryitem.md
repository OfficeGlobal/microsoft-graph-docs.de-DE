---
title: mobileAppTroubleshootingHistoryItem-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbc37488f478c47b0b097c4fd8a54b09273bc5c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160858"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="50bff-103">mobileAppTroubleshootingHistoryItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50bff-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="50bff-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50bff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50bff-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="50bff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50bff-106">Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="50bff-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="50bff-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50bff-107">Properties</span></span>
|<span data-ttu-id="50bff-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50bff-108">Property</span></span>|<span data-ttu-id="50bff-109">Typ</span><span class="sxs-lookup"><span data-stu-id="50bff-109">Type</span></span>|<span data-ttu-id="50bff-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50bff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50bff-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="50bff-111">occurrenceDateTime</span></span>|<span data-ttu-id="50bff-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50bff-112">DateTimeOffset</span></span>|<span data-ttu-id="50bff-113">Zeitpunkt, zu dem das Verlaufselement aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="50bff-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50bff-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="50bff-114">Relationships</span></span>
<span data-ttu-id="50bff-115">Keine</span><span class="sxs-lookup"><span data-stu-id="50bff-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50bff-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50bff-116">JSON Representation</span></span>
<span data-ttu-id="50bff-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50bff-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```




