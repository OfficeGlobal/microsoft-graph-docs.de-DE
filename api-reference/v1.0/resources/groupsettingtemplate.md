---
title: groupSettingTemplate-Ressourcentyp
description: Gruppeneinstellungsvorlagen stellen systemdefinierte Einstellungen dar, die für den Mandanten verfügbar sind. Gruppeneinstellungen können basierend auf den verfügbaren **groupSettingTemplates** erstellt werden, und die Standardwerte können geändert werden. Gruppeneinstellungsvorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können mandantenweite Einstellungen oder bestimmte Gruppeneinstellungen darstellen. Die derzeit einzig verfügbaren Vorlagen beziehen sich auf Office 365-Gruppen und umfassen Einstellungen dazu, ob Benutzer Gruppen erstellen oder Gäste von außerhalb der Organisation einladen können, Mitglieder einer Gruppe zu werden.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b9b95303b72bc111f045010e71459f541e9a9b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919337"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="38854-107">groupSettingTemplate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="38854-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="38854-p102">Gruppeneinstellungsvorlagen stellen systemdefinierte Einstellungen dar, die für den Mandanten verfügbar sind. [Gruppeneinstellungen](groupsetting.md) können basierend auf den verfügbaren **groupSettingTemplates** erstellt werden, und die Standardwerte können geändert werden. Gruppeneinstellungsvorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können mandantenweite Einstellungen oder bestimmte Gruppeneinstellungen darstellen. Die derzeit einzig verfügbaren Vorlagen beziehen sich auf Office 365-Gruppen und umfassen Einstellungen dazu, ob Benutzer Gruppen erstellen oder Gäste von außerhalb der Organisation einladen können, Mitglieder einer Gruppe zu werden.</span><span class="sxs-lookup"><span data-stu-id="38854-p102">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="38854-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="38854-113">Methods</span></span>

| <span data-ttu-id="38854-114">Methode</span><span class="sxs-lookup"><span data-stu-id="38854-114">Method</span></span> | <span data-ttu-id="38854-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="38854-115">Return Type</span></span> | <span data-ttu-id="38854-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38854-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="38854-117">Get groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="38854-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="38854-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="38854-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="38854-119">Liest die spezifischen Eigenschaften eines vom System definierten groupSettingTemplate-Objekts.</span><span class="sxs-lookup"><span data-stu-id="38854-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="38854-120">List groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="38854-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="38854-121">Sammlung von groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="38854-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="38854-122">Listet alle der vom System definierten groupSettingTemplate-Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="38854-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="38854-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38854-123">Properties</span></span>

| <span data-ttu-id="38854-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38854-124">Property</span></span> | <span data-ttu-id="38854-125">Typ</span><span class="sxs-lookup"><span data-stu-id="38854-125">Type</span></span> | <span data-ttu-id="38854-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38854-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="38854-127">description</span><span class="sxs-lookup"><span data-stu-id="38854-127">description</span></span>|<span data-ttu-id="38854-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38854-128">String</span></span>| <span data-ttu-id="38854-129">Beschreibung der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="38854-129">Description of the template.</span></span> |
|<span data-ttu-id="38854-130">displayName</span><span class="sxs-lookup"><span data-stu-id="38854-130">displayName</span></span>|<span data-ttu-id="38854-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38854-131">String</span></span>| <span data-ttu-id="38854-132">Anzeigename der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="38854-132">Display name of the template.</span></span> |
|<span data-ttu-id="38854-133">id</span><span class="sxs-lookup"><span data-stu-id="38854-133">id</span></span>|<span data-ttu-id="38854-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38854-134">String</span></span>| <span data-ttu-id="38854-p103">Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38854-p103">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="38854-137">values</span><span class="sxs-lookup"><span data-stu-id="38854-137">values</span></span>|<span data-ttu-id="38854-138">[settingTemplateValue](settingtemplatevalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38854-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="38854-139">Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden.</span><span class="sxs-lookup"><span data-stu-id="38854-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="38854-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="38854-140">Relationships</span></span>

<span data-ttu-id="38854-141">Keine.</span><span class="sxs-lookup"><span data-stu-id="38854-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="38854-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38854-142">JSON representation</span></span>

<span data-ttu-id="38854-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38854-143">Here is a JSON representation of the resource.</span></span>

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
