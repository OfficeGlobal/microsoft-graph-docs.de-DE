---
title: Verzeichnisberechtigungen Ressourcentyp
description: Directory-Einstellungen können basierend auf der verfügbaren DirectorySettingTemplates erstellt und Standardwerte voreingestellten von geändert werden. Diese Einstellungen können Entität oder ein Feature Verhaltensweisen, sowohl auf einem Mandanten-Ebene oder auf eine bestimmte Entitätsebene steuern. Wenn dieselbe Einstellung auf beide Mandanten geltende und bestimmte Entitätsebene definiert ist, die Einstellung der bestimmte Entität kann von der Einstellung für die gesamte Mandanten zielorientierten.  Beispielsweise die Einstellung für die gesamte Mandanten kann Gäste eingeladen werden, indem vorhandene Mitglieder von Gruppen, aber Einstellung für eine bestimmte Gruppe möglicherweise abmelden und nicht zulassen Gäste durch ein Mitglied der Gruppe eingeladen werden sollen. Derzeit definierten Systemeinstellungen sind nur Office Gruppen Verhalten steuern.
localization_priority: Normal
ms.openlocfilehash: 2687df732896abfb8ecf3b0651682228b84fa17b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810137"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="bb36a-107">Verzeichnisberechtigungen Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb36a-107">directorySetting resource type</span></span>

> <span data-ttu-id="bb36a-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bb36a-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb36a-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb36a-110">Directory-Einstellungen können basierend auf der verfügbaren [DirectorySettingTemplates](directorysettingtemplate.md)erstellt und die voreingestellte Standardeinstellung geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bb36a-110">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="bb36a-111">Diese Einstellungen können Entität oder ein Feature Verhaltensweisen, sowohl auf einem Mandanten-Ebene oder auf eine bestimmte Entitätsebene steuern.</span><span class="sxs-lookup"><span data-stu-id="bb36a-111">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="bb36a-112">Wenn dieselbe Einstellung auf beide Mandanten geltende und bestimmte Entitätsebene definiert ist, die Einstellung der bestimmte Entität kann von der Einstellung für die gesamte Mandanten zielorientierten.</span><span class="sxs-lookup"><span data-stu-id="bb36a-112">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="bb36a-113">Beispielsweise die Einstellung für die gesamte Mandanten kann Gäste eingeladen werden, indem vorhandene Mitglieder von Gruppen, aber Einstellung für eine bestimmte Gruppe möglicherweise abmelden und nicht zulassen Gäste durch ein Mitglied der Gruppe eingeladen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bb36a-113">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="bb36a-114">Derzeit definierten Systemeinstellungen sind nur Office Gruppen Verhalten steuern.</span><span class="sxs-lookup"><span data-stu-id="bb36a-114">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="bb36a-115">**Hinweis**: die /beta Version von dem Ressourcentyp Verzeichnisberechtigungen gilt nur für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="bb36a-115">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="bb36a-116">Die Version /v1.0 wurde in GroupSetting umbenannt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-116">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="bb36a-117">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb36a-117">Methods</span></span>

| <span data-ttu-id="bb36a-118">Methode</span><span class="sxs-lookup"><span data-stu-id="bb36a-118">Method</span></span>           | <span data-ttu-id="bb36a-119">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bb36a-119">Return Type</span></span>    |<span data-ttu-id="bb36a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb36a-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb36a-121">Einstellung erstellen</span><span class="sxs-lookup"><span data-stu-id="bb36a-121">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="bb36a-122">Verzeichnisberechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb36a-122">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="bb36a-123">Erstellen einer Einstellungsobjekt basierend auf einer DirectorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="bb36a-123">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="bb36a-124">Die POST-Anforderung muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben.</span><span class="sxs-lookup"><span data-stu-id="bb36a-124">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="bb36a-125">Einstellung abrufen</span><span class="sxs-lookup"><span data-stu-id="bb36a-125">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="bb36a-126">Verzeichnisberechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb36a-126">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="bb36a-127">Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="bb36a-127">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="bb36a-128">Einstellungen auflisten</span><span class="sxs-lookup"><span data-stu-id="bb36a-128">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="bb36a-129">[Verzeichnisberechtigungen](directorysetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb36a-129">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="bb36a-130">Listet Eigenschaften aller Einstellungsobjekte auf.</span><span class="sxs-lookup"><span data-stu-id="bb36a-130">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="bb36a-131">Einstellung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bb36a-131">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="bb36a-132">Verzeichnisberechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb36a-132">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="bb36a-133">Aktualisiert ein Einstellungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-133">Update a setting object.</span></span> <span data-ttu-id="bb36a-134">Nur EinstellenWerte können in einer Aktualisierung nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bb36a-134">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="bb36a-135">Einstellung löschen</span><span class="sxs-lookup"><span data-stu-id="bb36a-135">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="bb36a-136">Keine</span><span class="sxs-lookup"><span data-stu-id="bb36a-136">None</span></span> |<span data-ttu-id="bb36a-137">Löscht ein Einstellungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-137">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb36a-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb36a-138">Properties</span></span>
| <span data-ttu-id="bb36a-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb36a-139">Property</span></span>     | <span data-ttu-id="bb36a-140">Typ</span><span class="sxs-lookup"><span data-stu-id="bb36a-140">Type</span></span>   |<span data-ttu-id="bb36a-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb36a-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb36a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="bb36a-142">displayName</span></span>|<span data-ttu-id="bb36a-143">string</span><span class="sxs-lookup"><span data-stu-id="bb36a-143">string</span></span>|<span data-ttu-id="bb36a-144">Anzeigename für diese Gruppe von Einstellungen, der aus der zugeordneten Vorlage stammt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-144">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="bb36a-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-145">Read-only.</span></span>|
|<span data-ttu-id="bb36a-146">id</span><span class="sxs-lookup"><span data-stu-id="bb36a-146">id</span></span>|<span data-ttu-id="bb36a-147">string</span><span class="sxs-lookup"><span data-stu-id="bb36a-147">string</span></span>| <span data-ttu-id="bb36a-p108">Eindeutiger Bezeichner für diese Einstellungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-p108">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="bb36a-150">templateId</span><span class="sxs-lookup"><span data-stu-id="bb36a-150">templateId</span></span>|<span data-ttu-id="bb36a-151">string</span><span class="sxs-lookup"><span data-stu-id="bb36a-151">string</span></span>| <span data-ttu-id="bb36a-p109">Eindeutiger Bezeichner für die Vorlage, die zum Erstellen dieser Gruppe von Einstellungen verwendet wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb36a-p109">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="bb36a-154">values</span><span class="sxs-lookup"><span data-stu-id="bb36a-154">values</span></span>|<span data-ttu-id="bb36a-155">[settingValue](settingvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bb36a-155">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="bb36a-p110">Sammlung von Name/Wert-Paaren. Muss alle Einstellungen, die in dieser Vorlage definiert sind, enthalten und festlegen.</span><span class="sxs-lookup"><span data-stu-id="bb36a-p110">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb36a-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb36a-158">Relationships</span></span>
<span data-ttu-id="bb36a-159">Keine</span><span class="sxs-lookup"><span data-stu-id="bb36a-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb36a-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb36a-160">JSON representation</span></span>

<span data-ttu-id="bb36a-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb36a-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
