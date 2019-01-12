---
title: Ressourcentyp directorySettingTemplate
description: Verzeichnis Einstellung Vorlagen darstellen, die dem Mandanten verfügbaren systemdefinierte Einstellungen. Directory-Einstellungen können anhand der verfügbaren DirectorySettingTemplates und Werte geändert voreingestellten Standardwerte von erstellt werden. Verzeichnis Einstellung Vorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können Mandanten geltende Einstellungen darstellen, oder Sie können bestimmte Entität Einstellungen darstellen.  Derzeit nur verfügbaren Vorlagen gelten für Office-Gruppen und umfassen Einstellungen wie gibt an, ob Benutzer Gruppen erstellen oder Gäste außerhalb der Organisation, die Mitglied einer Gruppe werden einladen können.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d950b94c71bae70474bf9cdb9eee76fb8a3d9134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957634"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="8cf89-107">Ressourcentyp directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8cf89-107">directorySettingTemplate resource type</span></span>

> <span data-ttu-id="8cf89-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8cf89-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cf89-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8cf89-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cf89-110">Verzeichnis Einstellung Vorlagen darstellen, die dem Mandanten verfügbaren systemdefinierte Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="8cf89-110">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="8cf89-111">[Directory-Einstellungen](directorysetting.md) können anhand der verfügbaren DirectorySettingTemplates und Werte geändert voreingestellten Standardwerte von erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="8cf89-111">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="8cf89-112">Verzeichnis Einstellung Vorlagen können nicht erstellt, aktualisiert oder gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="8cf89-112">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="8cf89-113">Diese Einstellungen können Mandanten geltende Einstellungen darstellen, oder Sie können bestimmte Entität Einstellungen darstellen.</span><span class="sxs-lookup"><span data-stu-id="8cf89-113">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="8cf89-114">Derzeit nur verfügbaren Vorlagen gelten für Office-Gruppen und umfassen Einstellungen wie gibt an, ob Benutzer Gruppen erstellen oder Gäste außerhalb der Organisation, die Mitglied einer Gruppe werden einladen können.</span><span class="sxs-lookup"><span data-stu-id="8cf89-114">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="8cf89-115">**Hinweis**: die /beta Version von dem Ressourcentyp DirectorySettingTemplate gilt nur für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="8cf89-115">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="8cf89-116">Die Version /v1.0 wurde in GroupSettingTemplate umbenannt.</span><span class="sxs-lookup"><span data-stu-id="8cf89-116">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="8cf89-117">Methoden</span><span class="sxs-lookup"><span data-stu-id="8cf89-117">Methods</span></span>

| <span data-ttu-id="8cf89-118">Methode</span><span class="sxs-lookup"><span data-stu-id="8cf89-118">Method</span></span>           | <span data-ttu-id="8cf89-119">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8cf89-119">Return Type</span></span>    |<span data-ttu-id="8cf89-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8cf89-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cf89-121">Abrufen von directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8cf89-121">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="8cf89-122">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8cf89-122">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="8cf89-123">Lesen Sie die spezifischen Eigenschaften der eines der Objekte DirectorySettingTemplate System definiert.</span><span class="sxs-lookup"><span data-stu-id="8cf89-123">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="8cf89-124">Liste directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8cf89-124">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="8cf89-125">Auflistung von directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8cf89-125">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="8cf89-126">Listen Sie aller vom System definierten DirectorySettingTemplate Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="8cf89-126">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cf89-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8cf89-127">Properties</span></span>
| <span data-ttu-id="8cf89-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8cf89-128">Property</span></span>     | <span data-ttu-id="8cf89-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8cf89-129">Type</span></span>   |<span data-ttu-id="8cf89-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8cf89-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cf89-131">description</span><span class="sxs-lookup"><span data-stu-id="8cf89-131">description</span></span>|<span data-ttu-id="8cf89-132">string</span><span class="sxs-lookup"><span data-stu-id="8cf89-132">string</span></span>|<span data-ttu-id="8cf89-133">Beschreibung der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="8cf89-133">Description of the template.</span></span> <span data-ttu-id="8cf89-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8cf89-134">Read-only.</span></span>|
|<span data-ttu-id="8cf89-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8cf89-135">displayName</span></span>|<span data-ttu-id="8cf89-136">string</span><span class="sxs-lookup"><span data-stu-id="8cf89-136">string</span></span>|<span data-ttu-id="8cf89-137">Anzeigename der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="8cf89-137">Display name of the template.</span></span> <span data-ttu-id="8cf89-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8cf89-138">Read-only.</span></span> |
|<span data-ttu-id="8cf89-139">id</span><span class="sxs-lookup"><span data-stu-id="8cf89-139">id</span></span>|<span data-ttu-id="8cf89-140">string</span><span class="sxs-lookup"><span data-stu-id="8cf89-140">string</span></span>| <span data-ttu-id="8cf89-p107">Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8cf89-p107">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="8cf89-143">values</span><span class="sxs-lookup"><span data-stu-id="8cf89-143">values</span></span>|<span data-ttu-id="8cf89-144">[settingTemplateValue](settingtemplatevalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8cf89-144">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="8cf89-145">Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden.</span><span class="sxs-lookup"><span data-stu-id="8cf89-145">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="8cf89-146">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8cf89-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8cf89-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8cf89-147">Relationships</span></span>
<span data-ttu-id="8cf89-148">Keine</span><span class="sxs-lookup"><span data-stu-id="8cf89-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8cf89-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8cf89-149">JSON representation</span></span>

<span data-ttu-id="8cf89-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8cf89-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
