---
title: Ressourcentyp mobileAppTroubleshootingDeviceCheckinHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2fc4cd56b1f900eb3198cbfc078af1e894f2035
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940961"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="588b9-103">Ressourcentyp mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="588b9-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="588b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="588b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="588b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="588b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="588b9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="588b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="588b9-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="588b9-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="588b9-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="588b9-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="588b9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="588b9-109">Properties</span></span>
|<span data-ttu-id="588b9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="588b9-110">Property</span></span>|<span data-ttu-id="588b9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="588b9-111">Type</span></span>|<span data-ttu-id="588b9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="588b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="588b9-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="588b9-113">occurrenceDateTime</span></span>|<span data-ttu-id="588b9-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="588b9-114">DateTimeOffset</span></span>|<span data-ttu-id="588b9-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="588b9-115">Time when the history item occurred.</span></span> <span data-ttu-id="588b9-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="588b9-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="588b9-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="588b9-117">Relationships</span></span>
<span data-ttu-id="588b9-118">Keine</span><span class="sxs-lookup"><span data-stu-id="588b9-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="588b9-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="588b9-119">JSON Representation</span></span>
<span data-ttu-id="588b9-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="588b9-120">Here is a JSON representation of the resource.</span></span>
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





