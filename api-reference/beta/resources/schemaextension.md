---
title: schemaExtension-Ressourcentyp (Schemaerweiterungen)
description: 'Mithilfe von Schemaerweiterungen können Sie ein Schema definieren, um stark typisierte benutzerdefinierte Daten zu erweitern und einem Ressourcentyp hinzuzufügen. Die benutzerdefinierten Daten werden in der erweiterten Ressource als komplexer Typ angezeigt. '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 90acbfb0e7a6b031303ae3286f1a5ed366a2a8c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523855"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="6d3cc-104">schemaExtension-Ressourcentyp (Schemaerweiterungen)</span><span class="sxs-lookup"><span data-stu-id="6d3cc-104">schemaExtension resource type (schema extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d3cc-p102">Mithilfe von Schemaerweiterungen können Sie ein Schema definieren, um stark typisierte benutzerdefinierte Daten zu erweitern und einem Ressourcentyp hinzuzufügen. Die benutzerdefinierten Daten werden in der erweiterten Ressource als komplexer Typ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="6d3cc-107">Schemaerweiterungen werden von den folgenden Ressourcentypen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="6d3cc-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="6d3cc-108">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="6d3cc-108">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="6d3cc-109">contact</span><span class="sxs-lookup"><span data-stu-id="6d3cc-109">contact</span></span>](contact.md)
 - [<span data-ttu-id="6d3cc-110">device</span><span class="sxs-lookup"><span data-stu-id="6d3cc-110">device</span></span>](device.md)
 - <span data-ttu-id="6d3cc-111">[event](event.md) in einem Benutzer oder Office 365-Gruppenkalender</span><span class="sxs-lookup"><span data-stu-id="6d3cc-111">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="6d3cc-112">[post](post.md) einer Office 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="6d3cc-112">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="6d3cc-113">group</span><span class="sxs-lookup"><span data-stu-id="6d3cc-113">group</span></span>](group.md)
 - [<span data-ttu-id="6d3cc-114">message</span><span class="sxs-lookup"><span data-stu-id="6d3cc-114">message</span></span>](message.md) 
 - [<span data-ttu-id="6d3cc-115">organization</span><span class="sxs-lookup"><span data-stu-id="6d3cc-115">organization</span></span>](organization.md)
 - [<span data-ttu-id="6d3cc-116">user</span><span class="sxs-lookup"><span data-stu-id="6d3cc-116">user</span></span>](user.md)

<span data-ttu-id="6d3cc-117">Im [Beispiel für Schemaerweiterungen](/graph/extensibility-schema-groups) erfahren Sie, wie Sie benutzerdefinierte Daten zu Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="6d3cc-118">Methoden</span><span class="sxs-lookup"><span data-stu-id="6d3cc-118">Methods</span></span>

