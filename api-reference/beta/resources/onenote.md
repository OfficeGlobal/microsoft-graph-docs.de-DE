---
title: onenote-Ressourcentyp
description: Der Einstiegspunkt für OneNote-Ressourcen.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7f282147912f5d73d2aa1655055a763c0cec3764
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878015"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="6f26d-103">onenote-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6f26d-103">onenote resource type</span></span>

> <span data-ttu-id="6f26d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f26d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f26d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f26d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f26d-106">Der Einstiegspunkt für OneNote-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="6f26d-106">The entry point for OneNote resources.</span></span>

<span data-ttu-id="6f26d-107">Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="6f26d-107">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="6f26d-108">Der Speicherort kann Benutzer Notizbücher auf Office 365 oder Consumer OneDrive, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="6f26d-108">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="6f26d-109">**Benutzernotizbücher** Verwenden Sie einen der folgenden URLs, um auf persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business zuzugreifen:</span><span class="sxs-lookup"><span data-stu-id="6f26d-109">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="6f26d-110">**Gruppennotizbücher** Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:</span><span class="sxs-lookup"><span data-stu-id="6f26d-110">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="6f26d-111">**SharePoint-Websiten-Notizbücher** VerwendenSie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:</span><span class="sxs-lookup"><span data-stu-id="6f26d-111">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="6f26d-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f26d-112">Authorization</span></span>

<span data-ttu-id="6f26d-113">Informationen über die erforderlichen Berechtigungen zum Arbeiten mit OneNote-APIs finden Sie unter [Notizenberechtigungen](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="6f26d-113">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="6f26d-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6f26d-114">Relationships</span></span>
| <span data-ttu-id="6f26d-115">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6f26d-115">Relationship</span></span> | <span data-ttu-id="6f26d-116">Typ</span><span class="sxs-lookup"><span data-stu-id="6f26d-116">Type</span></span>   |<span data-ttu-id="6f26d-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f26d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f26d-118">Notizbücher</span><span class="sxs-lookup"><span data-stu-id="6f26d-118">notebooks</span></span>|<span data-ttu-id="6f26d-119">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-119">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="6f26d-p102">Die Sammlung von OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f26d-p102">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f26d-123">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="6f26d-123">operations</span></span>|<span data-ttu-id="6f26d-124">[Operation](onenoteoperation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-124">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="6f26d-p103">Der Status von OneNote-Vorgängen. Das Abrufen einer operations-Sammlung wird nicht unterstützt, Sie können aber den Status von lange dauernden Vorgängen abrufen, wenn der `Operation-Location`-Header in der Antwort zurückgegeben wird. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f26d-p103">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f26d-129">Seiten</span><span class="sxs-lookup"><span data-stu-id="6f26d-129">pages</span></span>|<span data-ttu-id="6f26d-130">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-130">[Page](page.md) collection</span></span>|<span data-ttu-id="6f26d-p104">Die Seiten in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f26d-p104">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f26d-134">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6f26d-134">resources</span></span>|<span data-ttu-id="6f26d-135">[Ressourcensammlung](resource.md)</span><span class="sxs-lookup"><span data-stu-id="6f26d-135">[Resource](resource.md) collection</span></span> |<span data-ttu-id="6f26d-p105">Das Bild und andere Dateiressourcen in OneNote-Seiten. Das Abrufen einer Ressourcensammlung wird nicht unterstützt, Sie können aber [den binären Inhalt einer bestimmten Ressource abrufen](resource.md). Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f26d-p105">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f26d-140">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6f26d-140">sectionGroups</span></span>|<span data-ttu-id="6f26d-141">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-141">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6f26d-p106">Die Abschnittsgruppen in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f26d-p106">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f26d-145">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="6f26d-145">sections</span></span>|<span data-ttu-id="6f26d-146">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-146">[Section](section.md) collection</span></span>|<span data-ttu-id="6f26d-p107">Die Abschnitte in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f26d-p107">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6f26d-150">Methoden</span><span class="sxs-lookup"><span data-stu-id="6f26d-150">Methods</span></span>

| <span data-ttu-id="6f26d-151">Methode</span><span class="sxs-lookup"><span data-stu-id="6f26d-151">Method</span></span>           | <span data-ttu-id="6f26d-152">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6f26d-152">Return Type</span></span>    |<span data-ttu-id="6f26d-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f26d-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f26d-154">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="6f26d-154">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="6f26d-155">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="6f26d-155">Notebook</span></span>](notebook.md)| <span data-ttu-id="6f26d-156">Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6f26d-156">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="6f26d-157">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="6f26d-157">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="6f26d-158">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-158">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="6f26d-159">Dient zum Abrufen einer Sammlung von Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="6f26d-159">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="6f26d-160">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="6f26d-160">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="6f26d-161">Seite</span><span class="sxs-lookup"><span data-stu-id="6f26d-161">Page</span></span>](page.md)| <span data-ttu-id="6f26d-162">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6f26d-162">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="6f26d-163">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="6f26d-163">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="6f26d-164">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-164">[Page](page.md) collection</span></span>| <span data-ttu-id="6f26d-165">Dient zum Abrufen einer Sammlung von Seiten.</span><span class="sxs-lookup"><span data-stu-id="6f26d-165">Get a collection of pages.</span></span>|
|[<span data-ttu-id="6f26d-166">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="6f26d-166">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="6f26d-167">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-167">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6f26d-168">Dient zum Abrufen einer Sammlung von Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="6f26d-168">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="6f26d-169">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="6f26d-169">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="6f26d-170">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f26d-170">[Section](section.md) collection</span></span>| <span data-ttu-id="6f26d-171">Dient zum Abrufen einer Sammlung von Abschnitten.</span><span class="sxs-lookup"><span data-stu-id="6f26d-171">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
