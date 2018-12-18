---
title: Ressourcentyp mobileAppTroubleshootingHistoryItem
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
author: tfitzmac
ms.openlocfilehash: 132039a0b6e457ebd2ca3e545f6f15dd4ad7ac58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329526"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="d81b2-103">Ressourcentyp mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="d81b2-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="d81b2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d81b2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d81b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d81b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d81b2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d81b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d81b2-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="d81b2-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="d81b2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d81b2-108">Properties</span></span>
|<span data-ttu-id="d81b2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d81b2-109">Property</span></span>|<span data-ttu-id="d81b2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d81b2-110">Type</span></span>|<span data-ttu-id="d81b2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d81b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81b2-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d81b2-112">occurrenceDateTime</span></span>|<span data-ttu-id="d81b2-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81b2-113">DateTimeOffset</span></span>|<span data-ttu-id="d81b2-114">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="d81b2-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d81b2-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d81b2-115">Relationships</span></span>
<span data-ttu-id="d81b2-116">Keine</span><span class="sxs-lookup"><span data-stu-id="d81b2-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d81b2-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d81b2-117">JSON Representation</span></span>
<span data-ttu-id="d81b2-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d81b2-118">Here is a JSON representation of the resource.</span></span>
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





