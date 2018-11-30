---
title: Ressourcentyp officeUserCheckinSummary
description: Entität, die Mandanten Einchecken Stats beschreibt.
ms.openlocfilehash: b8b3cc0c6129782a25a12cf22659cb6849a81e26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060560"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="78368-103">Ressourcentyp officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="78368-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="78368-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78368-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78368-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78368-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78368-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="78368-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78368-107">Entität, die Mandanten Einchecken Stats beschreibt.</span><span class="sxs-lookup"><span data-stu-id="78368-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="78368-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78368-108">Properties</span></span>
|<span data-ttu-id="78368-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78368-109">Property</span></span>|<span data-ttu-id="78368-110">Typ</span><span class="sxs-lookup"><span data-stu-id="78368-110">Type</span></span>|<span data-ttu-id="78368-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78368-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78368-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="78368-112">succeededUserCount</span></span>|<span data-ttu-id="78368-113">Int32</span><span class="sxs-lookup"><span data-stu-id="78368-113">Int32</span></span>|<span data-ttu-id="78368-114">Gesamtzahl erfolgreicher Benutzer überprüfen ins für die letzten drei Monate angezeigt.</span><span class="sxs-lookup"><span data-stu-id="78368-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="78368-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="78368-115">failedUserCount</span></span>|<span data-ttu-id="78368-116">Int32</span><span class="sxs-lookup"><span data-stu-id="78368-116">Int32</span></span>|<span data-ttu-id="78368-117">Benutzer gesamt fehlgeschlagenen überprüfen ins für die letzten drei Monate angezeigt.</span><span class="sxs-lookup"><span data-stu-id="78368-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78368-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78368-118">Relationships</span></span>
<span data-ttu-id="78368-119">Keine</span><span class="sxs-lookup"><span data-stu-id="78368-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78368-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78368-120">JSON Representation</span></span>
<span data-ttu-id="78368-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78368-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



