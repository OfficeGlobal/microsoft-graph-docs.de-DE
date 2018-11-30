---
title: schemaExtension-Ressourcentyp (Schemaerweiterungen)
description: 'Mithilfe von Schemaerweiterungen können Sie ein Schema definieren, um stark typisierte benutzerdefinierte Daten zu erweitern und einem Ressourcentyp hinzuzufügen. Die benutzerdefinierten Daten werden in der erweiterten Ressource als komplexer Typ angezeigt. '
ms.openlocfilehash: 885b315897814cc15f83526086edb9cf298995f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018960"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="82744-104">schemaExtension-Ressourcentyp (Schemaerweiterungen)</span><span class="sxs-lookup"><span data-stu-id="82744-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="82744-p102">Mithilfe von Schemaerweiterungen können Sie ein Schema definieren, um stark typisierte benutzerdefinierte Daten zu erweitern und einem Ressourcentyp hinzuzufügen. Die benutzerdefinierten Daten werden in der erweiterten Ressource als komplexer Typ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="82744-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="82744-107">Schemaerweiterungen werden von den folgenden Ressourcentypen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="82744-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="82744-108">contact</span><span class="sxs-lookup"><span data-stu-id="82744-108">contact</span></span>](contact.md)
 - [<span data-ttu-id="82744-109">device</span><span class="sxs-lookup"><span data-stu-id="82744-109">device</span></span>](device.md)
 - <span data-ttu-id="82744-110">[event](event.md) in einem Benutzer oder Office 365-Gruppenkalender</span><span class="sxs-lookup"><span data-stu-id="82744-110">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="82744-111">[post](post.md) einer Office 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="82744-111">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="82744-112">group</span><span class="sxs-lookup"><span data-stu-id="82744-112">group</span></span>](group.md)
 - [<span data-ttu-id="82744-113">message</span><span class="sxs-lookup"><span data-stu-id="82744-113">message</span></span>](message.md) 
 - [<span data-ttu-id="82744-114">organization</span><span class="sxs-lookup"><span data-stu-id="82744-114">organization</span></span>](organization.md)
 - [<span data-ttu-id="82744-115">user</span><span class="sxs-lookup"><span data-stu-id="82744-115">user</span></span>](user.md)

<span data-ttu-id="82744-116">Im [Beispiel für Schemaerweiterungen](/graph/extensibility-schema-groups) erfahren Sie, wie Sie benutzerdefinierte Daten zu Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="82744-116">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="82744-117">Methoden</span><span class="sxs-lookup"><span data-stu-id="82744-117">Methods</span></span>

