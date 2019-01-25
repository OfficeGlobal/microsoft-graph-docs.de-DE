---
title: Verzeichnisberechtigungen Ressourcentyp
description: Directory-Einstellungen können basierend auf der verfügbaren DirectorySettingTemplates erstellt und Standardwerte voreingestellten von geändert werden. Diese Einstellungen können Entität oder ein Feature Verhaltensweisen, sowohl auf einem Mandanten-Ebene oder auf eine bestimmte Entitätsebene steuern. Wenn dieselbe Einstellung auf beide Mandanten geltende und bestimmte Entitätsebene definiert ist, die Einstellung der bestimmte Entität kann von der Einstellung für die gesamte Mandanten zielorientierten.  Beispielsweise die Einstellung für die gesamte Mandanten kann Gäste eingeladen werden, indem vorhandene Mitglieder von Gruppen, aber Einstellung für eine bestimmte Gruppe möglicherweise abmelden und nicht zulassen Gäste durch ein Mitglied der Gruppe eingeladen werden sollen. Derzeit definierten Systemeinstellungen sind nur Office Gruppen Verhalten steuern.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521369"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="17e26-107">Verzeichnisberechtigungen Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="17e26-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17e26-108">Directory-Einstellungen können basierend auf der verfügbaren [DirectorySettingTemplates](directorysettingtemplate.md)erstellt und die voreingestellte Standardeinstellung geändert werden.</span><span class="sxs-lookup"><span data-stu-id="17e26-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="17e26-109">Diese Einstellungen können Entität oder ein Feature Verhaltensweisen, sowohl auf einem Mandanten-Ebene oder auf eine bestimmte Entitätsebene steuern.</span><span class="sxs-lookup"><span data-stu-id="17e26-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="17e26-110">Wenn dieselbe Einstellung auf beide Mandanten geltende und bestimmte Entitätsebene definiert ist, die Einstellung der bestimmte Entität kann von der Einstellung für die gesamte Mandanten zielorientierten.</span><span class="sxs-lookup"><span data-stu-id="17e26-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="17e26-111">Beispielsweise die Einstellung für die gesamte Mandanten kann Gäste eingeladen werden, indem vorhandene Mitglieder von Gruppen, aber Einstellung für eine bestimmte Gruppe möglicherweise abmelden und nicht zulassen Gäste durch ein Mitglied der Gruppe eingeladen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="17e26-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="17e26-112">Derzeit definierten Systemeinstellungen sind nur Office Gruppen Verhalten steuern.</span><span class="sxs-lookup"><span data-stu-id="17e26-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="17e26-113">**Hinweis**: die /beta Version von dem Ressourcentyp Verzeichnisberechtigungen gilt nur für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="17e26-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="17e26-114">Die Version /v1.0 wurde in GroupSetting umbenannt.</span><span class="sxs-lookup"><span data-stu-id="17e26-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="17e26-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="17e26-115">Methods</span></span>

| <span data-ttu-id="17e26-116">Methode</span><span class="sxs-lookup"><span data-stu-id="17e26-116">Method</span></span>           | <span data-ttu-id="17e26-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="17e26-117">Return Type</span></span>    |<span data-ttu-id="17e26-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17e26-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17e26-119">Einstellung erstellen</span><span class="sxs-lookup"><span data-stu-id="17e26-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="17e26-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="17e26-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="17e26-121">Erstellt ein Einstellungsobjekt basierend auf einer directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="17e26-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="17e26-122">Die POST-Anforderung muss settingValues für alle Einstellungen angeben, die in der Vorlage definiert sind.</span><span class="sxs-lookup"><span data-stu-id="17e26-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="17e26-123">Einstellung abrufen</span><span class="sxs-lookup"><span data-stu-id="17e26-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="17e26-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="17e26-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="17e26-125">Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="17e26-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="17e26-126">Einstellungen auflisten</span><span class="sxs-lookup"><span data-stu-id="17e26-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="17e26-127">[directorySetting](directorysetting.md) collection</span><span class="sxs-lookup"><span data-stu-id="17e26-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="17e26-128">Listet Eigenschaften aller Einstellungsobjekte auf.</span><span class="sxs-lookup"><span data-stu-id="17e26-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="17e26-129">Einstellung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="17e26-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="17e26-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="17e26-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="17e26-131">Aktualisiert ein Einstellungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="17e26-131">Update a setting object.</span></span> <span data-ttu-id="17e26-132">Nur EinstellenWerte können in einer Aktualisierung nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="17e26-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="17e26-133">Einstellung löschen</span><span class="sxs-lookup"><span data-stu-id="17e26-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="17e26-134">Keine</span><span class="sxs-lookup"><span data-stu-id="17e26-134">None</span></span> |<span data-ttu-id="17e26-135">Löscht ein Einstellungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="17e26-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="17e26-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17e26-136">Properties</span></span>
| <span data-ttu-id="17e26-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17e26-137">Property</span></span>     | <span data-ttu-id="17e26-138">Typ</span><span class="sxs-lookup"><span data-stu-id="17e26-138">Type</span></span>   |<span data-ttu-id="17e26-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17e26-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17e26-140">displayName</span><span class="sxs-lookup"><span data-stu-id="17e26-140">displayName</span></span>|<span data-ttu-id="17e26-141">string</span><span class="sxs-lookup"><span data-stu-id="17e26-141">string</span></span>|<span data-ttu-id="17e26-142">Anzeigename für diese Gruppe von Einstellungen, der aus der zugeordneten Vorlage stammt.</span><span class="sxs-lookup"><span data-stu-id="17e26-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="17e26-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="17e26-143">Read-only.</span></span>|
|<span data-ttu-id="17e26-144">id</span><span class="sxs-lookup"><span data-stu-id="17e26-144">id</span></span>|<span data-ttu-id="17e26-145">string</span><span class="sxs-lookup"><span data-stu-id="17e26-145">string</span></span>| <span data-ttu-id="17e26-p107">Eindeutiger Bezeichner für diese Einstellungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="17e26-p107">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="17e26-148">templateId</span><span class="sxs-lookup"><span data-stu-id="17e26-148">templateId</span></span>|<span data-ttu-id="17e26-149">string</span><span class="sxs-lookup"><span data-stu-id="17e26-149">string</span></span>| <span data-ttu-id="17e26-p108">Eindeutiger Bezeichner für die Vorlage, die zum Erstellen dieser Gruppe von Einstellungen verwendet wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="17e26-p108">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="17e26-152">values</span><span class="sxs-lookup"><span data-stu-id="17e26-152">values</span></span>|<span data-ttu-id="17e26-153">[settingValue](settingvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="17e26-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="17e26-p109">Sammlung von Name/Wert-Paaren. Muss alle Einstellungen, die in dieser Vorlage definiert sind, enthalten und festlegen.</span><span class="sxs-lookup"><span data-stu-id="17e26-p109">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17e26-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="17e26-156">Relationships</span></span>
<span data-ttu-id="17e26-157">Keine</span><span class="sxs-lookup"><span data-stu-id="17e26-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="17e26-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17e26-158">JSON representation</span></span>

<span data-ttu-id="17e26-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="17e26-159">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
