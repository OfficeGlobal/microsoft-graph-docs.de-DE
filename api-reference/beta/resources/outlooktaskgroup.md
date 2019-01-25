---
title: Ressourcentyp outlookTaskGroup
description: 'Eine Gruppe von Ordnern (OutlookTaskFolder), die Outlook-Aufgaben (Auflistung von OutlookTask-Objekten) enthalten. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524618"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="0f0cb-103">Ressourcentyp outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="0f0cb-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f0cb-104">Eine Gruppe von Ordnern ([OutlookTaskFolder](outlooktaskfolder.md)), die Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten) enthalten.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="0f0cb-105">In Outlook eine Aufgabe Standardgruppe vorhanden ist `My Tasks` das Umbenennen oder löschen können.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="0f0cb-106">Sie können jedoch zusätzliche Vorgangsgruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="0f0cb-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="0f0cb-107">Methods</span></span>

| <span data-ttu-id="0f0cb-108">Methode</span><span class="sxs-lookup"><span data-stu-id="0f0cb-108">Method</span></span>           | <span data-ttu-id="0f0cb-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0f0cb-109">Return Type</span></span>    |<span data-ttu-id="0f0cb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f0cb-111">Abrufen von outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="0f0cb-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="0f0cb-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="0f0cb-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="0f0cb-113">Rufen Sie die Eigenschaften und Beziehungen zwischen der angegebenen Gruppe der Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="0f0cb-114">Erstellen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="0f0cb-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="0f0cb-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="0f0cb-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="0f0cb-116">Erstellen eines Outlook-Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="0f0cb-117">Liste taskFolders</span><span class="sxs-lookup"><span data-stu-id="0f0cb-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="0f0cb-118">[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="0f0cb-119">Rufen Sie eine Auflistung von Outlook Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="0f0cb-120">Update</span><span class="sxs-lookup"><span data-stu-id="0f0cb-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="0f0cb-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="0f0cb-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="0f0cb-122">Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="0f0cb-123">Delete</span><span class="sxs-lookup"><span data-stu-id="0f0cb-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="0f0cb-124">Keine</span><span class="sxs-lookup"><span data-stu-id="0f0cb-124">None</span></span> |<span data-ttu-id="0f0cb-125">Löschen der angegebenen Gruppe der Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f0cb-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f0cb-126">Properties</span></span>
| <span data-ttu-id="0f0cb-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f0cb-127">Property</span></span>     | <span data-ttu-id="0f0cb-128">Typ</span><span class="sxs-lookup"><span data-stu-id="0f0cb-128">Type</span></span>   |<span data-ttu-id="0f0cb-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f0cb-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="0f0cb-130">changeKey</span></span>|<span data-ttu-id="0f0cb-131">String</span><span class="sxs-lookup"><span data-stu-id="0f0cb-131">String</span></span>|<span data-ttu-id="0f0cb-132">Die Version der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-132">The version of the task group.</span></span>|
|<span data-ttu-id="0f0cb-133">groupKey</span><span class="sxs-lookup"><span data-stu-id="0f0cb-133">groupKey</span></span>|<span data-ttu-id="0f0cb-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="0f0cb-134">Edm.Guid</span></span>|<span data-ttu-id="0f0cb-135">Der eindeutige GUID-Bezeichner für die Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="0f0cb-136">id</span><span class="sxs-lookup"><span data-stu-id="0f0cb-136">id</span></span>|<span data-ttu-id="0f0cb-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f0cb-137">String</span></span>|<span data-ttu-id="0f0cb-138">Der eindeutige Zeichenfolgenbezeichner der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="0f0cb-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-139">Read-only.</span></span>|
|<span data-ttu-id="0f0cb-140">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="0f0cb-140">isDefaultGroup</span></span>|<span data-ttu-id="0f0cb-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0f0cb-141">Boolean</span></span>|<span data-ttu-id="0f0cb-142">True, wenn die "Task Group" der Standardproxygruppe für die Aufgabe ist.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="0f0cb-143">name</span><span class="sxs-lookup"><span data-stu-id="0f0cb-143">name</span></span>|<span data-ttu-id="0f0cb-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f0cb-144">String</span></span>|<span data-ttu-id="0f0cb-145">Der Name der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f0cb-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f0cb-146">Relationships</span></span>
| <span data-ttu-id="0f0cb-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-147">Relationship</span></span> | <span data-ttu-id="0f0cb-148">Typ</span><span class="sxs-lookup"><span data-stu-id="0f0cb-148">Type</span></span>   |<span data-ttu-id="0f0cb-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f0cb-150">taskFolders</span><span class="sxs-lookup"><span data-stu-id="0f0cb-150">taskFolders</span></span>|<span data-ttu-id="0f0cb-151">[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="0f0cb-152">Die Auflistung von Task-Ordner in der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="0f0cb-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-153">Read-only.</span></span> <span data-ttu-id="0f0cb-154">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f0cb-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f0cb-155">JSON representation</span></span>
<span data-ttu-id="0f0cb-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f0cb-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
