# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="e3d87-101">groupSettingTemplate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3d87-101">groupSettingTemplate resource type</span></span>

<span data-ttu-id="e3d87-p101">Gruppeneinstellungsvorlagen stellen systemdefinierte Einstellungen dar, die für den Mandanten verfügbar sind. [Gruppeneinstellungen](groupsetting.md) können basierend auf den verfügbaren **groupSettingTemplates** erstellt werden, und die Standardwerte können geändert werden. Gruppeneinstellungsvorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können mandantenweite Einstellungen oder bestimmte Gruppeneinstellungen darstellen. Die derzeit einzig verfügbaren Vorlagen beziehen sich auf Office 365-Gruppen und umfassen Einstellungen dazu, ob Benutzer Gruppen erstellen oder Gäste von außerhalb der Organisation einladen können, Mitglieder einer Gruppe zu werden.</span><span class="sxs-lookup"><span data-stu-id="e3d87-p101">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="e3d87-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="e3d87-107">Methods</span></span>

| <span data-ttu-id="e3d87-108">Methode</span><span class="sxs-lookup"><span data-stu-id="e3d87-108">Method</span></span> | <span data-ttu-id="e3d87-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e3d87-109">Return Type</span></span> | <span data-ttu-id="e3d87-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3d87-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3d87-111">Get groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="e3d87-111">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate_get.md) | [<span data-ttu-id="e3d87-112">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="e3d87-112">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="e3d87-113">Liest die spezifischen Eigenschaften eines vom System definierten groupSettingTemplate-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3d87-113">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="e3d87-114">List groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="e3d87-114">List groupSettingTemplate</span></span>](../api/groupsettingtemplate_list.md) | [<span data-ttu-id="e3d87-115">Sammlung von groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="e3d87-115">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="e3d87-116">Listet alle der vom System definierten groupSettingTemplate-Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="e3d87-116">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3d87-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3d87-117">Properties</span></span>

| <span data-ttu-id="e3d87-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3d87-118">Property</span></span> | <span data-ttu-id="e3d87-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e3d87-119">Type</span></span> | <span data-ttu-id="e3d87-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3d87-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e3d87-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3d87-121">description</span></span>|<span data-ttu-id="e3d87-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3d87-122">String</span></span>| <span data-ttu-id="e3d87-123">Beschreibung der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="e3d87-123">Description of the template.</span></span> |
|<span data-ttu-id="e3d87-124">displayName</span><span class="sxs-lookup"><span data-stu-id="e3d87-124">displayName</span></span>|<span data-ttu-id="e3d87-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3d87-125">String</span></span>| <span data-ttu-id="e3d87-126">Anzeigename der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="e3d87-126">Display name of the template.</span></span> |
|<span data-ttu-id="e3d87-127">id</span><span class="sxs-lookup"><span data-stu-id="e3d87-127">id</span></span>|<span data-ttu-id="e3d87-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3d87-128">String</span></span>| <span data-ttu-id="e3d87-p102">Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3d87-p102">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="e3d87-131">values</span><span class="sxs-lookup"><span data-stu-id="e3d87-131">values</span></span>|<span data-ttu-id="e3d87-132">[settingTemplateValue](settingtemplatevalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e3d87-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="e3d87-133">Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden.</span><span class="sxs-lookup"><span data-stu-id="e3d87-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e3d87-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3d87-134">Relationships</span></span>

<span data-ttu-id="e3d87-135">Keine.</span><span class="sxs-lookup"><span data-stu-id="e3d87-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e3d87-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3d87-136">JSON representation</span></span>

<span data-ttu-id="e3d87-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3d87-137">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->