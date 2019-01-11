---
title: groupSetting-Ressourcentyp
description: Gruppeneinstellungen steuern Verhalten wie blockierte Wortlisten für Gruppenanzeigenamen oder ob Gastbenutzer Gruppenbesitzer sein können.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4508de9c03820031e47e3457e24dc39ed14c36a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840768"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="5cec2-103">groupSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5cec2-103">groupSetting resource type</span></span>

<span data-ttu-id="5cec2-104">Gruppeneinstellungen steuern Verhalten wie blockierte Wortlisten für Gruppenanzeigenamen oder ob Gastbenutzer Gruppenbesitzer sein können.</span><span class="sxs-lookup"><span data-stu-id="5cec2-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="5cec2-p101">Gruppeneinstellungen können basierend auf den verfügbaren [groupSettingTemplates](groupsettingtemplate.md) erstellt werden, und die Standardwerte können geändert werden. Diese Einstellungen regeln Gruppenverhalten auf mandantenweiter Ebene oder für eine bestimmte Gruppe. Wenn die gleiche Einstellung sowohl mandantenweit als auch für eine bestimmte Gruppe definiert ist, überschreibt die Einstellung auf Gruppierungsebene die mandantenweite Einstellung.  So ermöglicht die mandantenweite Einstellung Gästen möglicherweise, von vorhandenen Mitgliedern der Gruppe eingeladen zu werden, wobei eine einzelne Gruppeneinstellung dies jedoch überschreiben und nicht zulassen kann, das Gäste von Mitgliedern der Gruppe eingeladen werden. Gruppeneinstellungen regeln nur das Gruppenverhalten in Office 365.</span><span class="sxs-lookup"><span data-stu-id="5cec2-p101">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="5cec2-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="5cec2-110">Methods</span></span>

| <span data-ttu-id="5cec2-111">Methode</span><span class="sxs-lookup"><span data-stu-id="5cec2-111">Method</span></span> | <span data-ttu-id="5cec2-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5cec2-112">Return Type</span></span> | <span data-ttu-id="5cec2-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5cec2-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cec2-114">Einstellung erstellen</span><span class="sxs-lookup"><span data-stu-id="5cec2-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="5cec2-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="5cec2-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="5cec2-p102">Erstellen Sie eine Einstellungsobjekt basierend auf einer groupSettingTemplate. Die POST-Anforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind.</span><span class="sxs-lookup"><span data-stu-id="5cec2-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="5cec2-118">Einstellung abrufen</span><span class="sxs-lookup"><span data-stu-id="5cec2-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="5cec2-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="5cec2-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="5cec2-120">Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="5cec2-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="5cec2-121">Einstellungen auflisten</span><span class="sxs-lookup"><span data-stu-id="5cec2-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="5cec2-122">[groupSetting](groupsetting.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5cec2-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="5cec2-123">Listet Eigenschaften aller Einstellungsobjekte auf.</span><span class="sxs-lookup"><span data-stu-id="5cec2-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="5cec2-124">Einstellung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5cec2-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="5cec2-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="5cec2-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="5cec2-126">groupsetting-Objekt wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5cec2-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="5cec2-127">Einstellung löschen</span><span class="sxs-lookup"><span data-stu-id="5cec2-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="5cec2-128">Keine</span><span class="sxs-lookup"><span data-stu-id="5cec2-128">None</span></span> | <span data-ttu-id="5cec2-129">Löscht ein Einstellungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="5cec2-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cec2-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5cec2-130">Properties</span></span>

| <span data-ttu-id="5cec2-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5cec2-131">Property</span></span> | <span data-ttu-id="5cec2-132">Typ</span><span class="sxs-lookup"><span data-stu-id="5cec2-132">Type</span></span> | <span data-ttu-id="5cec2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5cec2-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5cec2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5cec2-134">displayName</span></span>|<span data-ttu-id="5cec2-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5cec2-135">String</span></span>| <span data-ttu-id="5cec2-136">Anzeigename für diese Gruppe von Einstellungen, der aus der zugeordneten Vorlage stammt.</span><span class="sxs-lookup"><span data-stu-id="5cec2-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="5cec2-137">id</span><span class="sxs-lookup"><span data-stu-id="5cec2-137">id</span></span>|<span data-ttu-id="5cec2-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5cec2-138">String</span></span>| <span data-ttu-id="5cec2-p103">Eindeutiger Bezeichner für diese Einstellungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5cec2-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="5cec2-141">templateId</span><span class="sxs-lookup"><span data-stu-id="5cec2-141">templateId</span></span>|<span data-ttu-id="5cec2-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5cec2-142">String</span></span>| <span data-ttu-id="5cec2-p104">Eindeutiger Bezeichner für die Vorlage, die zum Erstellen dieser Gruppe von Einstellungen verwendet wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5cec2-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="5cec2-145">values</span><span class="sxs-lookup"><span data-stu-id="5cec2-145">values</span></span>|<span data-ttu-id="5cec2-146">[settingValue](settingvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5cec2-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="5cec2-p105">Sammlung von Name/Wert-Paaren. Muss alle Einstellungen, die in dieser Vorlage definiert sind, enthalten und festlegen.</span><span class="sxs-lookup"><span data-stu-id="5cec2-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5cec2-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5cec2-149">Relationships</span></span>

<span data-ttu-id="5cec2-150">Keine.</span><span class="sxs-lookup"><span data-stu-id="5cec2-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cec2-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5cec2-151">JSON representation</span></span>

<span data-ttu-id="5cec2-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5cec2-152">Here is a JSON representation of the resource.</span></span>

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
