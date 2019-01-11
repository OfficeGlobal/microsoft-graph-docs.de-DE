---
title: Ressourcentyp outlookTaskGroup
description: 'Eine Gruppe von Ordnern (OutlookTaskFolder), die Outlook-Aufgaben (Auflistung von OutlookTask-Objekten) enthalten. '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5e885c4c8cc2abe4b3890635e010d495267dc877
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878771"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="8993e-103">Ressourcentyp outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="8993e-103">outlookTaskGroup resource type</span></span>

> <span data-ttu-id="8993e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8993e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8993e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8993e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8993e-106">Eine Gruppe von Ordnern ([OutlookTaskFolder](outlooktaskfolder.md)), die Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten) enthalten.</span><span class="sxs-lookup"><span data-stu-id="8993e-106">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="8993e-107">In Outlook eine Aufgabe Standardgruppe vorhanden ist `My Tasks` das Umbenennen oder löschen können.</span><span class="sxs-lookup"><span data-stu-id="8993e-107">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="8993e-108">Sie können jedoch zusätzliche Vorgangsgruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="8993e-108">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="8993e-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="8993e-109">Methods</span></span>

| <span data-ttu-id="8993e-110">Methode</span><span class="sxs-lookup"><span data-stu-id="8993e-110">Method</span></span>           | <span data-ttu-id="8993e-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8993e-111">Return Type</span></span>    |<span data-ttu-id="8993e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8993e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8993e-113">Abrufen von outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="8993e-113">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="8993e-114">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="8993e-114">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="8993e-115">Rufen Sie die Eigenschaften und Beziehungen zwischen der angegebenen Gruppe der Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="8993e-115">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="8993e-116">Erstellen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8993e-116">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="8993e-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8993e-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="8993e-118">Erstellen eines Outlook-Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="8993e-118">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="8993e-119">Liste taskFolders</span><span class="sxs-lookup"><span data-stu-id="8993e-119">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="8993e-120">[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8993e-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="8993e-121">Rufen Sie eine Auflistung von Outlook Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="8993e-121">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="8993e-122">Update</span><span class="sxs-lookup"><span data-stu-id="8993e-122">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="8993e-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="8993e-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="8993e-124">Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="8993e-124">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="8993e-125">Delete</span><span class="sxs-lookup"><span data-stu-id="8993e-125">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="8993e-126">Keine</span><span class="sxs-lookup"><span data-stu-id="8993e-126">None</span></span> |<span data-ttu-id="8993e-127">Löschen der angegebenen Gruppe der Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="8993e-127">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="8993e-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8993e-128">Properties</span></span>
| <span data-ttu-id="8993e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8993e-129">Property</span></span>     | <span data-ttu-id="8993e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8993e-130">Type</span></span>   |<span data-ttu-id="8993e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8993e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8993e-132">changeKey</span><span class="sxs-lookup"><span data-stu-id="8993e-132">changeKey</span></span>|<span data-ttu-id="8993e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8993e-133">String</span></span>|<span data-ttu-id="8993e-134">Die Version der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="8993e-134">The version of the task group.</span></span>|
|<span data-ttu-id="8993e-135">groupKey</span><span class="sxs-lookup"><span data-stu-id="8993e-135">groupKey</span></span>|<span data-ttu-id="8993e-136">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="8993e-136">Edm.Guid</span></span>|<span data-ttu-id="8993e-137">Der eindeutige GUID-Bezeichner für die Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="8993e-137">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="8993e-138">id</span><span class="sxs-lookup"><span data-stu-id="8993e-138">id</span></span>|<span data-ttu-id="8993e-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8993e-139">String</span></span>|<span data-ttu-id="8993e-140">Der eindeutige Zeichenfolgenbezeichner der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="8993e-140">The unique string identifier of the task group.</span></span> <span data-ttu-id="8993e-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8993e-141">Read-only.</span></span>|
|<span data-ttu-id="8993e-142">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="8993e-142">isDefaultGroup</span></span>|<span data-ttu-id="8993e-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8993e-143">Boolean</span></span>|<span data-ttu-id="8993e-144">True, wenn die "Task Group" der Standardproxygruppe für die Aufgabe ist.</span><span class="sxs-lookup"><span data-stu-id="8993e-144">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="8993e-145">name</span><span class="sxs-lookup"><span data-stu-id="8993e-145">name</span></span>|<span data-ttu-id="8993e-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8993e-146">String</span></span>|<span data-ttu-id="8993e-147">Der Name der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="8993e-147">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8993e-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8993e-148">Relationships</span></span>
| <span data-ttu-id="8993e-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8993e-149">Relationship</span></span> | <span data-ttu-id="8993e-150">Typ</span><span class="sxs-lookup"><span data-stu-id="8993e-150">Type</span></span>   |<span data-ttu-id="8993e-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8993e-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8993e-152">taskFolders</span><span class="sxs-lookup"><span data-stu-id="8993e-152">taskFolders</span></span>|<span data-ttu-id="8993e-153">[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8993e-153">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="8993e-154">Die Auflistung von Task-Ordner in der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="8993e-154">The collection of task folders in the task group.</span></span> <span data-ttu-id="8993e-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8993e-155">Read-only.</span></span> <span data-ttu-id="8993e-156">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8993e-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8993e-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8993e-157">JSON representation</span></span>
<span data-ttu-id="8993e-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8993e-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