| <span data-ttu-id="6d3cc-119">Methode</span><span class="sxs-lookup"><span data-stu-id="6d3cc-119">Method</span></span>           | <span data-ttu-id="6d3cc-120">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6d3cc-120">Return Type</span></span>    |<span data-ttu-id="6d3cc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d3cc-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d3cc-122">Create</span><span class="sxs-lookup"><span data-stu-id="6d3cc-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="6d3cc-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="6d3cc-123">schemaExtension</span></span> |<span data-ttu-id="6d3cc-124">Dient zum Erstellen einer Schemaerweiterungsdefinition.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="6d3cc-125">List</span><span class="sxs-lookup"><span data-stu-id="6d3cc-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="6d3cc-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="6d3cc-126">schemaExtension</span></span> |<span data-ttu-id="6d3cc-127">Auflisten der Avaialbe SchemaExtension Definitionen und deren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-127">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="6d3cc-128">Get</span><span class="sxs-lookup"><span data-stu-id="6d3cc-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="6d3cc-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="6d3cc-129">schemaExtension</span></span> |<span data-ttu-id="6d3cc-130">Dient zum Lesen der Eigenschaften einer bestimmten schemaExtension-Definition.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="6d3cc-131">Update</span><span class="sxs-lookup"><span data-stu-id="6d3cc-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="6d3cc-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="6d3cc-132">schemaExtension</span></span>   |<span data-ttu-id="6d3cc-133">Dient zum Aktualisieren einer schemaExtension-Definition.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="6d3cc-134">Delete</span><span class="sxs-lookup"><span data-stu-id="6d3cc-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="6d3cc-135">Keine</span><span class="sxs-lookup"><span data-stu-id="6d3cc-135">None</span></span> |<span data-ttu-id="6d3cc-136">Dient zum Löschen einer schemaExtension-Definition.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="6d3cc-137">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d3cc-137">Properties</span></span>
| <span data-ttu-id="6d3cc-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d3cc-138">Property</span></span>     | <span data-ttu-id="6d3cc-139">Typ</span><span class="sxs-lookup"><span data-stu-id="6d3cc-139">Type</span></span>   |<span data-ttu-id="6d3cc-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d3cc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d3cc-141">description</span><span class="sxs-lookup"><span data-stu-id="6d3cc-141">description</span></span>|<span data-ttu-id="6d3cc-142">String</span><span class="sxs-lookup"><span data-stu-id="6d3cc-142">String</span></span>|<span data-ttu-id="6d3cc-143">Beschreibung für die Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="6d3cc-144">id</span><span class="sxs-lookup"><span data-stu-id="6d3cc-144">id</span></span>|<span data-ttu-id="6d3cc-145">String</span><span class="sxs-lookup"><span data-stu-id="6d3cc-145">String</span></span>|<span data-ttu-id="6d3cc-146">Der eindeutige Bezeichner für die Schemaerweiterungsdefinition.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="6d3cc-147">Sie können einen Wert mit einer von zwei Methoden zuweisen:</span><span class="sxs-lookup"><span data-stu-id="6d3cc-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="6d3cc-p103">Verketten Sie den Namen einer Ihrer überprüften Domänen mit einem Namen für die Schemaerweiterung, um eine eindeutige Zeichenfolge in diesem Format zu bilden: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Beispiel: `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="6d3cc-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="6d3cc-p104">Geben Sie einen Schemanamen an, und verwenden Sie diesen Schemanamen in Microsoft Graph zum Vervollständigen der **id**-Zuweisung in diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Zum Beispiel: `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="6d3cc-152">Diese Eigenschaft kann nach dem Erstellen nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="6d3cc-153">owner</span><span class="sxs-lookup"><span data-stu-id="6d3cc-153">owner</span></span>|<span data-ttu-id="6d3cc-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3cc-154">String</span></span>|<span data-ttu-id="6d3cc-155">Die `appId` der Anwendung, die der Besitzer der Schemaerweiterung ist.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="6d3cc-156">Diese Eigenschaft kann bei der Erstellung bereitgestellt werden, um den Besitzer anzugeben.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="6d3cc-157">Wird Sie nicht bereitgestellt, wird die `appId` der aufrufenden Anwendung als Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="6d3cc-158">In beiden Fällen muss der angemeldete Benutzer angemeldet der Besitzer der Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="6d3cc-159">Wurde diese Eigenschaft einmal festgelegt, ist sie schreibgeschützt und kann nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-159">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="6d3cc-160">properties</span><span class="sxs-lookup"><span data-stu-id="6d3cc-160">properties</span></span>|<span data-ttu-id="6d3cc-161">[extensionSchemaProperty](extensionschemaproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d3cc-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="6d3cc-162">Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="6d3cc-163">status</span><span class="sxs-lookup"><span data-stu-id="6d3cc-163">status</span></span>|<span data-ttu-id="6d3cc-164">String</span><span class="sxs-lookup"><span data-stu-id="6d3cc-164">String</span></span>|<span data-ttu-id="6d3cc-p106">Der Lebenszyklusstatus der Schemaerweiterung. Mögliche Statuswerte sind: **InDevelopment**, **Available** und **Deprecated**. Wird bei der Erstellung automatisch auf **InDevelopment** festgelegt. Unter [Schemaerweiterungen](/graph/extensibility-overview#schema-extensions) finden Sie weitere Informationen zu den möglichen Statusübergängen und Verhaltensweisen.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="6d3cc-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="6d3cc-169">targetTypes</span></span>|<span data-ttu-id="6d3cc-170">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d3cc-170">String collection</span></span>|<span data-ttu-id="6d3cc-171">Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="6d3cc-172">Wählen Sie aus **AdministrativeUnit**, **wenden Sie sich an**, **Gerät**, **Ereignis**, **Gruppe**, **Nachricht**, **Organisation**, **Veröffentlichen**oder **Benutzer**.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-172">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d3cc-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d3cc-173">JSON representation</span></span>

<span data-ttu-id="6d3cc-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d3cc-174">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schemaextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
