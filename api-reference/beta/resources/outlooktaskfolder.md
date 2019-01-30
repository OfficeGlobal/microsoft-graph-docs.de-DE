---
title: Ressourcentyp outlookTaskFolder
description: 'Ein Ordner mit Outlook-Aufgaben (Auflistung von OutlookTask-Objekten). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643923"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="e06f0-103">Ressourcentyp outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e06f0-104">Ein Ordner mit Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten).</span><span class="sxs-lookup"><span data-stu-id="e06f0-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="e06f0-105">In Outlook, der Standardgruppe Aufgabe `My Tasks`, enthält einen Standardordner Aufgabe `Tasks`, für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e06f0-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="e06f0-106">Sie umbenennen oder löschen Sie diese Aufgabe Standardgruppe und der Ordner ist nicht möglich, aber Sie können zusätzliche Vorgangsgruppen und Aufgabenordner erstellen.</span><span class="sxs-lookup"><span data-stu-id="e06f0-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="e06f0-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="e06f0-107">Methods</span></span>

| <span data-ttu-id="e06f0-108">Methode</span><span class="sxs-lookup"><span data-stu-id="e06f0-108">Method</span></span>           | <span data-ttu-id="e06f0-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e06f0-109">Return Type</span></span>    |<span data-ttu-id="e06f0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e06f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e06f0-111">Abrufen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="e06f0-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="e06f0-113">Rufen Sie die Eigenschaften und Beziehungen zwischen den angegebenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="e06f0-114">Erstellen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="e06f0-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="e06f0-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e06f0-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="e06f0-116">Erstellen Sie eine Outlook-Aufgabe im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="e06f0-117">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="e06f0-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="e06f0-118">[outlookTask](outlooktask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e06f0-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="e06f0-119">Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="e06f0-120">Update</span><span class="sxs-lookup"><span data-stu-id="e06f0-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="e06f0-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="e06f0-122">Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="e06f0-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="e06f0-123">Delete</span><span class="sxs-lookup"><span data-stu-id="e06f0-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="e06f0-124">Keine</span><span class="sxs-lookup"><span data-stu-id="e06f0-124">None</span></span> |<span data-ttu-id="e06f0-125">Den angegebenen Outlook den Ordner zu löschen.</span><span class="sxs-lookup"><span data-stu-id="e06f0-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="e06f0-126">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="e06f0-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="e06f0-127">Create single-value extended property</span><span class="sxs-lookup"><span data-stu-id="e06f0-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="e06f0-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="e06f0-129">Erstellen Sie eine oder mehrere einwertig erweiterte Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="e06f0-130">Abrufen von Aufgabenordner mit erweiterten Eigenschaft einwertig</span><span class="sxs-lookup"><span data-stu-id="e06f0-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e06f0-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="e06f0-132">Abrufen von Outlook-Aufgabenordner, die einen erweiterte Eigenschaft mithilfe von Single-Wert enthalten `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e06f0-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e06f0-133">Create multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="e06f0-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="e06f0-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="e06f0-135">Erstellen Sie eine oder mehrere erweiterte mehrwertige Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="e06f0-136">Abrufen von Aufgabenordner mit erweiterten Eigenschaft mit mehreren Werten</span><span class="sxs-lookup"><span data-stu-id="e06f0-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e06f0-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="e06f0-138">Abrufen einer Outlook-Aufgabenordner, die mithilfe eine erweiterte Eigenschaft mit mehreren Werte enthält `$expand`.</span><span class="sxs-lookup"><span data-stu-id="e06f0-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e06f0-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e06f0-139">Properties</span></span>
| <span data-ttu-id="e06f0-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e06f0-140">Property</span></span>     | <span data-ttu-id="e06f0-141">Typ</span><span class="sxs-lookup"><span data-stu-id="e06f0-141">Type</span></span>   |<span data-ttu-id="e06f0-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e06f0-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e06f0-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="e06f0-143">changeKey</span></span>|<span data-ttu-id="e06f0-144">String</span><span class="sxs-lookup"><span data-stu-id="e06f0-144">String</span></span>|<span data-ttu-id="e06f0-145">Die Version des den Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-145">The version of the task folder.</span></span>|
|<span data-ttu-id="e06f0-146">id</span><span class="sxs-lookup"><span data-stu-id="e06f0-146">id</span></span>|<span data-ttu-id="e06f0-147">String</span><span class="sxs-lookup"><span data-stu-id="e06f0-147">String</span></span>|<span data-ttu-id="e06f0-148">Der Bezeichner des den Aufgabenordner, die im Postfach des Benutzers eindeutig.</span><span class="sxs-lookup"><span data-stu-id="e06f0-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="e06f0-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e06f0-149">Read-only.</span></span>|
|<span data-ttu-id="e06f0-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="e06f0-150">isDefaultFolder</span></span>|<span data-ttu-id="e06f0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="e06f0-151">Boolean</span></span>|<span data-ttu-id="e06f0-152">True, wenn der Ordner der Standardordner für die Aufgabe ist.</span><span class="sxs-lookup"><span data-stu-id="e06f0-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="e06f0-153">name</span><span class="sxs-lookup"><span data-stu-id="e06f0-153">name</span></span>|<span data-ttu-id="e06f0-154">String</span><span class="sxs-lookup"><span data-stu-id="e06f0-154">String</span></span>|<span data-ttu-id="e06f0-155">Der Name des Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="e06f0-155">The name of the task folder.</span></span>|
|<span data-ttu-id="e06f0-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="e06f0-156">parentGroupKey</span></span>|<span data-ttu-id="e06f0-157">Guid</span><span class="sxs-lookup"><span data-stu-id="e06f0-157">Guid</span></span>|<span data-ttu-id="e06f0-158">Der eindeutige GUID-Bezeichner für die übergeordnete Gruppe des vorgangsordners.</span><span class="sxs-lookup"><span data-stu-id="e06f0-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e06f0-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e06f0-159">Relationships</span></span>
| <span data-ttu-id="e06f0-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e06f0-160">Relationship</span></span> | <span data-ttu-id="e06f0-161">Typ</span><span class="sxs-lookup"><span data-stu-id="e06f0-161">Type</span></span>   |<span data-ttu-id="e06f0-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e06f0-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e06f0-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e06f0-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="e06f0-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e06f0-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="e06f0-165">Die Auflistung der Mehrfachwert erweiterte Eigenschaften für den Aufgabenordner definiert.</span><span class="sxs-lookup"><span data-stu-id="e06f0-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="e06f0-166">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e06f0-166">Read-only.</span></span> <span data-ttu-id="e06f0-167">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="e06f0-167">Nullable.</span></span>|
|<span data-ttu-id="e06f0-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e06f0-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="e06f0-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e06f0-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="e06f0-170">Die Auflistung der einwertig erweiterte Eigenschaften für den Aufgabenordner definiert.</span><span class="sxs-lookup"><span data-stu-id="e06f0-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="e06f0-171">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e06f0-171">Read-only.</span></span> <span data-ttu-id="e06f0-172">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e06f0-172">Nullable.</span></span>|
|<span data-ttu-id="e06f0-173">tasks</span><span class="sxs-lookup"><span data-stu-id="e06f0-173">tasks</span></span>|<span data-ttu-id="e06f0-174">[outlookTask](outlooktask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e06f0-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="e06f0-175">Die Aufgaben in diesem Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="e06f0-175">The tasks in this task folder.</span></span> <span data-ttu-id="e06f0-176">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e06f0-176">Read-only.</span></span> <span data-ttu-id="e06f0-177">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e06f0-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e06f0-178">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e06f0-178">JSON representation</span></span>
<span data-ttu-id="e06f0-179">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e06f0-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
