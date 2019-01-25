---
title: Ressourcentyp directoryRoleTemplate
description: 'Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle DirectoryRole an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den -Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter RoleTemplateId der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. Hinweis: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd813c9f7676e7190e5aedbb6d9b950e9ffc6aac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526158"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="d54a7-114">Ressourcentyp directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="d54a7-114">directoryRoleTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d54a7-p102">Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle [DirectoryRole](directoryrole.md) an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den `/directoryRoles`-Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter **RoleTemplateId** der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. **Hinweis**: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.</span><span class="sxs-lookup"><span data-stu-id="d54a7-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="d54a7-127">Methoden</span><span class="sxs-lookup"><span data-stu-id="d54a7-127">Methods</span></span>

| <span data-ttu-id="d54a7-128">Methode</span><span class="sxs-lookup"><span data-stu-id="d54a7-128">Method</span></span>       | <span data-ttu-id="d54a7-129">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d54a7-129">Return Type</span></span>  |<span data-ttu-id="d54a7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d54a7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d54a7-131">directoryRoleTemplate abrufen</span><span class="sxs-lookup"><span data-stu-id="d54a7-131">[Get directoryRoleTemplate](../api/directoryroletemplate-get.md)</span></span> | [<span data-ttu-id="d54a7-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="d54a7-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="d54a7-133">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRoleTemplate-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d54a7-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d54a7-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d54a7-134">Properties</span></span>
| <span data-ttu-id="d54a7-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d54a7-135">Property</span></span>     | <span data-ttu-id="d54a7-136">Typ</span><span class="sxs-lookup"><span data-stu-id="d54a7-136">Type</span></span>   |<span data-ttu-id="d54a7-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d54a7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d54a7-138">description</span><span class="sxs-lookup"><span data-stu-id="d54a7-138">description</span></span>|<span data-ttu-id="d54a7-139">String</span><span class="sxs-lookup"><span data-stu-id="d54a7-139">String</span></span>|<span data-ttu-id="d54a7-p103">Die festzulegende Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d54a7-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="d54a7-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d54a7-142">displayName</span></span>|<span data-ttu-id="d54a7-143">String</span><span class="sxs-lookup"><span data-stu-id="d54a7-143">String</span></span>|<span data-ttu-id="d54a7-p104">Der festzulegende Name für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d54a7-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="d54a7-146">id</span><span class="sxs-lookup"><span data-stu-id="d54a7-146">id</span></span>|<span data-ttu-id="d54a7-147">string</span><span class="sxs-lookup"><span data-stu-id="d54a7-147">String</span></span>|<span data-ttu-id="d54a7-p105">Der eindeutige Bezeichner für die Vorlage. Geerbt von [directoryObject](directoryobject.md). Sie geben die **id** der Verzeichnisrollenvorlage die Eigenschaft **RoleTemplateId** in der POST-Anforderung zum Aktivieren einer [DirectoryRole](directoryrole.md) in einen Mandanten an. Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d54a7-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d54a7-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d54a7-153">Relationships</span></span>
<span data-ttu-id="d54a7-154">Keine</span><span class="sxs-lookup"><span data-stu-id="d54a7-154">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="d54a7-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d54a7-155">JSON representation</span></span>

<span data-ttu-id="d54a7-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d54a7-156">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryroletemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
