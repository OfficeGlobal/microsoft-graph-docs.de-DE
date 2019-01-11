---
title: Ressourcentyp signInStatus
description: Stellt die Anmeldestatus (Erfolg oder Fehler) von der Anmeldung
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878638"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="b0730-103">Ressourcentyp signInStatus</span><span class="sxs-lookup"><span data-stu-id="b0730-103">signInStatus resource type</span></span>
<span data-ttu-id="b0730-104">Stellt die Anmeldestatus (Erfolg oder Fehler) von der Anmeldung</span><span class="sxs-lookup"><span data-stu-id="b0730-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="b0730-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b0730-105">Properties</span></span>
| <span data-ttu-id="b0730-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0730-106">Property</span></span>     | <span data-ttu-id="b0730-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b0730-107">Type</span></span>   |<span data-ttu-id="b0730-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0730-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0730-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="b0730-109">additionalDetails</span></span>|<span data-ttu-id="b0730-110">String</span><span class="sxs-lookup"><span data-stu-id="b0730-110">String</span></span>|<span data-ttu-id="b0730-111">Bietet zusätzliche Details für die Aktivität-Anmeldung</span><span class="sxs-lookup"><span data-stu-id="b0730-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="b0730-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="b0730-112">errorCode</span></span>|<span data-ttu-id="b0730-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b0730-113">Int32</span></span>|<span data-ttu-id="b0730-114">Enthält den 5 6digit Fehlercode, der bei einem Ausfall-Anmeldung generiert wird.</span><span class="sxs-lookup"><span data-stu-id="b0730-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="b0730-115">Checken Sie die [Liste der Fehlercodes und Nachrichten](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="b0730-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="b0730-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="b0730-116">failureReason</span></span>|<span data-ttu-id="b0730-117">String</span><span class="sxs-lookup"><span data-stu-id="b0730-117">String</span></span>|<span data-ttu-id="b0730-118">Enthält die Fehlermeldung oder der Fehlerursache für die entsprechende Aktivität-Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="b0730-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="b0730-119">Checken Sie die [Liste der Fehlercodes und Nachrichten](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="b0730-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0730-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b0730-120">JSON representation</span></span>

<span data-ttu-id="b0730-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b0730-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
