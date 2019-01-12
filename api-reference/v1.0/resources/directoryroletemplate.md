---
title: Ressourcentyp directoryRoleTemplate
description: 'Stellt eine Verzeichnis Rollenvorlage dar. Vorlage Rolle Directory gibt die Eigenschaftswerte einer Directory-Rolle (DirectoryRole). Es ist eine zugehörige Verzeichnis Rolle Template-Objekt für jede der Directory Rollen, die in einem Mandanten aktiviert werden können. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert. Andere Rollen verfügbaren Verzeichnis zu aktivieren, die Sie Senden einer POST-Anforderung an den `/directoryRoles` Endpunkt mit der ID des Directory Rolle die Rolle Directory auf dem basiert angegebenen Vorlage im **RoleTemplateId** -Parameter der Anforderung. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie dann zum Lesen und Zuweisen von Mitgliedern zur Rolle Directory starten. **Hinweis**: Directory Rollenvorlage ist für die Rolle der Benutzer Directory verfügbar gemacht werden. Die Benutzer-Directory-Rolle ist implizit und ist für Directory-Clients nicht sichtbar. Jeder Benutzer in den Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 57dec43699ba75c7e936fa02dbdf09df74dd06ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966993"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="c8988-114">Ressourcentyp directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="c8988-114">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="c8988-p102">Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle [DirectoryRole](directoryrole.md) an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den `/directoryRoles`-Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter **RoleTemplateId** der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. **Hinweis**: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.</span><span class="sxs-lookup"><span data-stu-id="c8988-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="c8988-127">Methoden</span><span class="sxs-lookup"><span data-stu-id="c8988-127">Methods</span></span>

| <span data-ttu-id="c8988-128">Methode</span><span class="sxs-lookup"><span data-stu-id="c8988-128">Method</span></span>       | <span data-ttu-id="c8988-129">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c8988-129">Return Type</span></span>  |<span data-ttu-id="c8988-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8988-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8988-131">directoryRoleTemplate abrufen</span><span class="sxs-lookup"><span data-stu-id="c8988-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="c8988-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="c8988-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="c8988-133">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRoleTemplate-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c8988-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="c8988-134">directoryRoleTemplate auflisten</span><span class="sxs-lookup"><span data-stu-id="c8988-134">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="c8988-135">[directoryRoleTemplate-Sammlung](directoryroletemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c8988-135">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="c8988-136">Dient zum Abrufen einer Liste von directoryRoleTemplate-Objekten.</span><span class="sxs-lookup"><span data-stu-id="c8988-136">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8988-137">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c8988-137">Properties</span></span>
| <span data-ttu-id="c8988-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8988-138">Property</span></span>     | <span data-ttu-id="c8988-139">Typ</span><span class="sxs-lookup"><span data-stu-id="c8988-139">Type</span></span>   |<span data-ttu-id="c8988-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8988-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8988-141">description</span><span class="sxs-lookup"><span data-stu-id="c8988-141">description</span></span>|<span data-ttu-id="c8988-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8988-142">String</span></span>|<span data-ttu-id="c8988-p103">Die festzulegende Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c8988-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="c8988-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c8988-145">displayName</span></span>|<span data-ttu-id="c8988-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8988-146">String</span></span>|<span data-ttu-id="c8988-p104">Der festzulegende Name für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c8988-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="c8988-149">id</span><span class="sxs-lookup"><span data-stu-id="c8988-149">id</span></span>|<span data-ttu-id="c8988-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8988-150">String</span></span>|<span data-ttu-id="c8988-p105">Der eindeutige Bezeichner für die Vorlage. Geerbt von [directoryObject](directoryobject.md). Sie geben die **id** der Verzeichnisrollenvorlage die Eigenschaft **RoleTemplateId** in der POST-Anforderung zum Aktivieren einer [DirectoryRole](directoryrole.md) in einen Mandanten an. Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c8988-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8988-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c8988-156">Relationships</span></span>
<span data-ttu-id="c8988-157">Keine</span><span class="sxs-lookup"><span data-stu-id="c8988-157">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="c8988-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c8988-158">JSON representation</span></span>

<span data-ttu-id="c8988-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c8988-159">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
