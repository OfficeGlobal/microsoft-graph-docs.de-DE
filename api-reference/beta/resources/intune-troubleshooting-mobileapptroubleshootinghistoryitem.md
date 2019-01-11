---
title: Ressourcentyp mobileAppTroubleshootingHistoryItem
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4db29e7badc8748e4aa64f318b68e0f21d0da5db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867928"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="a6dcc-103">Ressourcentyp mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="a6dcc-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="a6dcc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6dcc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6dcc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6dcc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6dcc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6dcc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6dcc-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="a6dcc-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="a6dcc-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a6dcc-108">Properties</span></span>
|<span data-ttu-id="a6dcc-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6dcc-109">Property</span></span>|<span data-ttu-id="a6dcc-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a6dcc-110">Type</span></span>|<span data-ttu-id="a6dcc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6dcc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6dcc-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="a6dcc-112">occurrenceDateTime</span></span>|<span data-ttu-id="a6dcc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6dcc-113">DateTimeOffset</span></span>|<span data-ttu-id="a6dcc-114">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="a6dcc-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6dcc-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a6dcc-115">Relationships</span></span>
<span data-ttu-id="a6dcc-116">Keine</span><span class="sxs-lookup"><span data-stu-id="a6dcc-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6dcc-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a6dcc-117">JSON Representation</span></span>
<span data-ttu-id="a6dcc-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a6dcc-118">Here is a JSON representation of the resource.</span></span>
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





