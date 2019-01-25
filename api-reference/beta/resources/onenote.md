---
title: onenote-Ressourcentyp
description: Der Einstiegspunkt für OneNote-Ressourcen.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508727"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="616cd-103">onenote-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="616cd-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="616cd-104">Der Einstiegspunkt für OneNote-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="616cd-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="616cd-105">Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="616cd-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="616cd-106">Der Speicherort kann Benutzer Notizbücher auf Office 365 oder Consumer OneDrive, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="616cd-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="616cd-107">**Benutzernotizbücher** Verwenden Sie einen der folgenden URLs, um auf persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business zuzugreifen:</span><span class="sxs-lookup"><span data-stu-id="616cd-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="616cd-108">**Gruppennotizbücher** Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:</span><span class="sxs-lookup"><span data-stu-id="616cd-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="616cd-109">**SharePoint-Websiten-Notizbücher** VerwendenSie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:</span><span class="sxs-lookup"><span data-stu-id="616cd-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="616cd-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="616cd-110">Authorization</span></span>

<span data-ttu-id="616cd-111">Informationen über die erforderlichen Berechtigungen zum Arbeiten mit OneNote-APIs finden Sie unter [Notizenberechtigungen](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="616cd-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="616cd-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="616cd-112">Relationships</span></span>
| <span data-ttu-id="616cd-113">Beziehung</span><span class="sxs-lookup"><span data-stu-id="616cd-113">Relationship</span></span> | <span data-ttu-id="616cd-114">Typ</span><span class="sxs-lookup"><span data-stu-id="616cd-114">Type</span></span>   |<span data-ttu-id="616cd-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="616cd-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="616cd-116">Notizbücher</span><span class="sxs-lookup"><span data-stu-id="616cd-116">notebooks</span></span>|<span data-ttu-id="616cd-117">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="616cd-p101">Die Sammlung von OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="616cd-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="616cd-121">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="616cd-121">operations</span></span>|<span data-ttu-id="616cd-122">[Operation](onenoteoperation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="616cd-p102">Der Status von OneNote-Vorgängen. Das Abrufen einer operations-Sammlung wird nicht unterstützt, Sie können aber den Status von lange dauernden Vorgängen abrufen, wenn der `Operation-Location`-Header in der Antwort zurückgegeben wird. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="616cd-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="616cd-127">Seiten</span><span class="sxs-lookup"><span data-stu-id="616cd-127">pages</span></span>|<span data-ttu-id="616cd-128">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-128">[Page](page.md) collection</span></span>|<span data-ttu-id="616cd-p103">Die Seiten in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="616cd-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="616cd-132">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="616cd-132">resources</span></span>|<span data-ttu-id="616cd-133">[Ressourcensammlung](resource.md)</span><span class="sxs-lookup"><span data-stu-id="616cd-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="616cd-p104">Das Bild und andere Dateiressourcen in OneNote-Seiten. Das Abrufen einer Ressourcensammlung wird nicht unterstützt, Sie können aber [den binären Inhalt einer bestimmten Ressource abrufen](resource.md). Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="616cd-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="616cd-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="616cd-138">sectionGroups</span></span>|<span data-ttu-id="616cd-139">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="616cd-p105">Die Abschnittsgruppen in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="616cd-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="616cd-143">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="616cd-143">sections</span></span>|<span data-ttu-id="616cd-144">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-144">[Section](section.md) collection</span></span>|<span data-ttu-id="616cd-p106">Die Abschnitte in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="616cd-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="616cd-148">Methoden</span><span class="sxs-lookup"><span data-stu-id="616cd-148">Methods</span></span>

| <span data-ttu-id="616cd-149">Methode</span><span class="sxs-lookup"><span data-stu-id="616cd-149">Method</span></span>           | <span data-ttu-id="616cd-150">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="616cd-150">Return Type</span></span>    |<span data-ttu-id="616cd-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="616cd-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="616cd-152">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="616cd-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="616cd-153">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="616cd-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="616cd-154">Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="616cd-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="616cd-155">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="616cd-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="616cd-156">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="616cd-157">Dient zum Abrufen einer Sammlung von Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="616cd-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="616cd-158">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="616cd-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="616cd-159">Seite</span><span class="sxs-lookup"><span data-stu-id="616cd-159">Page</span></span>](page.md)| <span data-ttu-id="616cd-160">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="616cd-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="616cd-161">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="616cd-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="616cd-162">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-162">[Page](page.md) collection</span></span>| <span data-ttu-id="616cd-163">Dient zum Abrufen einer Sammlung von Seiten.</span><span class="sxs-lookup"><span data-stu-id="616cd-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="616cd-164">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="616cd-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="616cd-165">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="616cd-166">Dient zum Abrufen einer Sammlung von Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="616cd-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="616cd-167">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="616cd-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="616cd-168">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="616cd-168">[Section](section.md) collection</span></span>| <span data-ttu-id="616cd-169">Dient zum Abrufen einer Sammlung von Abschnitten.</span><span class="sxs-lookup"><span data-stu-id="616cd-169">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