| <span data-ttu-id="82744-118">Methode</span><span class="sxs-lookup"><span data-stu-id="82744-118">Method</span></span>           | <span data-ttu-id="82744-119">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="82744-119">Return Type</span></span>    |<span data-ttu-id="82744-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82744-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82744-121">Create</span><span class="sxs-lookup"><span data-stu-id="82744-121">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="82744-122">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="82744-122">schemaExtension</span></span> |<span data-ttu-id="82744-123">Dient zum Erstellen einer Schemaerweiterungsdefinition.</span><span class="sxs-lookup"><span data-stu-id="82744-123">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="82744-124">List</span><span class="sxs-lookup"><span data-stu-id="82744-124">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="82744-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="82744-125">schemaExtension</span></span> |<span data-ttu-id="82744-126">Dient zum Auflisten der verfügbaren schemaExtension-Definitionen und ihrer Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="82744-126">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="82744-127">Get</span><span class="sxs-lookup"><span data-stu-id="82744-127">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="82744-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="82744-128">schemaExtension</span></span> |<span data-ttu-id="82744-129">Dient zum Lesen der Eigenschaften einer bestimmten schemaExtension-Definition.</span><span class="sxs-lookup"><span data-stu-id="82744-129">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="82744-130">Update</span><span class="sxs-lookup"><span data-stu-id="82744-130">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="82744-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="82744-131">schemaExtension</span></span>   |<span data-ttu-id="82744-132">Dient zum Aktualisieren einer schemaExtension-Definition.</span><span class="sxs-lookup"><span data-stu-id="82744-132">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="82744-133">Delete</span><span class="sxs-lookup"><span data-stu-id="82744-133">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="82744-134">Keine</span><span class="sxs-lookup"><span data-stu-id="82744-134">None</span></span> |<span data-ttu-id="82744-135">Dient zum Löschen einer schemaExtension-Definition.</span><span class="sxs-lookup"><span data-stu-id="82744-135">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="82744-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="82744-136">Properties</span></span>
| <span data-ttu-id="82744-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82744-137">Property</span></span>     | <span data-ttu-id="82744-138">Typ</span><span class="sxs-lookup"><span data-stu-id="82744-138">Type</span></span>   |<span data-ttu-id="82744-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82744-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82744-140">description</span><span class="sxs-lookup"><span data-stu-id="82744-140">description</span></span>|<span data-ttu-id="82744-141">String</span><span class="sxs-lookup"><span data-stu-id="82744-141">String</span></span>|<span data-ttu-id="82744-142">Beschreibung für die Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="82744-142">Description for the schema extension.</span></span>|
|<span data-ttu-id="82744-143">id</span><span class="sxs-lookup"><span data-stu-id="82744-143">id</span></span>|<span data-ttu-id="82744-144">String</span><span class="sxs-lookup"><span data-stu-id="82744-144">String</span></span>|<span data-ttu-id="82744-145">Der eindeutige Bezeichner für die Schemaerweiterungsdefinition.</span><span class="sxs-lookup"><span data-stu-id="82744-145">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="82744-146">Sie können einen Wert mit einer von zwei Methoden zuweisen:</span><span class="sxs-lookup"><span data-stu-id="82744-146">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="82744-p103">Verketten Sie den Namen einer Ihrer überprüften Domänen mit einem Namen für die Schemaerweiterung, um eine eindeutige Zeichenfolge in diesem Format zu bilden: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Beispiel: `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="82744-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="82744-p104">Geben Sie einen Schemanamen an, und verwenden Sie diesen Schemanamen in Microsoft Graph zum Vervollständigen der **id**-Zuweisung in diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Zum Beispiel: `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="82744-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="82744-151">Diese Eigenschaft kann nach dem Erstellen nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="82744-151">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="82744-152">owner</span><span class="sxs-lookup"><span data-stu-id="82744-152">owner</span></span>|<span data-ttu-id="82744-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82744-153">String</span></span>|<span data-ttu-id="82744-154">Die `appId` der Anwendung, die der Besitzer der Schemaerweiterung ist.</span><span class="sxs-lookup"><span data-stu-id="82744-154">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="82744-155">Diese Eigenschaft kann bei der Erstellung bereitgestellt werden, um den Besitzer anzugeben.</span><span class="sxs-lookup"><span data-stu-id="82744-155">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="82744-156">Wird Sie nicht bereitgestellt, wird die `appId` der aufrufenden Anwendung als Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="82744-156">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="82744-157">In beiden Fällen muss der angemeldete Benutzer angemeldet der Besitzer der Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="82744-157">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="82744-158">Wurde diese Eigenschaft einmal festgelegt, ist sie schreibgeschützt und kann nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="82744-158">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="82744-159">properties</span><span class="sxs-lookup"><span data-stu-id="82744-159">properties</span></span>|<span data-ttu-id="82744-160">[extensionSchemaProperty](extensionschemaproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="82744-160">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="82744-161">Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden.</span><span class="sxs-lookup"><span data-stu-id="82744-161">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="82744-162">status</span><span class="sxs-lookup"><span data-stu-id="82744-162">status</span></span>|<span data-ttu-id="82744-163">String</span><span class="sxs-lookup"><span data-stu-id="82744-163">String</span></span>|<span data-ttu-id="82744-p106">Der Lebenszyklusstatus der Schemaerweiterung. Mögliche Statuswerte sind: **InDevelopment**, **Available** und **Deprecated**. Wird bei der Erstellung automatisch auf **InDevelopment** festgelegt. Unter [Schemaerweiterungen](/graph/extensibility-overview#schema-extensions) finden Sie weitere Informationen zu den möglichen Statusübergängen und Verhaltensweisen.</span><span class="sxs-lookup"><span data-stu-id="82744-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="82744-168">targetTypes</span><span class="sxs-lookup"><span data-stu-id="82744-168">targetTypes</span></span>|<span data-ttu-id="82744-169">String collection</span><span class="sxs-lookup"><span data-stu-id="82744-169">String collection</span></span>|<span data-ttu-id="82744-p107">Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann. Zur Auswahl stehen **contact**, **device**, **event**, **group**, **message**, **organization**, **post** und **user**.</span><span class="sxs-lookup"><span data-stu-id="82744-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82744-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="82744-172">JSON representation</span></span>

<span data-ttu-id="82744-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="82744-173">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->