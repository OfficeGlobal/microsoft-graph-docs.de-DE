---
title: Ressourcentyp mobileAppTroubleshootingAppUpdateHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
ms.openlocfilehash: d546475f568c279137e411d546765fe828c43975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062571"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="85ea5-103">Ressourcentyp mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="85ea5-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="85ea5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85ea5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85ea5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85ea5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85ea5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85ea5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85ea5-107">Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.</span><span class="sxs-lookup"><span data-stu-id="85ea5-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="85ea5-108">Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="85ea5-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85ea5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85ea5-109">Properties</span></span>
|<span data-ttu-id="85ea5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85ea5-110">Property</span></span>|<span data-ttu-id="85ea5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="85ea5-111">Type</span></span>|<span data-ttu-id="85ea5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85ea5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85ea5-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="85ea5-113">occurrenceDateTime</span></span>|<span data-ttu-id="85ea5-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85ea5-114">DateTimeOffset</span></span>|<span data-ttu-id="85ea5-115">Zeitpunkt, wenn das Historienelement aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="85ea5-115">Time when the history item occurred.</span></span> <span data-ttu-id="85ea5-116">Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="85ea5-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="85ea5-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="85ea5-117">Relationships</span></span>
<span data-ttu-id="85ea5-118">Keine</span><span class="sxs-lookup"><span data-stu-id="85ea5-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85ea5-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85ea5-119">JSON Representation</span></span>
<span data-ttu-id="85ea5-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85ea5-120">Here is a JSON representation of the resource.</span></span>
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





