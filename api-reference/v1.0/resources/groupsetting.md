# <a name="groupsetting-resource-type"></a><span data-ttu-id="96a7c-101">groupSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="96a7c-101">groupSetting resource type</span></span>

<span data-ttu-id="96a7c-102">Gruppeneinstellungen steuern Verhalten wie blockierte Wortlisten für Gruppenanzeigenamen oder ob Gastbenutzer Gruppenbesitzer sein können.</span><span class="sxs-lookup"><span data-stu-id="96a7c-102">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="96a7c-p101">Gruppeneinstellungen können basierend auf den verfügbaren [groupSettingTemplates](groupSettingTemplate.md) erstellt werden, und die Standardwerte können geändert werden. Diese Einstellungen regeln Gruppenverhalten auf mandantenweiter Ebene oder für eine bestimmte Gruppe. Wenn die gleiche Einstellung sowohl mandantenweit als auch für eine bestimmte Gruppe definiert ist, überschreibt die Einstellung auf Gruppierungsebene die mandantenweite Einstellung.  So ermöglicht die mandantenweite Einstellung Gästen möglicherweise, von vorhandenen Mitgliedern der Gruppe eingeladen zu werden, wobei eine einzelne Gruppeneinstellung dies jedoch überschreiben und nicht zulassen kann, das Gäste von Mitgliedern der Gruppe eingeladen werden. Gruppeneinstellungen regeln nur das Gruppenverhalten in Office 365.</span><span class="sxs-lookup"><span data-stu-id="96a7c-p101">Group settings can be created based on the available [groupSettingTemplates](groupSettingTemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="96a7c-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="96a7c-108">Methods</span></span>

| <span data-ttu-id="96a7c-109">Methode</span><span class="sxs-lookup"><span data-stu-id="96a7c-109">Method</span></span> | <span data-ttu-id="96a7c-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="96a7c-110">Return Type</span></span> | <span data-ttu-id="96a7c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96a7c-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="96a7c-112">Einstellung erstellen</span><span class="sxs-lookup"><span data-stu-id="96a7c-112">Create setting</span></span>](../api/groupsetting_post_groupsettings.md) | [<span data-ttu-id="96a7c-113">groupSetting</span><span class="sxs-lookup"><span data-stu-id="96a7c-113">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="96a7c-p102">Erstellen Sie eine Einstellungsobjekt basierend auf einer groupSettingTemplate. Die POST-Anforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind.</span><span class="sxs-lookup"><span data-stu-id="96a7c-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="96a7c-116">Einstellung abrufen</span><span class="sxs-lookup"><span data-stu-id="96a7c-116">Get setting</span></span>](../api/groupsetting_get.md) | [<span data-ttu-id="96a7c-117">groupSetting</span><span class="sxs-lookup"><span data-stu-id="96a7c-117">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="96a7c-118">Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="96a7c-118">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="96a7c-119">Einstellungen auflisten</span><span class="sxs-lookup"><span data-stu-id="96a7c-119">List settings</span></span>](../api/groupsetting_list.md) | <span data-ttu-id="96a7c-120">[groupSetting](groupsetting.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96a7c-120">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="96a7c-121">Listet Eigenschaften aller Einstellungsobjekte auf.</span><span class="sxs-lookup"><span data-stu-id="96a7c-121">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="96a7c-122">Einstellung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="96a7c-122">Update setting</span></span>](../api/groupsetting_update.md) | [<span data-ttu-id="96a7c-123">groupSetting</span><span class="sxs-lookup"><span data-stu-id="96a7c-123">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="96a7c-124">groupsetting-Objekt wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="96a7c-124">Update groupsetting object.</span></span> |
|[<span data-ttu-id="96a7c-125">Einstellung löschen</span><span class="sxs-lookup"><span data-stu-id="96a7c-125">Delete setting</span></span>](../api/groupsetting_delete.md) | <span data-ttu-id="96a7c-126">Keine</span><span class="sxs-lookup"><span data-stu-id="96a7c-126">None</span></span> | <span data-ttu-id="96a7c-127">Löscht ein Einstellungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="96a7c-127">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="96a7c-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96a7c-128">Properties</span></span>

| <span data-ttu-id="96a7c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96a7c-129">Property</span></span> | <span data-ttu-id="96a7c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="96a7c-130">Type</span></span> | <span data-ttu-id="96a7c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96a7c-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="96a7c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="96a7c-132">displayName</span></span>|<span data-ttu-id="96a7c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96a7c-133">String</span></span>| <span data-ttu-id="96a7c-134">Anzeigename für diese Gruppe von Einstellungen, der aus der zugeordneten Vorlage stammt.</span><span class="sxs-lookup"><span data-stu-id="96a7c-134">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="96a7c-135">id</span><span class="sxs-lookup"><span data-stu-id="96a7c-135">id</span></span>|<span data-ttu-id="96a7c-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96a7c-136">String</span></span>| <span data-ttu-id="96a7c-p103">Eindeutiger Bezeichner für diese Einstellungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="96a7c-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="96a7c-139">templateId</span><span class="sxs-lookup"><span data-stu-id="96a7c-139">templateId</span></span>|<span data-ttu-id="96a7c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96a7c-140">String</span></span>| <span data-ttu-id="96a7c-p104">Eindeutiger Bezeichner für die Vorlage, die zum Erstellen dieser Gruppe von Einstellungen verwendet wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="96a7c-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="96a7c-143">values</span><span class="sxs-lookup"><span data-stu-id="96a7c-143">values</span></span>|<span data-ttu-id="96a7c-144">[settingValue](settingvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96a7c-144">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="96a7c-p105">Sammlung von Name/Wert-Paaren. Muss alle Einstellungen, die in dieser Vorlage definiert sind, enthalten und festlegen.</span><span class="sxs-lookup"><span data-stu-id="96a7c-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96a7c-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="96a7c-147">Relationships</span></span>

<span data-ttu-id="96a7c-148">Keine.</span><span class="sxs-lookup"><span data-stu-id="96a7c-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96a7c-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96a7c-149">JSON representation</span></span>

<span data-ttu-id="96a7c-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96a7c-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->