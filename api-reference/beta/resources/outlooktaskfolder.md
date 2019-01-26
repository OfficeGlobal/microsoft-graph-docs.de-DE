---
title: Ressourcentyp outlookTaskFolder
description: 'Ein Ordner mit Outlook-Aufgaben (Auflistung von OutlookTask-Objekten). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a117e14ea1cfe4b69cbbf69720a22a0094fb0b72
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575667"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="52991-103">Ressourcentyp outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52991-104">Ein Ordner mit Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten).</span><span class="sxs-lookup"><span data-stu-id="52991-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="52991-105">In Outlook, der Standardgruppe Aufgabe `My Tasks`, enthält einen Standardordner Aufgabe `Tasks`, für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="52991-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="52991-106">Sie umbenennen oder löschen Sie diese Aufgabe Standardgruppe und der Ordner ist nicht möglich, aber Sie können zusätzliche Vorgangsgruppen und Aufgabenordner erstellen.</span><span class="sxs-lookup"><span data-stu-id="52991-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="52991-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="52991-107">Methods</span></span>

| <span data-ttu-id="52991-108">Methode</span><span class="sxs-lookup"><span data-stu-id="52991-108">Method</span></span>           | <span data-ttu-id="52991-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="52991-109">Return Type</span></span>    |<span data-ttu-id="52991-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52991-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52991-111">Abrufen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="52991-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="52991-113">Rufen Sie die Eigenschaften und Beziehungen zwischen den angegebenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="52991-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="52991-114">Erstellen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="52991-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="52991-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="52991-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="52991-116">Erstellen Sie eine Outlook-Aufgabe im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="52991-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="52991-117">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="52991-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="52991-118">[OutlookTask](outlooktask.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="52991-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="52991-119">Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="52991-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="52991-120">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="52991-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="52991-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="52991-122">Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="52991-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="52991-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="52991-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="52991-124">Keine</span><span class="sxs-lookup"><span data-stu-id="52991-124">None</span></span> |<span data-ttu-id="52991-125">Den angegebenen Outlook den Ordner zu löschen.</span><span class="sxs-lookup"><span data-stu-id="52991-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="52991-126">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="52991-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="52991-127">Einwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="52991-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="52991-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="52991-129">Erstellen Sie eine oder mehrere einwertig erweiterte Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="52991-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="52991-130">Abrufen von Aufgabenordner mit erweiterten Eigenschaft einwertig</span><span class="sxs-lookup"><span data-stu-id="52991-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="52991-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="52991-132">Abrufen von Outlook-Aufgabenordner, die einen erweiterte Eigenschaft mithilfe von Single-Wert enthalten `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="52991-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="52991-133">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="52991-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="52991-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="52991-135">Erstellen Sie eine oder mehrere erweiterte mehrwertige Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="52991-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="52991-136">Abrufen von Aufgabenordner mit erweiterten Eigenschaft mit mehreren Werten</span><span class="sxs-lookup"><span data-stu-id="52991-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="52991-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52991-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="52991-138">Abrufen einer Outlook-Aufgabenordner, die mithilfe eine erweiterte Eigenschaft mit mehreren Werte enthält `$expand`.</span><span class="sxs-lookup"><span data-stu-id="52991-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="52991-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="52991-139">Properties</span></span>
| <span data-ttu-id="52991-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52991-140">Property</span></span>     | <span data-ttu-id="52991-141">Typ</span><span class="sxs-lookup"><span data-stu-id="52991-141">Type</span></span>   |<span data-ttu-id="52991-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52991-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52991-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="52991-143">changeKey</span></span>|<span data-ttu-id="52991-144">String</span><span class="sxs-lookup"><span data-stu-id="52991-144">String</span></span>|<span data-ttu-id="52991-145">Die Version des den Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="52991-145">The version of the task folder.</span></span>|
|<span data-ttu-id="52991-146">id</span><span class="sxs-lookup"><span data-stu-id="52991-146">id</span></span>|<span data-ttu-id="52991-147">String</span><span class="sxs-lookup"><span data-stu-id="52991-147">String</span></span>|<span data-ttu-id="52991-148">Der Bezeichner des den Aufgabenordner, die im Postfach des Benutzers eindeutig.</span><span class="sxs-lookup"><span data-stu-id="52991-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="52991-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52991-149">Read-only.</span></span>|
|<span data-ttu-id="52991-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="52991-150">isDefaultFolder</span></span>|<span data-ttu-id="52991-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="52991-151">Boolean</span></span>|<span data-ttu-id="52991-152">True, wenn der Ordner der Standardordner für die Aufgabe ist.</span><span class="sxs-lookup"><span data-stu-id="52991-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="52991-153">name</span><span class="sxs-lookup"><span data-stu-id="52991-153">name</span></span>|<span data-ttu-id="52991-154">String</span><span class="sxs-lookup"><span data-stu-id="52991-154">String</span></span>|<span data-ttu-id="52991-155">Der Name des Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="52991-155">The name of the task folder.</span></span>|
|<span data-ttu-id="52991-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="52991-156">parentGroupKey</span></span>|<span data-ttu-id="52991-157">Guid</span><span class="sxs-lookup"><span data-stu-id="52991-157">Guid</span></span>|<span data-ttu-id="52991-158">Der eindeutige GUID-Bezeichner für die übergeordnete Gruppe des vorgangsordners.</span><span class="sxs-lookup"><span data-stu-id="52991-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52991-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="52991-159">Relationships</span></span>
| <span data-ttu-id="52991-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="52991-160">Relationship</span></span> | <span data-ttu-id="52991-161">Typ</span><span class="sxs-lookup"><span data-stu-id="52991-161">Type</span></span>   |<span data-ttu-id="52991-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52991-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52991-163">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="52991-163">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="52991-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="52991-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="52991-165">Die Auflistung der Mehrfachwert erweiterte Eigenschaften für den Aufgabenordner definiert.</span><span class="sxs-lookup"><span data-stu-id="52991-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="52991-166">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52991-166">Read-only.</span></span> <span data-ttu-id="52991-167">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="52991-167">Nullable.</span></span>|
|<span data-ttu-id="52991-168">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="52991-168">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="52991-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="52991-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="52991-170">Die Auflistung der einwertig erweiterte Eigenschaften für den Aufgabenordner definiert.</span><span class="sxs-lookup"><span data-stu-id="52991-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="52991-171">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52991-171">Read-only.</span></span> <span data-ttu-id="52991-172">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="52991-172">Nullable.</span></span>|
|<span data-ttu-id="52991-173">tasks</span><span class="sxs-lookup"><span data-stu-id="52991-173">tasks</span></span>|<span data-ttu-id="52991-174">[OutlookTask](outlooktask.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="52991-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="52991-175">Die Aufgaben in diesem Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="52991-175">The tasks in this task folder.</span></span> <span data-ttu-id="52991-176">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52991-176">Read-only.</span></span> <span data-ttu-id="52991-177">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="52991-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52991-178">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="52991-178">JSON representation</span></span>
<span data-ttu-id="52991-179">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="52991-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty",
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
