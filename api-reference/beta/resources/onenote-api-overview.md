---
title: Verwenden der OneNote-REST-API
description: 'Microsoft Graph können Ihre app autorisierten Zugriff auf eines Benutzers OneNote-Notizbücher, Abschnitte und Seiten in einem persönlichen oder Organisation Konto zu erhalten. Mit der entsprechenden delegiert, oder Berechtigungen für die Anwendung, Ihre app die OneNote-Daten des angemeldeten Benutzers oder jeder Benutzer in einem Mandanten zugreifen können. '
ms.openlocfilehash: 091dd18cbcfae2a4058aff71df14ed7aa5fd7a03
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065799"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="d04c2-104">Verwenden der OneNote-REST-API</span><span class="sxs-lookup"><span data-stu-id="d04c2-104">Use the OneNote REST API</span></span>

> <span data-ttu-id="d04c2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d04c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d04c2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d04c2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d04c2-107">Microsoft Graph können Ihre app autorisierten Zugriff auf eines Benutzers OneNote-Notizbücher, Abschnitte und Seiten in einem persönlichen oder Organisation Konto zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="d04c2-107">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="d04c2-108">Mit den [entsprechenden Berechtigungen für delegierte oder Anwendung](/graph/permissions-reference#notes-permissions)kann Ihre app die OneNote-Daten des angemeldeten Benutzers oder jeder Benutzer in einem Mandanten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d04c2-108">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="d04c2-109">Stamm-URL</span><span class="sxs-lookup"><span data-stu-id="d04c2-109">Root URL</span></span>
<span data-ttu-id="d04c2-110">Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:</span><span class="sxs-lookup"><span data-stu-id="d04c2-110">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="d04c2-111">Die `version` Segment in der URL darstellt, die Version von Microsoft Graph, die Sie verwenden möchten:</span><span class="sxs-lookup"><span data-stu-id="d04c2-111">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="d04c2-112">Setzen Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="d04c2-112">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="d04c2-113">Setzen Sie `beta`, wenn Sie ein Feature testen möchten, das sich noch in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="d04c2-113">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="d04c2-114">Features und Funktionen in der Beta-Endpunkt möglicherweise ändern. Es wird nicht empfohlen, für die Verwendung in Ihrem Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="d04c2-114">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="d04c2-115">Der Speicherort kann Benutzer Notizbücher auf Office 365 oder Consumer OneDrive, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="d04c2-115">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote-API-Entwicklung Stapel](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="d04c2-117">Benutzer-Notizbüchern</span><span class="sxs-lookup"><span data-stu-id="d04c2-117">User notebooks</span></span>
<span data-ttu-id="d04c2-118">Verwenden Sie den Zugriff auf persönliche Notizbücher auf Consumer OneDrive oder OneDrive für Unternehmen eine der folgenden URLs:</span><span class="sxs-lookup"><span data-stu-id="d04c2-118">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="d04c2-119">Setzen Sie `me` für OneNote-Inhalte, auf die der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="d04c2-119">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="d04c2-120">Setzen Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="d04c2-120">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="d04c2-121">Verwenden Sie die [Benutzer](users.md) API.</span><span class="sxs-lookup"><span data-stu-id="d04c2-121">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="d04c2-122">**Hinweis:** Sie können die Benutzer-IDs abrufen, indem Sie tätigen eine GET-Anforderung auf `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="d04c2-122">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="d04c2-123">Gruppe-Notizbüchern</span><span class="sxs-lookup"><span data-stu-id="d04c2-123">Group notebooks</span></span>

<span data-ttu-id="d04c2-124">Um Notizbücher zugreifen, die eine Gruppe gehören, verwenden Sie die folgenden dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="d04c2-124">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="d04c2-125">SharePoint-Website-Notizbüchern</span><span class="sxs-lookup"><span data-stu-id="d04c2-125">SharePoint site notebooks</span></span>
<span data-ttu-id="d04c2-126">Um Notizbücher zugreifen, die SharePoint-Teamwebsite gehören, verwenden Sie die folgenden dienststamm-URL:</span><span class="sxs-lookup"><span data-stu-id="d04c2-126">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
