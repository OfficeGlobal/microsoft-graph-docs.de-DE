---
title: Ressourcentyp mobileAppTroubleshootingDeviceCheckinHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43816929fd01be56b7487e3c0101ca08c928ac85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410168"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="8c343-103">Ressourcentyp mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="8c343-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="8c343-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8c343-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c343-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c343-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c343-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c343-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c343-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="8c343-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="8c343-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8c343-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c343-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c343-109">Properties</span></span>
|<span data-ttu-id="8c343-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c343-110">Property</span></span>|<span data-ttu-id="8c343-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8c343-111">Type</span></span>|<span data-ttu-id="8c343-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c343-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c343-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="8c343-113">occurrenceDateTime</span></span>|<span data-ttu-id="8c343-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c343-114">DateTimeOffset</span></span>|<span data-ttu-id="8c343-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="8c343-115">Time when the history item occurred.</span></span> <span data-ttu-id="8c343-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8c343-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c343-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8c343-117">Relationships</span></span>
<span data-ttu-id="8c343-118">Keine</span><span class="sxs-lookup"><span data-stu-id="8c343-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c343-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8c343-119">JSON Representation</span></span>
<span data-ttu-id="8c343-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8c343-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




