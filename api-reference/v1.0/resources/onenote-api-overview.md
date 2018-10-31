# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="c1106-101">Verwenden der OneNote-REST-API</span><span class="sxs-lookup"><span data-stu-id="c1106-101">Use the OneNote REST API</span></span>

<span data-ttu-id="c1106-102">Mit Microsoft Graph erhält Ihre App autorisierten Zugriff auf die OneNote-Notizbücher, Abschnitte und Seiten eines Benutzers in einem persönlichen oder Organisationskonto.</span><span class="sxs-lookup"><span data-stu-id="c1106-102">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="c1106-103">Mit den [entsprechenden Berechtigungen für delegierte oder Anwendungsberechtigungen](../../../concepts/permissions_reference.md#notes-permissions) kann Ihre App auf die OneNote-Daten des angemeldeten Benutzers oder jedes Benutzers in einem Mandanten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="c1106-103">With the [appropriate delegated or application permissions](../../../concepts/permissions_reference.md#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span>

## <a name="root-url"></a><span data-ttu-id="c1106-104">Stamm-URL</span><span class="sxs-lookup"><span data-stu-id="c1106-104">Root URL</span></span>
<span data-ttu-id="c1106-105">Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:</span><span class="sxs-lookup"><span data-stu-id="c1106-105">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
<span data-ttu-id="c1106-106">Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll:</span><span class="sxs-lookup"><span data-stu-id="c1106-106">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>

- <span data-ttu-id="c1106-107">`v1.0` ist für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="c1106-107">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="c1106-108">`beta` |||UNTRANSLATED_CONTENT_START|||is to try out a feature that's in development.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="c1106-108">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="c1106-109">Funktionen und Funktionalität in der Betaversion ändern sich möglicherweise, sodass Sie diese nicht in Ihrem Produktionscode verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="c1106-109">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="c1106-110">Speicherort können Benutzernotizbücher in Office 365 oder dem Verbraucher-OneDrive, Gruppennotizbücher oder auf einer SharePoint-Website gehostete Teamnotizbücher in Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="c1106-110">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote-API-Entwicklungsstapel](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="c1106-112">Benutzer-Notizbücher</span><span class="sxs-lookup"><span data-stu-id="c1106-112">User notebooks</span></span>
<span data-ttu-id="c1106-113">Verwenden Sie eine der folgenden URLs, um auf persönliche Notizbücher in Consumer-OneDrive oder in OneDrive for Business zuzugreifen:</span><span class="sxs-lookup"><span data-stu-id="c1106-113">User notebooks To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="c1106-114">`me` |||UNTRANSLATED_CONTENT_START|||is for OneNote content that the current user can access (owned and shared).|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="c1106-114">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="c1106-115">`users/{id}` |||UNTRANSLATED_CONTENT_START|||is for OneNote content that the specified user (in the URL) has shared with the current user.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="c1106-115">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c1106-116">Verwenden Sie die [Benutzer](users.md)-API.</span><span class="sxs-lookup"><span data-stu-id="c1106-116">[Use the Planner API](users.md)</span></span>
> <span data-ttu-id="c1106-117">**Hinweis:** Benutzer-IDs können Sie über eine GET-Anforderung an `https://graph.microsoft.com/v1.0/users` abrufen.</span><span class="sxs-lookup"><span data-stu-id="c1106-117">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="c1106-118">Gruppen-Notizbücher</span><span class="sxs-lookup"><span data-stu-id="c1106-118">Group notebooks</span></span>
<span data-ttu-id="c1106-119">Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:</span><span class="sxs-lookup"><span data-stu-id="c1106-119">Group notebooks To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="c1106-120">SharePoint Website-Notebooks</span><span class="sxs-lookup"><span data-stu-id="c1106-120">SharePoint site notebooks</span></span>

<span data-ttu-id="c1106-121">Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:</span><span class="sxs-lookup"><span data-stu-id="c1106-121">SharePoint site notebooks To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

