---
title: Ressourcentyp mobileAppTroubleshootingDeviceCheckinHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6b9d900e712e3c3b126dd36671049e8935f09a83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844947"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="b42ba-103">Ressourcentyp mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="b42ba-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="b42ba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b42ba-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b42ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b42ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b42ba-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b42ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b42ba-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="b42ba-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="b42ba-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b42ba-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b42ba-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b42ba-109">Properties</span></span>
|<span data-ttu-id="b42ba-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b42ba-110">Property</span></span>|<span data-ttu-id="b42ba-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b42ba-111">Type</span></span>|<span data-ttu-id="b42ba-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b42ba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b42ba-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="b42ba-113">occurrenceDateTime</span></span>|<span data-ttu-id="b42ba-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b42ba-114">DateTimeOffset</span></span>|<span data-ttu-id="b42ba-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="b42ba-115">Time when the history item occurred.</span></span> <span data-ttu-id="b42ba-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b42ba-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b42ba-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b42ba-117">Relationships</span></span>
<span data-ttu-id="b42ba-118">Keine</span><span class="sxs-lookup"><span data-stu-id="b42ba-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b42ba-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b42ba-119">JSON Representation</span></span>
<span data-ttu-id="b42ba-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b42ba-120">Here is a JSON representation of the resource.</span></span>
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





