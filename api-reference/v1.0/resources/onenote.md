---
title: onenote-Ressourcentyp
description: Der Einstiegspunkt für OneNote-Ressourcen.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 8240336bfcb9e45e33172c2c1551b71a65c315e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982351"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="6319f-103">onenote-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6319f-103">onenote resource type</span></span>

<span data-ttu-id="6319f-104">Der Einstiegspunkt für OneNote-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="6319f-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="6319f-105">Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="6319f-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="6319f-106">Speicherort können Benutzernotizbücher in Office 365 oder dem Verbraucher-OneDrive, Gruppennotizbücher oder auf einer SharePoint-Website gehostete Teamnotizbücher in Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="6319f-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="6319f-107">**Benutzernotizbücher** Verwenden Sie einen der folgenden URLs, um auf persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business zuzugreifen:</span><span class="sxs-lookup"><span data-stu-id="6319f-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="6319f-108">**Gruppennotizbücher** Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:</span><span class="sxs-lookup"><span data-stu-id="6319f-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="6319f-109">**SharePoint-Websiten-Notizbücher** VerwendenSie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:</span><span class="sxs-lookup"><span data-stu-id="6319f-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="6319f-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="6319f-110">Authorization</span></span>

<span data-ttu-id="6319f-111">Informationen über die erforderlichen Berechtigungen zum Arbeiten mit OneNote-APIs finden Sie unter [Notizenberechtigungen](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="6319f-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="6319f-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6319f-112">Relationships</span></span>
| <span data-ttu-id="6319f-113">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6319f-113">Relationship</span></span> | <span data-ttu-id="6319f-114">Typ</span><span class="sxs-lookup"><span data-stu-id="6319f-114">Type</span></span>   |<span data-ttu-id="6319f-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6319f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6319f-116">Notizbücher</span><span class="sxs-lookup"><span data-stu-id="6319f-116">notebooks</span></span>|<span data-ttu-id="6319f-117">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6319f-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="6319f-p101">Die Sammlung von OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6319f-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6319f-121">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="6319f-121">operations</span></span>|<span data-ttu-id="6319f-122">[OnenoteOperation](onenoteoperation.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6319f-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="6319f-p102">Der Status von OneNote-Vorgängen. Das Abrufen einer operations-Sammlung wird nicht unterstützt, Sie können aber den Status von lange dauernden Vorgängen abrufen, wenn der `Operation-Location`-Header in der Antwort zurückgegeben wird. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6319f-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6319f-127">Seiten</span><span class="sxs-lookup"><span data-stu-id="6319f-127">pages</span></span>|<span data-ttu-id="6319f-128">[OnenotePage](page.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6319f-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="6319f-p103">Die Seiten in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6319f-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6319f-132">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6319f-132">resources</span></span>|<span data-ttu-id="6319f-133">[OnenoteResource](resource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6319f-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="6319f-p104">Das Bild und andere Dateiressourcen in OneNote-Seiten. Das Abrufen einer Ressourcensammlung wird nicht unterstützt, Sie können aber [den binären Inhalt einer bestimmten Ressource abrufen](resource.md). Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6319f-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="6319f-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6319f-138">sectionGroups</span></span>|<span data-ttu-id="6319f-139">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6319f-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6319f-p105">Die Abschnittsgruppen in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6319f-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6319f-143">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="6319f-143">sections</span></span>|<span data-ttu-id="6319f-144">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6319f-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="6319f-p106">Die Abschnitte in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6319f-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6319f-148">Methoden</span><span class="sxs-lookup"><span data-stu-id="6319f-148">Methods</span></span>

| <span data-ttu-id="6319f-149">Methode</span><span class="sxs-lookup"><span data-stu-id="6319f-149">Method</span></span>           | <span data-ttu-id="6319f-150">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6319f-150">Return Type</span></span>    |<span data-ttu-id="6319f-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6319f-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6319f-152">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="6319f-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="6319f-153">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="6319f-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="6319f-154">Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6319f-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="6319f-155">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="6319f-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="6319f-156">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6319f-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="6319f-157">Dient zum Abrufen einer Sammlung von Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="6319f-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="6319f-158">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="6319f-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="6319f-159">Seite</span><span class="sxs-lookup"><span data-stu-id="6319f-159">Page</span></span>](page.md)| <span data-ttu-id="6319f-160">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6319f-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="6319f-161">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="6319f-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="6319f-162">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6319f-162">[Page](page.md) collection</span></span>| <span data-ttu-id="6319f-163">Dient zum Abrufen einer Sammlung von Seiten.</span><span class="sxs-lookup"><span data-stu-id="6319f-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="6319f-164">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="6319f-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="6319f-165">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6319f-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6319f-166">Dient zum Abrufen einer Sammlung von Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="6319f-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="6319f-167">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="6319f-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="6319f-168">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6319f-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="6319f-169">Dient zum Abrufen einer Sammlung von Abschnitten.</span><span class="sxs-lookup"><span data-stu-id="6319f-169">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6319f-170">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6319f-170">JSON Representation</span></span>
<span data-ttu-id="6319f-171">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6319f-171">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
