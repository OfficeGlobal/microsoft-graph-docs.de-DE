---
title: Ressourcentyp synchronizationSchema
description: Definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll. Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag. Sie werden in der Regel anpassen einiger Attribut Zuordnungen oder Hinzufügen eines Gültigkeitsbereichs Filters zum Synchronisieren von nur Objekte, die eine bestimmte Bedingung erfüllen.
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515930"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="c0175-105">Ressourcentyp synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c0175-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0175-106">Definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0175-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="c0175-107">Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag.</span><span class="sxs-lookup"><span data-stu-id="c0175-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="c0175-108">Sie werden in der Regel anpassen einiger [Attribut Zuordnungen](synchronization-attributemapping.md)oder Hinzufügen eines [Gültigkeitsbereichs Filter](synchronization-filter.md) , um nur die Objekte zu synchronisieren, die eine bestimmte Bedingung erfüllen.</span><span class="sxs-lookup"><span data-stu-id="c0175-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="c0175-109">In den folgenden Abschnitten werden die allgemeinen Komponenten des Synchronisierungsschemas beschrieben.</span><span class="sxs-lookup"><span data-stu-id="c0175-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="c0175-110">Directory-Definitionen</span><span class="sxs-lookup"><span data-stu-id="c0175-110">Directory definitions</span></span>

<span data-ttu-id="c0175-111">[Directory-Definitionen](synchronization-directorydefinition.md) finden Sie die Synchronisierung Engine Verzeichnisse und deren Objekte Informationen.</span><span class="sxs-lookup"><span data-stu-id="c0175-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="c0175-112">Die Definition Directory gibt beispielsweise dem Synchronisierungsmodul, dass ein Azure AD-Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="c0175-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="c0175-113">In der Reihenfolge für ein bestimmtes Objekt und das Attribut im Synchronisierung Rules-Objekt Zuordnungen verwendet werden soll müssen sie als Teil der Definition der Directory definiert werden.</span><span class="sxs-lookup"><span data-stu-id="c0175-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="c0175-114">Synchronisierungsregeln</span><span class="sxs-lookup"><span data-stu-id="c0175-114">Synchronization rules</span></span>

<span data-ttu-id="c0175-115">[Synchronisierungsregeln](synchronization-synchronizationrule.md) sind die Kernelemente der Synchronisation Einrichtung.</span><span class="sxs-lookup"><span data-stu-id="c0175-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="c0175-116">Sie definieren für das Synchronisierungsmodul wie die Synchronisierung ausgeführt werden sollen, welche Objekte einschließlich synchronisiert werden soll, wie Objekte aus dem Quellverzeichnis-Objekte in das Zielverzeichnis zugeordnet werden soll, und wie Attribute werden sollen transformiert, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.</span><span class="sxs-lookup"><span data-stu-id="c0175-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="c0175-117">Objekt-Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="c0175-117">Object mappings</span></span>

<span data-ttu-id="c0175-118">[Objekt Zuordnungen](synchronization-objectmapping.md) sind die wichtigsten Teil der Regel Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="c0175-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="c0175-119">Jede objektzuordnung definiert, wie ein bestimmtes Objekt aus der Quelle in das Zielverzeichnis synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c0175-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="c0175-120">Insbesondere die Zuordnung definiert, wie ein Objekt in das Quellverzeichnis mit einem Objekt in das Zielverzeichnis zugeordnet werden sollen was (falls vorhanden) Bereichsdefinierung Filter sollte verwendet werden, um festzulegen, ob ein Objekt bereit, und wie Objektattribute transformiert werden sollten Wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.</span><span class="sxs-lookup"><span data-stu-id="c0175-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="c0175-121">Methoden</span><span class="sxs-lookup"><span data-stu-id="c0175-121">Methods</span></span>

