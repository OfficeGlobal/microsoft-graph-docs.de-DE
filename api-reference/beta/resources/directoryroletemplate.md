---
title: Ressourcentyp directoryRoleTemplate
description: 'Stellt eine Verzeichnis Rollenvorlage dar. Vorlage Rolle Directory gibt die Eigenschaftswerte einer Directory-Rolle (DirectoryRole). Es ist eine zugehörige Verzeichnis Rolle Template-Objekt für jede der Directory Rollen, die in einem Mandanten aktiviert werden können. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert. Andere Rollen verfügbaren Verzeichnis zu aktivieren, die Sie Senden einer POST-Anforderung an den `/directoryRoles` Endpunkt mit der ID des Directory Rolle die Rolle Directory auf dem basiert angegebenen Vorlage im **RoleTemplateId** -Parameter der Anforderung. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie dann zum Lesen und Zuweisen von Mitgliedern zur Rolle Directory starten. **Hinweis**: Directory Rollenvorlage ist für die Rolle der Benutzer Directory verfügbar gemacht werden. Die Benutzer-Directory-Rolle ist implizit und ist für Directory-Clients nicht sichtbar. Jeder Benutzer in den Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b4a4e79c11f38991da88cd685983229c9f7da7b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938181"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="e730a-114">Ressourcentyp directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="e730a-114">directoryRoleTemplate resource type</span></span>

> <span data-ttu-id="e730a-115">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e730a-115">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e730a-116">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e730a-116">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e730a-p103">Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle [DirectoryRole](directoryrole.md) an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den `/directoryRoles`-Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter **RoleTemplateId** der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. **Hinweis**: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.</span><span class="sxs-lookup"><span data-stu-id="e730a-p103">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="e730a-129">Methoden</span><span class="sxs-lookup"><span data-stu-id="e730a-129">Methods</span></span>

| <span data-ttu-id="e730a-130">Methode</span><span class="sxs-lookup"><span data-stu-id="e730a-130">Method</span></span>       | <span data-ttu-id="e730a-131">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e730a-131">Return Type</span></span>  |<span data-ttu-id="e730a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e730a-132">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e730a-133">directoryRoleTemplate abrufen</span><span class="sxs-lookup"><span data-stu-id="e730a-133">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="e730a-134">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="e730a-134">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="e730a-135">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRoleTemplate-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e730a-135">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e730a-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e730a-136">Properties</span></span>
| <span data-ttu-id="e730a-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e730a-137">Property</span></span>     | <span data-ttu-id="e730a-138">Typ</span><span class="sxs-lookup"><span data-stu-id="e730a-138">Type</span></span>   |<span data-ttu-id="e730a-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e730a-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e730a-140">description</span><span class="sxs-lookup"><span data-stu-id="e730a-140">description</span></span>|<span data-ttu-id="e730a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e730a-141">String</span></span>|<span data-ttu-id="e730a-p104">Die festzulegende Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e730a-p104">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="e730a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="e730a-144">displayName</span></span>|<span data-ttu-id="e730a-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e730a-145">String</span></span>|<span data-ttu-id="e730a-p105">Der festzulegende Name für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e730a-p105">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="e730a-148">id</span><span class="sxs-lookup"><span data-stu-id="e730a-148">id</span></span>|<span data-ttu-id="e730a-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e730a-149">String</span></span>|<span data-ttu-id="e730a-p106">Der eindeutige Bezeichner für die Vorlage. Geerbt von [directoryObject](directoryobject.md). Sie geben die **id** der Verzeichnisrollenvorlage die Eigenschaft **RoleTemplateId** in der POST-Anforderung zum Aktivieren einer [DirectoryRole](directoryrole.md) in einen Mandanten an. Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e730a-p106">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e730a-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e730a-155">Relationships</span></span>
<span data-ttu-id="e730a-156">Keine</span><span class="sxs-lookup"><span data-stu-id="e730a-156">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="e730a-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e730a-157">JSON representation</span></span>

<span data-ttu-id="e730a-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e730a-158">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
