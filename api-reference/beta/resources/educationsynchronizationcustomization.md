---
title: Ressourcentyp educationSynchronizationCustomization
description: 'Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9294af5796daeefb394ed1625a9a36128ae7b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860900"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="17317-104">Ressourcentyp educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="17317-104">educationSynchronizationCustomization resource type</span></span>

> <span data-ttu-id="17317-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="17317-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17317-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17317-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17317-107">Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit.</span><span class="sxs-lookup"><span data-stu-id="17317-107">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="17317-108">Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="17317-108">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="17317-109">**Hinweis:** Die **SynchronizationStartDate** -Eigenschaft gilt nur für die Entität **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="17317-109">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="17317-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17317-110">Properties</span></span>

| <span data-ttu-id="17317-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17317-111">Property</span></span> | <span data-ttu-id="17317-112">Typ</span><span class="sxs-lookup"><span data-stu-id="17317-112">Type</span></span> | <span data-ttu-id="17317-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17317-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="17317-114">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="17317-114">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="17317-115">Auflistung der Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17317-115">collection of string</span></span> |  <span data-ttu-id="17317-116">Die Auflistung von Eigenschaftennamen synchronisieren. Wenn auf null festgelegt, alle Eigenschaften werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="17317-116">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="17317-117">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="17317-117">**synchronizationStartDate**</span></span> | <span data-ttu-id="17317-118">DateTime</span><span class="sxs-lookup"><span data-stu-id="17317-118">DateTime</span></span> |  <span data-ttu-id="17317-119">Das Datum, das die Synchronisierung gestartet werden soll.</span><span class="sxs-lookup"><span data-stu-id="17317-119">The date that the synchronization should start.</span></span> <span data-ttu-id="17317-120">Dieser Wert sollte zu einem späteren Zeitpunkt festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="17317-120">This value should be set to a future date.</span></span> <span data-ttu-id="17317-121">Wenn der Wert Null, die Ressource synchronisiert werden soll, wenn das Profil Setup abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="17317-121">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="17317-122">**Hinweis:** Dies gilt nur für die **StudentEnrollment** -Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="17317-122">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="17317-123">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="17317-123">**isSyncDeferred**</span></span> |<span data-ttu-id="17317-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="17317-124">Boolean</span></span> | <span data-ttu-id="17317-125">Gibt an, ob die Synchronisierung der übergeordneten Entität zu einem späteren Zeitpunkt verzögert ist.</span><span class="sxs-lookup"><span data-stu-id="17317-125">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="17317-126">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="17317-126">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="17317-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="17317-127">Boolean</span></span> |  <span data-ttu-id="17317-128">Gibt an, ob der Anzeigename der Ressource durch die Synchronisierung überschrieben werden kann.</span><span class="sxs-lookup"><span data-stu-id="17317-128">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="17317-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17317-129">JSON representation</span></span>
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
