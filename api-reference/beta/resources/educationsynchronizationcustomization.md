---
title: Ressourcentyp educationSynchronizationCustomization
description: 'Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513606"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="654d0-104">Ressourcentyp educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="654d0-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="654d0-105">Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit.</span><span class="sxs-lookup"><span data-stu-id="654d0-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="654d0-106">Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="654d0-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="654d0-107">**Hinweis:** Die **SynchronizationStartDate** -Eigenschaft gilt nur für die Entität **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="654d0-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="654d0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="654d0-108">Properties</span></span>

| <span data-ttu-id="654d0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="654d0-109">Property</span></span> | <span data-ttu-id="654d0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="654d0-110">Type</span></span> | <span data-ttu-id="654d0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="654d0-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="654d0-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="654d0-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="654d0-113">Collection of String
</span><span class="sxs-lookup"><span data-stu-id="654d0-113">collection of string</span></span> |  <span data-ttu-id="654d0-114">Die Auflistung von Eigenschaftennamen synchronisieren. Wenn auf null festgelegt, alle Eigenschaften werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="654d0-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="654d0-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="654d0-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="654d0-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="654d0-116">DateTime</span></span> |  <span data-ttu-id="654d0-117">Das Datum, das die Synchronisierung gestartet werden soll.</span><span class="sxs-lookup"><span data-stu-id="654d0-117">The date that the synchronization should start.</span></span> <span data-ttu-id="654d0-118">Dieser Wert sollte zu einem späteren Zeitpunkt festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="654d0-118">This value should be set to a future date.</span></span> <span data-ttu-id="654d0-119">Wenn der Wert Null, die Ressource synchronisiert werden soll, wenn das Profil Setup abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="654d0-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="654d0-120">**Hinweis:** Dies gilt nur für die **StudentEnrollment** -Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="654d0-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="654d0-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="654d0-121">**isSyncDeferred**</span></span> |<span data-ttu-id="654d0-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="654d0-122">Boolean</span></span> | <span data-ttu-id="654d0-123">Gibt an, ob die Synchronisierung der übergeordneten Entität zu einem späteren Zeitpunkt verzögert ist.</span><span class="sxs-lookup"><span data-stu-id="654d0-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="654d0-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="654d0-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="654d0-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="654d0-125">Boolean</span></span> |  <span data-ttu-id="654d0-126">Gibt an, ob der Anzeigename der Ressource durch die Synchronisierung überschrieben werden kann.</span><span class="sxs-lookup"><span data-stu-id="654d0-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="654d0-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="654d0-127">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
