---
title: Ressourcentyp mobileAppTroubleshootingAppUpdateHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 606fe9dcf282dd75992f5a936aa5f49dfbb61dc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414207"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="6a5b4-103">Ressourcentyp mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="6a5b4-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="6a5b4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6a5b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a5b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a5b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a5b4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a5b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a5b4-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="6a5b4-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="6a5b4-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a5b4-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a5b4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a5b4-109">Properties</span></span>
|<span data-ttu-id="6a5b4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a5b4-110">Property</span></span>|<span data-ttu-id="6a5b4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6a5b4-111">Type</span></span>|<span data-ttu-id="6a5b4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a5b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a5b4-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="6a5b4-113">occurrenceDateTime</span></span>|<span data-ttu-id="6a5b4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a5b4-114">DateTimeOffset</span></span>|<span data-ttu-id="6a5b4-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="6a5b4-115">Time when the history item occurred.</span></span> <span data-ttu-id="6a5b4-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a5b4-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a5b4-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a5b4-117">Relationships</span></span>
<span data-ttu-id="6a5b4-118">Keine</span><span class="sxs-lookup"><span data-stu-id="6a5b4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a5b4-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a5b4-119">JSON Representation</span></span>
<span data-ttu-id="6a5b4-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a5b4-120">Here is a JSON representation of the resource.</span></span>
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




