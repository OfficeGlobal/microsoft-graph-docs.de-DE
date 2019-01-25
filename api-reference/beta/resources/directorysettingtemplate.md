---
title: Ressourcentyp directorySettingTemplate
description: Verzeichnis Einstellung Vorlagen darstellen, die dem Mandanten verfügbaren systemdefinierte Einstellungen. Directory-Einstellungen können anhand der verfügbaren DirectorySettingTemplates und Werte geändert voreingestellten Standardwerte von erstellt werden. Verzeichnis Einstellung Vorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können Mandanten geltende Einstellungen darstellen, oder Sie können bestimmte Entität Einstellungen darstellen.  Derzeit nur verfügbaren Vorlagen gelten für Office-Gruppen und umfassen Einstellungen wie gibt an, ob Benutzer Gruppen erstellen oder Gäste außerhalb der Organisation, die Mitglied einer Gruppe werden einladen können.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516658"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="a69bd-107">Ressourcentyp directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a69bd-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a69bd-108">Verzeichnis Einstellung Vorlagen darstellen, die dem Mandanten verfügbaren systemdefinierte Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a69bd-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="a69bd-109">[Directory-Einstellungen](directorysetting.md) können anhand der verfügbaren DirectorySettingTemplates und Werte geändert voreingestellten Standardwerte von erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="a69bd-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="a69bd-110">Verzeichnis Einstellung Vorlagen können nicht erstellt, aktualisiert oder gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="a69bd-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="a69bd-111">Diese Einstellungen können Mandanten geltende Einstellungen darstellen, oder Sie können bestimmte Entität Einstellungen darstellen.</span><span class="sxs-lookup"><span data-stu-id="a69bd-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="a69bd-112">Derzeit nur verfügbaren Vorlagen gelten für Office-Gruppen und umfassen Einstellungen wie gibt an, ob Benutzer Gruppen erstellen oder Gäste außerhalb der Organisation, die Mitglied einer Gruppe werden einladen können.</span><span class="sxs-lookup"><span data-stu-id="a69bd-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="a69bd-113">**Hinweis**: die /beta Version von dem Ressourcentyp DirectorySettingTemplate gilt nur für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="a69bd-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="a69bd-114">Die Version /v1.0 wurde in GroupSettingTemplate umbenannt.</span><span class="sxs-lookup"><span data-stu-id="a69bd-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="a69bd-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="a69bd-115">Methods</span></span>

| <span data-ttu-id="a69bd-116">Methode</span><span class="sxs-lookup"><span data-stu-id="a69bd-116">Method</span></span>           | <span data-ttu-id="a69bd-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a69bd-117">Return Type</span></span>    |<span data-ttu-id="a69bd-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a69bd-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a69bd-119">Abrufen von directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a69bd-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="a69bd-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a69bd-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="a69bd-121">Lesen Sie die spezifischen Eigenschaften der eines der Objekte DirectorySettingTemplate System definiert.</span><span class="sxs-lookup"><span data-stu-id="a69bd-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="a69bd-122">Liste directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a69bd-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="a69bd-123">Auflistung von directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a69bd-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="a69bd-124">Listen Sie aller vom System definierten DirectorySettingTemplate Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="a69bd-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="a69bd-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a69bd-125">Properties</span></span>
| <span data-ttu-id="a69bd-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a69bd-126">Property</span></span>     | <span data-ttu-id="a69bd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a69bd-127">Type</span></span>   |<span data-ttu-id="a69bd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a69bd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a69bd-129">description</span><span class="sxs-lookup"><span data-stu-id="a69bd-129">description</span></span>|<span data-ttu-id="a69bd-130">string</span><span class="sxs-lookup"><span data-stu-id="a69bd-130">string</span></span>|<span data-ttu-id="a69bd-131">Beschreibung der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="a69bd-131">Description of the template.</span></span> <span data-ttu-id="a69bd-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a69bd-132">Read-only.</span></span>|
|<span data-ttu-id="a69bd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a69bd-133">displayName</span></span>|<span data-ttu-id="a69bd-134">string</span><span class="sxs-lookup"><span data-stu-id="a69bd-134">string</span></span>|<span data-ttu-id="a69bd-135">Anzeigename der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="a69bd-135">Display name of the template.</span></span> <span data-ttu-id="a69bd-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a69bd-136">Read-only.</span></span> |
|<span data-ttu-id="a69bd-137">id</span><span class="sxs-lookup"><span data-stu-id="a69bd-137">id</span></span>|<span data-ttu-id="a69bd-138">string</span><span class="sxs-lookup"><span data-stu-id="a69bd-138">string</span></span>| <span data-ttu-id="a69bd-p106">Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a69bd-p106">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="a69bd-141">values</span><span class="sxs-lookup"><span data-stu-id="a69bd-141">values</span></span>|<span data-ttu-id="a69bd-142">[settingTemplateValue](settingtemplatevalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a69bd-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="a69bd-143">Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden.</span><span class="sxs-lookup"><span data-stu-id="a69bd-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="a69bd-144">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a69bd-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a69bd-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a69bd-145">Relationships</span></span>
<span data-ttu-id="a69bd-146">Keine</span><span class="sxs-lookup"><span data-stu-id="a69bd-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a69bd-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a69bd-147">JSON representation</span></span>

<span data-ttu-id="a69bd-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a69bd-148">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
