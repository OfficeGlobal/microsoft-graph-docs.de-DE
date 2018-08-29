# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="08e67-101">Ressourcentyp directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="08e67-101">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="08e67-p101">Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle [DirectoryRole](directoryrole.md) an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den `/directoryRoles`-Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter **RoleTemplateId** der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. **Hinweis**: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.</span><span class="sxs-lookup"><span data-stu-id="08e67-p101">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="08e67-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="08e67-114">Methods</span></span>

| <span data-ttu-id="08e67-115">Methode</span><span class="sxs-lookup"><span data-stu-id="08e67-115">Method</span></span>       | <span data-ttu-id="08e67-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="08e67-116">Return Type</span></span>  |<span data-ttu-id="08e67-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e67-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08e67-118">directoryRoleTemplate abrufen</span><span class="sxs-lookup"><span data-stu-id="08e67-118">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate_get.md) | [<span data-ttu-id="08e67-119">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="08e67-119">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="08e67-120">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRoleTemplate-Objekts.</span><span class="sxs-lookup"><span data-stu-id="08e67-120">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="08e67-121">directoryRoleTemplate auflisten</span><span class="sxs-lookup"><span data-stu-id="08e67-121">List directoryRoleTemplate</span></span>](../api/directoryroletemplate_list.md) | <span data-ttu-id="08e67-122">|||UNTRANSLATED_CONTENT_START|||[directoryRoleTemplate](directoryroletemplate.md) collection|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="08e67-122">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="08e67-123">Dient zum Abrufen einer Liste von directoryRoleTemplate-Objekten.</span><span class="sxs-lookup"><span data-stu-id="08e67-123">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="08e67-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08e67-124">Properties</span></span>
| <span data-ttu-id="08e67-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08e67-125">Property</span></span>     | <span data-ttu-id="08e67-126">Typ</span><span class="sxs-lookup"><span data-stu-id="08e67-126">Type</span></span>   |<span data-ttu-id="08e67-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e67-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08e67-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e67-128">description</span></span>|<span data-ttu-id="08e67-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e67-129">String</span></span>|<span data-ttu-id="08e67-p102">Die festzulegende Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08e67-p102">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="08e67-132">displayName</span><span class="sxs-lookup"><span data-stu-id="08e67-132">displayName</span></span>|<span data-ttu-id="08e67-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e67-133">String</span></span>|<span data-ttu-id="08e67-p103">Der festzulegende Name für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08e67-p103">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="08e67-136">id</span><span class="sxs-lookup"><span data-stu-id="08e67-136">id</span></span>|<span data-ttu-id="08e67-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e67-137">String</span></span>|<span data-ttu-id="08e67-p104">Der eindeutige Bezeichner für die Vorlage. Geerbt von [directoryObject](directoryobject.md). Sie geben die **id** der Verzeichnisrollenvorlage die Eigenschaft **RoleTemplateId** in der POST-Anforderung zum Aktivieren einer [DirectoryRole](directoryrole.md) in einen Mandanten an. Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08e67-p104">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08e67-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08e67-143">Relationships</span></span>
<span data-ttu-id="08e67-144">Keine</span><span class="sxs-lookup"><span data-stu-id="08e67-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="08e67-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08e67-145">JSON representation</span></span>

<span data-ttu-id="08e67-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08e67-146">Here is a JSON representation of the resource</span></span>

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
