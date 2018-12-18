---
title: onenote-Ressourcentyp
description: Der Einstiegspunkt für OneNote-Ressourcen.
author: Jewan-microsoft
ms.openlocfilehash: b145dc36c761d1f389b28454b9900305ac259809
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323632"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="6e886-103">onenote-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6e886-103">onenote resource type</span></span>

> <span data-ttu-id="6e886-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6e886-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e886-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e886-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e886-106">Der Einstiegspunkt für OneNote-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="6e886-106">The entry point for OneNote resources.</span></span>

<span data-ttu-id="6e886-107">Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="6e886-107">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="6e886-108">Der Speicherort kann Benutzer Notizbücher auf Office 365 oder Consumer OneDrive, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="6e886-108">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="6e886-109">**Benutzernotizbücher** Verwenden Sie einen der folgenden URLs, um auf persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business zuzugreifen:</span><span class="sxs-lookup"><span data-stu-id="6e886-109">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="6e886-110">**Gruppennotizbücher** Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:</span><span class="sxs-lookup"><span data-stu-id="6e886-110">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="6e886-111">**SharePoint-Websiten-Notizbücher** VerwendenSie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:</span><span class="sxs-lookup"><span data-stu-id="6e886-111">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="6e886-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e886-112">Authorization</span></span>

<span data-ttu-id="6e886-113">Informationen über die erforderlichen Berechtigungen zum Arbeiten mit OneNote-APIs finden Sie unter [Notizenberechtigungen](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="6e886-113">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="6e886-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6e886-114">Relationships</span></span>
| <span data-ttu-id="6e886-115">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6e886-115">Relationship</span></span> | <span data-ttu-id="6e886-116">Typ</span><span class="sxs-lookup"><span data-stu-id="6e886-116">Type</span></span>   |<span data-ttu-id="6e886-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e886-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e886-118">Notizbücher</span><span class="sxs-lookup"><span data-stu-id="6e886-118">notebooks</span></span>|<span data-ttu-id="6e886-119">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-119">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="6e886-p102">Die Sammlung von OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6e886-p102">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6e886-123">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="6e886-123">operations</span></span>|<span data-ttu-id="6e886-124">[Operation](onenoteoperation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-124">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="6e886-p103">Der Status von OneNote-Vorgängen. Das Abrufen einer operations-Sammlung wird nicht unterstützt, Sie können aber den Status von lange dauernden Vorgängen abrufen, wenn der `Operation-Location`-Header in der Antwort zurückgegeben wird. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6e886-p103">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6e886-129">Seiten</span><span class="sxs-lookup"><span data-stu-id="6e886-129">pages</span></span>|<span data-ttu-id="6e886-130">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-130">[Page](page.md) collection</span></span>|<span data-ttu-id="6e886-p104">Die Seiten in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6e886-p104">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6e886-134">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6e886-134">resources</span></span>|<span data-ttu-id="6e886-135">[Ressourcensammlung](resource.md)</span><span class="sxs-lookup"><span data-stu-id="6e886-135">[Resource](resource.md) collection</span></span> |<span data-ttu-id="6e886-p105">Das Bild und andere Dateiressourcen in OneNote-Seiten. Das Abrufen einer Ressourcensammlung wird nicht unterstützt, Sie können aber [den binären Inhalt einer bestimmten Ressource abrufen](resource.md). Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6e886-p105">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="6e886-140">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6e886-140">sectionGroups</span></span>|<span data-ttu-id="6e886-141">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-141">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6e886-p106">Die Abschnittsgruppen in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6e886-p106">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6e886-145">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="6e886-145">sections</span></span>|<span data-ttu-id="6e886-146">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-146">[Section](section.md) collection</span></span>|<span data-ttu-id="6e886-p107">Die Abschnitte in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6e886-p107">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6e886-150">Methoden</span><span class="sxs-lookup"><span data-stu-id="6e886-150">Methods</span></span>

| <span data-ttu-id="6e886-151">Methode</span><span class="sxs-lookup"><span data-stu-id="6e886-151">Method</span></span>           | <span data-ttu-id="6e886-152">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6e886-152">Return Type</span></span>    |<span data-ttu-id="6e886-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e886-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e886-154">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="6e886-154">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="6e886-155">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="6e886-155">Notebook</span></span>](notebook.md)| <span data-ttu-id="6e886-156">Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6e886-156">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="6e886-157">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="6e886-157">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="6e886-158">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-158">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="6e886-159">Dient zum Abrufen einer Sammlung von Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="6e886-159">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="6e886-160">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="6e886-160">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="6e886-161">Seite</span><span class="sxs-lookup"><span data-stu-id="6e886-161">Page</span></span>](page.md)| <span data-ttu-id="6e886-162">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6e886-162">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="6e886-163">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="6e886-163">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="6e886-164">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-164">[Page](page.md) collection</span></span>| <span data-ttu-id="6e886-165">Dient zum Abrufen einer Sammlung von Seiten.</span><span class="sxs-lookup"><span data-stu-id="6e886-165">Get a collection of pages.</span></span>|
|[<span data-ttu-id="6e886-166">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="6e886-166">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="6e886-167">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-167">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6e886-168">Dient zum Abrufen einer Sammlung von Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="6e886-168">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="6e886-169">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="6e886-169">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="6e886-170">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6e886-170">[Section](section.md) collection</span></span>| <span data-ttu-id="6e886-171">Dient zum Abrufen einer Sammlung von Abschnitten.</span><span class="sxs-lookup"><span data-stu-id="6e886-171">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
