---
title: Ressourcentyp outlookTaskFolder
description: 'Ein Ordner mit Outlook-Aufgaben (Auflistung von OutlookTask-Objekten). '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4b4c4bade46022b30c6e4e1f50aae58d32656f0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882929"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="80235-103">Ressourcentyp outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-103">outlookTaskFolder resource type</span></span>

> <span data-ttu-id="80235-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80235-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80235-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80235-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80235-106">Ein Ordner mit Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten).</span><span class="sxs-lookup"><span data-stu-id="80235-106">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="80235-107">In Outlook, der Standardgruppe Aufgabe `My Tasks`, enthält einen Standardordner Aufgabe `Tasks`, für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="80235-107">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="80235-108">Sie umbenennen oder löschen Sie diese Aufgabe Standardgruppe und der Ordner ist nicht möglich, aber Sie können zusätzliche Vorgangsgruppen und Aufgabenordner erstellen.</span><span class="sxs-lookup"><span data-stu-id="80235-108">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="80235-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="80235-109">Methods</span></span>

| <span data-ttu-id="80235-110">Methode</span><span class="sxs-lookup"><span data-stu-id="80235-110">Method</span></span>           | <span data-ttu-id="80235-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="80235-111">Return Type</span></span>    |<span data-ttu-id="80235-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80235-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80235-113">Abrufen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-113">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="80235-114">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-114">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="80235-115">Rufen Sie die Eigenschaften und Beziehungen zwischen den angegebenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="80235-115">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="80235-116">Erstellen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="80235-116">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="80235-117">outlookTask</span><span class="sxs-lookup"><span data-stu-id="80235-117">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="80235-118">Erstellen Sie eine Outlook-Aufgabe im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="80235-118">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="80235-119">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="80235-119">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="80235-120">[OutlookTask](outlooktask.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="80235-120">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="80235-121">Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="80235-121">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="80235-122">Update</span><span class="sxs-lookup"><span data-stu-id="80235-122">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="80235-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="80235-124">Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="80235-124">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="80235-125">Delete</span><span class="sxs-lookup"><span data-stu-id="80235-125">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="80235-126">Keine</span><span class="sxs-lookup"><span data-stu-id="80235-126">None</span></span> |<span data-ttu-id="80235-127">Den angegebenen Outlook den Ordner zu löschen.</span><span class="sxs-lookup"><span data-stu-id="80235-127">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="80235-128">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="80235-128">**Extended properties**</span></span>| | |
|[<span data-ttu-id="80235-129">Create single-value extended property</span><span class="sxs-lookup"><span data-stu-id="80235-129">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="80235-130">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-130">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="80235-131">Erstellen Sie eine oder mehrere einwertig erweiterte Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="80235-131">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="80235-132">Abrufen von Aufgabenordner mit erweiterten Eigenschaft einwertig</span><span class="sxs-lookup"><span data-stu-id="80235-132">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="80235-133">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-133">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="80235-134">Abrufen von Outlook-Aufgabenordner, die einen erweiterte Eigenschaft mithilfe von Single-Wert enthalten `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="80235-134">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="80235-135">Create multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="80235-135">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="80235-136">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-136">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="80235-137">Erstellen Sie eine oder mehrere erweiterte mehrwertige Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="80235-137">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="80235-138">Abrufen von Aufgabenordner mit erweiterten Eigenschaft mit mehreren Werten</span><span class="sxs-lookup"><span data-stu-id="80235-138">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="80235-139">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="80235-139">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="80235-140">Abrufen einer Outlook-Aufgabenordner, die mithilfe eine erweiterte Eigenschaft mit mehreren Werte enthält `$expand`.</span><span class="sxs-lookup"><span data-stu-id="80235-140">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="80235-141">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80235-141">Properties</span></span>
| <span data-ttu-id="80235-142">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80235-142">Property</span></span>     | <span data-ttu-id="80235-143">Typ</span><span class="sxs-lookup"><span data-stu-id="80235-143">Type</span></span>   |<span data-ttu-id="80235-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80235-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80235-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="80235-145">changeKey</span></span>|<span data-ttu-id="80235-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80235-146">String</span></span>|<span data-ttu-id="80235-147">Die Version des den Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="80235-147">The version of the task folder.</span></span>|
|<span data-ttu-id="80235-148">id</span><span class="sxs-lookup"><span data-stu-id="80235-148">id</span></span>|<span data-ttu-id="80235-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80235-149">String</span></span>|<span data-ttu-id="80235-150">Der Bezeichner des den Aufgabenordner, die im Postfach des Benutzers eindeutig.</span><span class="sxs-lookup"><span data-stu-id="80235-150">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="80235-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80235-151">Read-only.</span></span>|
|<span data-ttu-id="80235-152">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="80235-152">isDefaultFolder</span></span>|<span data-ttu-id="80235-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80235-153">Boolean</span></span>|<span data-ttu-id="80235-154">True, wenn der Ordner der Standardordner für die Aufgabe ist.</span><span class="sxs-lookup"><span data-stu-id="80235-154">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="80235-155">name</span><span class="sxs-lookup"><span data-stu-id="80235-155">name</span></span>|<span data-ttu-id="80235-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80235-156">String</span></span>|<span data-ttu-id="80235-157">Der Name des Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="80235-157">The name of the task folder.</span></span>|
|<span data-ttu-id="80235-158">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="80235-158">parentGroupKey</span></span>|<span data-ttu-id="80235-159">Guid</span><span class="sxs-lookup"><span data-stu-id="80235-159">Guid</span></span>|<span data-ttu-id="80235-160">Der eindeutige GUID-Bezeichner für die übergeordnete Gruppe des vorgangsordners.</span><span class="sxs-lookup"><span data-stu-id="80235-160">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80235-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="80235-161">Relationships</span></span>
| <span data-ttu-id="80235-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="80235-162">Relationship</span></span> | <span data-ttu-id="80235-163">Typ</span><span class="sxs-lookup"><span data-stu-id="80235-163">Type</span></span>   |<span data-ttu-id="80235-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80235-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80235-165">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="80235-165">multiValueExtendedProperties</span></span>|<span data-ttu-id="80235-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="80235-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="80235-167">Die Auflistung der Mehrfachwert erweiterte Eigenschaften für den Aufgabenordner definiert.</span><span class="sxs-lookup"><span data-stu-id="80235-167">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="80235-168">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80235-168">Read-only.</span></span> <span data-ttu-id="80235-169">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="80235-169">Nullable.</span></span>|
|<span data-ttu-id="80235-170">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="80235-170">singleValueExtendedProperties</span></span>|<span data-ttu-id="80235-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="80235-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="80235-172">Die Auflistung der einwertig erweiterte Eigenschaften für den Aufgabenordner definiert.</span><span class="sxs-lookup"><span data-stu-id="80235-172">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="80235-173">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80235-173">Read-only.</span></span> <span data-ttu-id="80235-174">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="80235-174">Nullable.</span></span>|
|<span data-ttu-id="80235-175">tasks</span><span class="sxs-lookup"><span data-stu-id="80235-175">tasks</span></span>|<span data-ttu-id="80235-176">[OutlookTask](outlooktask.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="80235-176">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="80235-177">Die Aufgaben in diesem Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="80235-177">The tasks in this task folder.</span></span> <span data-ttu-id="80235-178">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80235-178">Read-only.</span></span> <span data-ttu-id="80235-179">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="80235-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80235-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80235-180">JSON representation</span></span>
<span data-ttu-id="80235-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80235-181">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
