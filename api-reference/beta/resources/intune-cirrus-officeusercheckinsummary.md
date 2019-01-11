---
title: Ressourcentyp officeUserCheckinSummary
description: Entität, die Mandanten Einchecken Stats beschreibt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2470b1e531f1b268d6797fe2692baf0031728b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834021"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="be46e-103">Ressourcentyp officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="be46e-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="be46e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be46e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be46e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be46e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be46e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be46e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be46e-107">Entität, die Mandanten Einchecken Stats beschreibt.</span><span class="sxs-lookup"><span data-stu-id="be46e-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="be46e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be46e-108">Properties</span></span>
|<span data-ttu-id="be46e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be46e-109">Property</span></span>|<span data-ttu-id="be46e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="be46e-110">Type</span></span>|<span data-ttu-id="be46e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be46e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be46e-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="be46e-112">succeededUserCount</span></span>|<span data-ttu-id="be46e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="be46e-113">Int32</span></span>|<span data-ttu-id="be46e-114">Gesamtzahl erfolgreicher Benutzer überprüfen ins für die letzten drei Monate angezeigt.</span><span class="sxs-lookup"><span data-stu-id="be46e-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="be46e-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="be46e-115">failedUserCount</span></span>|<span data-ttu-id="be46e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="be46e-116">Int32</span></span>|<span data-ttu-id="be46e-117">Benutzer gesamt fehlgeschlagenen überprüfen ins für die letzten drei Monate angezeigt.</span><span class="sxs-lookup"><span data-stu-id="be46e-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be46e-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="be46e-118">Relationships</span></span>
<span data-ttu-id="be46e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="be46e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be46e-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="be46e-120">JSON Representation</span></span>
<span data-ttu-id="be46e-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="be46e-121">Here is a JSON representation of the resource.</span></span>
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



