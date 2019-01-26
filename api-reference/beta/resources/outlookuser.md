---
title: outlookUser-Ressourcentyp
description: Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f8265f9da285ce0f52e6201ffdb1298893b86753
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574096"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="16178-103">outlookUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16178-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16178-104">Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.</span><span class="sxs-lookup"><span data-stu-id="16178-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="16178-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="16178-105">Methods</span></span>

| <span data-ttu-id="16178-106">Methode</span><span class="sxs-lookup"><span data-stu-id="16178-106">Method</span></span>           | <span data-ttu-id="16178-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="16178-107">Return Type</span></span>    |<span data-ttu-id="16178-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16178-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16178-109">Kategorie erstellen</span><span class="sxs-lookup"><span data-stu-id="16178-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="16178-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="16178-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="16178-111">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="16178-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="16178-112">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="16178-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="16178-113">[outlookCategory](outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16178-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="16178-114">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="16178-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="16178-115">Erstellen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="16178-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="16178-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="16178-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="16178-117">Erstellen Sie einen Aufgabenordner in der Standardgruppe Aufgabe (`My Tasks`) für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="16178-118">Liste taskFolders</span><span class="sxs-lookup"><span data-stu-id="16178-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="16178-119">[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16178-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="16178-120">Rufen Sie alle Outlook Aufgabenordner im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="16178-121">Erstellen von outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="16178-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="16178-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="16178-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="16178-123">Erstellen eines Outlook-"Task Group" im Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="16178-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="16178-124">Liste taskGroups</span><span class="sxs-lookup"><span data-stu-id="16178-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="16178-125">[OutlookTaskGroup](outlooktaskgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16178-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="16178-126">Rufen Sie die Outlook-Vorgangsgruppen im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="16178-127">Erstellen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="16178-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="16178-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="16178-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="16178-129">Erstellen Sie eine Outlook-Aufgabe in der Standardgruppe Aufgabe (`My Tasks`) und Aufgabe Standardordner (`Tasks`) in das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="16178-130">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="16178-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="16178-131">[OutlookTask](outlooktask.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16178-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="16178-132">Rufen Sie die Outlook-Aufgaben in das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="16178-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="16178-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="16178-134">[localeInfo](localeinfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16178-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="16178-135">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="16178-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="16178-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="16178-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="16178-137">[timeZoneInformation](timezoneinformation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16178-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="16178-138">Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="16178-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="16178-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16178-139">Properties</span></span>
<span data-ttu-id="16178-140">Keine</span><span class="sxs-lookup"><span data-stu-id="16178-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="16178-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16178-141">Relationships</span></span>
| <span data-ttu-id="16178-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="16178-142">Relationship</span></span> | <span data-ttu-id="16178-143">Typ</span><span class="sxs-lookup"><span data-stu-id="16178-143">Type</span></span>   |<span data-ttu-id="16178-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16178-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16178-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="16178-145">masterCategories</span></span>|<span data-ttu-id="16178-146">[outlookCategory](../resources/outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16178-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="16178-147">Eine Liste von Kategorien, die für den Benutzer definiert sind.</span><span class="sxs-lookup"><span data-stu-id="16178-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="16178-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="16178-148">taskFolders</span></span>|<span data-ttu-id="16178-149">[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16178-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="16178-150">Outlook-Aufgabe-Ordner des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-150">The user's Outlook task folders.</span></span> <span data-ttu-id="16178-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16178-151">Read-only.</span></span> <span data-ttu-id="16178-152">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="16178-152">Nullable.</span></span>|
|<span data-ttu-id="16178-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="16178-153">taskGroups</span></span>|<span data-ttu-id="16178-154">[OutlookTaskGroup](outlooktaskgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16178-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="16178-155">Der Benutzer Outlook Vorgangsgruppen.</span><span class="sxs-lookup"><span data-stu-id="16178-155">The user's Outlook task groups.</span></span> <span data-ttu-id="16178-156">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16178-156">Read-only.</span></span> <span data-ttu-id="16178-157">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="16178-157">Nullable.</span></span>|
|<span data-ttu-id="16178-158">tasks</span><span class="sxs-lookup"><span data-stu-id="16178-158">tasks</span></span>|<span data-ttu-id="16178-159">[OutlookTask](outlooktask.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16178-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="16178-160">Outlook-Aufgaben des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16178-160">The user's Outlook tasks.</span></span> <span data-ttu-id="16178-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16178-161">Read-only.</span></span> <span data-ttu-id="16178-162">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="16178-162">Nullable.</span></span>|


<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.outlookUser"
}-->
```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