| <span data-ttu-id="c0175-122">Methode</span><span class="sxs-lookup"><span data-stu-id="c0175-122">Method</span></span>        | <span data-ttu-id="c0175-123">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c0175-123">Return Type</span></span>               | <span data-ttu-id="c0175-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0175-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="c0175-125">Get-schema</span><span class="sxs-lookup"><span data-stu-id="c0175-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="c0175-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c0175-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="c0175-127">Lesen Sie Eigenschaften und Beziehungen des **SynchronizationSchema** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c0175-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="c0175-128">Aktualisieren des Schemas</span><span class="sxs-lookup"><span data-stu-id="c0175-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="c0175-129">Keine</span><span class="sxs-lookup"><span data-stu-id="c0175-129">None</span></span>   |<span data-ttu-id="c0175-130">Aktualisieren Sie das Synchronisierungsschema.</span><span class="sxs-lookup"><span data-stu-id="c0175-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="c0175-131">Schema löschen</span><span class="sxs-lookup"><span data-stu-id="c0175-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="c0175-132">Keine</span><span class="sxs-lookup"><span data-stu-id="c0175-132">None</span></span>   |<span data-ttu-id="c0175-133">Löschen Sie das angepasste Schema, das Schema auf die Standardkonfiguration zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="c0175-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="c0175-134">Liste Filteroperatoren</span><span class="sxs-lookup"><span data-stu-id="c0175-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="c0175-135">[FilterOperatorSchema](../resources/synchronization-filteroperatorschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c0175-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="c0175-136">Alle in den Gültigkeitsbereichen Filtern unterstützte Operatoren aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="c0175-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="c0175-137">List-Attribut Zuordnen von Funktionen</span><span class="sxs-lookup"><span data-stu-id="c0175-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="c0175-138">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c0175-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="c0175-139">Listen Sie alle Funktionen, die in das Attribut Zuordnung Ausdrücken unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0175-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="c0175-140">Analysieren von Attribut Zuordnung Ausdruck</span><span class="sxs-lookup"><span data-stu-id="c0175-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="c0175-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="c0175-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="c0175-142">Ein Zeichenfolgenausdruck in einem [AttributeMappingSource analysieren</span><span class="sxs-lookup"><span data-stu-id="c0175-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="c0175-143">(.. / resources/synchronization_attributemappingsource.md) Objekt.</span><span class="sxs-lookup"><span data-stu-id="c0175-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="c0175-144">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0175-144">Properties</span></span>

| <span data-ttu-id="c0175-145">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0175-145">Property</span></span>      | <span data-ttu-id="c0175-146">Typ</span><span class="sxs-lookup"><span data-stu-id="c0175-146">Type</span></span>      | <span data-ttu-id="c0175-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0175-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c0175-148">directories</span><span class="sxs-lookup"><span data-stu-id="c0175-148">directories</span></span>            |<span data-ttu-id="c0175-149">[DirectoryDefinition](synchronization-directorydefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c0175-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="c0175-150">Beschreibt Verzeichnisse und Objekte, die Teil der [SynchronizationJob](synchronization-synchronizationjob.md) oder [SynchronisationVorlage](synchronization-synchronizationtemplate.md)sind.</span><span class="sxs-lookup"><span data-stu-id="c0175-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="c0175-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="c0175-151">synchronizationRules</span></span>   |<span data-ttu-id="c0175-152">[SynchronizationRule](synchronization-synchronizationrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c0175-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="c0175-153">Eine Auflistung von Regeln für die [SynchronizationJob](synchronization-synchronizationjob.md) oder [SynchronisationVorlage](synchronization-synchronizationtemplate.md)konfiguriert sind,</span><span class="sxs-lookup"><span data-stu-id="c0175-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="c0175-154">Version</span><span class="sxs-lookup"><span data-stu-id="c0175-154">version</span></span>                |<span data-ttu-id="c0175-155">String</span><span class="sxs-lookup"><span data-stu-id="c0175-155">String</span></span>                             |<span data-ttu-id="c0175-156">Die Version des Schemas, bei jeder Änderung Schema automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c0175-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c0175-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0175-157">JSON representation</span></span>

<span data-ttu-id="c0175-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c0175-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
