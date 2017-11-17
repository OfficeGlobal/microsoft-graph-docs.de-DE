# <a name="onenote-resource-type"></a><span data-ttu-id="85fb4-101">onenote-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85fb4-101">onenote resource type</span></span>

<span data-ttu-id="85fb4-102">Der Einstiegspunkt für OneNote-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="85fb4-102">The entry point for OneNote resources.</span></span>

<span data-ttu-id="85fb4-103">Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="85fb4-103">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="85fb4-104">Speicherort können Benutzernotizbücher in Office 365 oder dem Verbraucher-OneDrive, Gruppennotizbücher oder auf einer SharePoint-Website gehostete Teamnotizbücher in Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="85fb4-104">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="85fb4-105">**Benutzernotizbücher** Verwenden Sie einen der folgenden URLs, um auf persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business zuzugreifen:</span><span class="sxs-lookup"><span data-stu-id="85fb4-105">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="85fb4-106">**Gruppennotizbücher** Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:</span><span class="sxs-lookup"><span data-stu-id="85fb4-106">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="85fb4-107">**SharePoint-Websiten-Notizbücher** VerwendenSie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:</span><span class="sxs-lookup"><span data-stu-id="85fb4-107">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="85fb4-108">Authorization</span><span class="sxs-lookup"><span data-stu-id="85fb4-108">Authorization</span></span>

<span data-ttu-id="85fb4-109">Informationen über die erforderlichen Berechtigungen zum Arbeiten mit OneNote-APIs finden Sie unter [Notizenberechtigungen](../../../concepts/permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="85fb4-109">For information about the permissions required to work with OneNote APIs, see [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="85fb4-110">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="85fb4-110">Relationships</span></span>
| <span data-ttu-id="85fb4-111">Beziehung</span><span class="sxs-lookup"><span data-stu-id="85fb4-111">Relationship</span></span> | <span data-ttu-id="85fb4-112">Typ</span><span class="sxs-lookup"><span data-stu-id="85fb4-112">Type</span></span>   |<span data-ttu-id="85fb4-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85fb4-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85fb4-114">Notizbücher</span><span class="sxs-lookup"><span data-stu-id="85fb4-114">notebooks</span></span>|<span data-ttu-id="85fb4-115">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-115">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="85fb4-p101">Die Sammlung von OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="85fb4-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="85fb4-119">Vorgänge</span><span class="sxs-lookup"><span data-stu-id="85fb4-119">operations</span></span>|<span data-ttu-id="85fb4-120">[Operation](onenoteoperation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-120">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="85fb4-p102">Der Status von OneNote-Vorgängen. Das Abrufen einer operations-Sammlung wird nicht unterstützt, Sie können aber den Status von lange dauernden Vorgängen abrufen, wenn der `Operation-Location`-Header in der Antwort zurückgegeben wird. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="85fb4-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="85fb4-125">Seiten</span><span class="sxs-lookup"><span data-stu-id="85fb4-125">pages</span></span>|<span data-ttu-id="85fb4-126">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-126">[Page](page.md) collection</span></span>|<span data-ttu-id="85fb4-p103">Die Seiten in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="85fb4-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="85fb4-130">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="85fb4-130">resources</span></span>|<span data-ttu-id="85fb4-131">[Ressourcensammlung](resource.md)</span><span class="sxs-lookup"><span data-stu-id="85fb4-131">[Resource](resource.md) collection</span></span> |<span data-ttu-id="85fb4-p104">Das Bild und andere Dateiressourcen in OneNote-Seiten. Das Abrufen einer Ressourcensammlung wird nicht unterstützt, Sie können aber [den binären Inhalt einer bestimmten Ressource abrufen](resource.md). Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="85fb4-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="85fb4-136">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="85fb4-136">sectionGroups</span></span>|<span data-ttu-id="85fb4-137">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-137">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="85fb4-p105">Die Abschnittsgruppen in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="85fb4-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="85fb4-141">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="85fb4-141">sections</span></span>|<span data-ttu-id="85fb4-142">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-142">[Section](section.md) collection</span></span>|<span data-ttu-id="85fb4-p106">Die Abschnitte in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="85fb4-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="85fb4-146">Methoden</span><span class="sxs-lookup"><span data-stu-id="85fb4-146">Methods</span></span>

| <span data-ttu-id="85fb4-147">Methode</span><span class="sxs-lookup"><span data-stu-id="85fb4-147">Method</span></span>           | <span data-ttu-id="85fb4-148">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="85fb4-148">Return Type</span></span>    |<span data-ttu-id="85fb4-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85fb4-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85fb4-150">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="85fb4-150">Create notebook</span></span>](../api/onenote_post_notebooks.md) |[<span data-ttu-id="85fb4-151">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="85fb4-151">Notebook</span></span>](notebook.md)| <span data-ttu-id="85fb4-152">Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="85fb4-152">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="85fb4-153">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="85fb4-153">List notebooks</span></span>](../api/onenote_list_notebooks.md) |<span data-ttu-id="85fb4-154">[Notebook](notebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-154">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="85fb4-155">Dient zum Abrufen einer Sammlung von Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="85fb4-155">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="85fb4-156">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="85fb4-156">Create page</span></span>](../api/onenote_post_pages.md) |[<span data-ttu-id="85fb4-157">Seite</span><span class="sxs-lookup"><span data-stu-id="85fb4-157">Page</span></span>](page.md)| <span data-ttu-id="85fb4-158">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="85fb4-158">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="85fb4-159">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="85fb4-159">List pages</span></span>](../api/onenote_list_pages.md) |<span data-ttu-id="85fb4-160">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-160">[Page](page.md) collection</span></span>| <span data-ttu-id="85fb4-161">Dient zum Abrufen einer Sammlung von Seiten.</span><span class="sxs-lookup"><span data-stu-id="85fb4-161">Get a collection of pages.</span></span>|
|[<span data-ttu-id="85fb4-162">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="85fb4-162">List section groups</span></span>](../api/onenote_list_sectiongroups.md) |<span data-ttu-id="85fb4-163">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-163">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="85fb4-164">Dient zum Abrufen einer Sammlung von Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="85fb4-164">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="85fb4-165">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="85fb4-165">List sections</span></span>](../api/onenote_list_sections.md) |<span data-ttu-id="85fb4-166">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85fb4-166">[Section](section.md) collection</span></span>| <span data-ttu-id="85fb4-167">Dient zum Abrufen einer Sammlung von Abschnitten.</span><span class="sxs-lookup"><span data-stu-id="85fb4-167">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
