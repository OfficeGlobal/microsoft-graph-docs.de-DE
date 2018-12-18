---
title: Ressourcentyp educationSynchronizationCustomization
description: 'Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. '
author: mmast-msft
ms.openlocfilehash: d4f67c9f56198350731c18fe3da8b512522c4d71
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350636"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="e1e37-104">Ressourcentyp educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="e1e37-104">educationSynchronizationCustomization resource type</span></span>

> <span data-ttu-id="e1e37-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e1e37-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1e37-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1e37-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1e37-107">Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit.</span><span class="sxs-lookup"><span data-stu-id="e1e37-107">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="e1e37-108">Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="e1e37-108">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="e1e37-109">**Hinweis:** Die **SynchronizationStartDate** -Eigenschaft gilt nur für die Entität **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="e1e37-109">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="e1e37-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1e37-110">Properties</span></span>

| <span data-ttu-id="e1e37-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1e37-111">Property</span></span> | <span data-ttu-id="e1e37-112">Typ</span><span class="sxs-lookup"><span data-stu-id="e1e37-112">Type</span></span> | <span data-ttu-id="e1e37-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1e37-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e1e37-114">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="e1e37-114">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="e1e37-115">Auflistung der Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1e37-115">collection of string</span></span> |  <span data-ttu-id="e1e37-116">Die Auflistung von Eigenschaftennamen synchronisieren. Wenn auf null festgelegt, alle Eigenschaften werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="e1e37-116">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="e1e37-117">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="e1e37-117">**synchronizationStartDate**</span></span> | <span data-ttu-id="e1e37-118">DateTime</span><span class="sxs-lookup"><span data-stu-id="e1e37-118">DateTime</span></span> |  <span data-ttu-id="e1e37-119">Das Datum, das die Synchronisierung gestartet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e1e37-119">The date that the synchronization should start.</span></span> <span data-ttu-id="e1e37-120">Dieser Wert sollte zu einem späteren Zeitpunkt festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="e1e37-120">This value should be set to a future date.</span></span> <span data-ttu-id="e1e37-121">Wenn der Wert Null, die Ressource synchronisiert werden soll, wenn das Profil Setup abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="e1e37-121">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="e1e37-122">**Hinweis:** Dies gilt nur für die **StudentEnrollment** -Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="e1e37-122">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="e1e37-123">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="e1e37-123">**isSyncDeferred**</span></span> |<span data-ttu-id="e1e37-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="e1e37-124">Boolean</span></span> | <span data-ttu-id="e1e37-125">Gibt an, ob die Synchronisierung der übergeordneten Entität zu einem späteren Zeitpunkt verzögert ist.</span><span class="sxs-lookup"><span data-stu-id="e1e37-125">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="e1e37-126">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="e1e37-126">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="e1e37-127">Boolesch</span><span class="sxs-lookup"><span data-stu-id="e1e37-127">Boolean</span></span> |  <span data-ttu-id="e1e37-128">Gibt an, ob der Anzeigename der Ressource durch die Synchronisierung überschrieben werden kann.</span><span class="sxs-lookup"><span data-stu-id="e1e37-128">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="e1e37-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1e37-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
