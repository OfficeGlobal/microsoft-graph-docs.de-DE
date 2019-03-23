---
title: 'Notizbuch: getNotebookFromWebUrl'
description: Rufen Sie die Eigenschaften und Beziehungen eines Notebook-Objekts mithilfe des URL-Pfads ab.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: b5067f50b1e03c124af8323709fc7b3f70af871b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789648"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="cf126-103">Notizbuch: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="cf126-103">notebook: getNotebookFromWebUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf126-104">Rufen Sie die Eigenschaften und Beziehungen eines [Notebook](../resources/notebook.md) -Objekts mithilfe des URL-Pfads ab.</span><span class="sxs-lookup"><span data-stu-id="cf126-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="cf126-105">Der Speicherort kann Benutzer-Notebooks in Office 365, Gruppen-Notebooks oder von SharePoint-Websites gehostete Team-Notizbücher in Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="cf126-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf126-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf126-106">Permissions</span></span>
<span data-ttu-id="cf126-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf126-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf126-109">Permission type</span></span>      | <span data-ttu-id="cf126-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf126-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf126-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf126-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf126-112">Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. all, Notes. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="cf126-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf126-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf126-113">Application</span></span> | <span data-ttu-id="cf126-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf126-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf126-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf126-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="cf126-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf126-116">Request headers</span></span>
| <span data-ttu-id="cf126-117">Name</span><span class="sxs-lookup"><span data-stu-id="cf126-117">Name</span></span>       | <span data-ttu-id="cf126-118">Typ</span><span class="sxs-lookup"><span data-stu-id="cf126-118">Type</span></span> | <span data-ttu-id="cf126-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf126-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cf126-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf126-120">Authorization</span></span>  | <span data-ttu-id="cf126-121">string</span><span class="sxs-lookup"><span data-stu-id="cf126-121">string</span></span>  | <span data-ttu-id="cf126-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf126-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf126-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cf126-124">Accept</span></span> | <span data-ttu-id="cf126-125">string</span><span class="sxs-lookup"><span data-stu-id="cf126-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cf126-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf126-126">Request body</span></span>
<span data-ttu-id="cf126-127">Geben Sie im Anforderungstext eine JSON-Darstellung des vollständigen URL-Pfads des abzurufenden Notebooks an.</span><span class="sxs-lookup"><span data-stu-id="cf126-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="cf126-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf126-128">Property</span></span>     | <span data-ttu-id="cf126-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cf126-129">Type</span></span>        | <span data-ttu-id="cf126-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf126-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="cf126-131">Der URL-Pfad des abzurufenden Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="cf126-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="cf126-132">Es kann auch ein "OneNote:"-Präfix enthalten.</span><span class="sxs-lookup"><span data-stu-id="cf126-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="cf126-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf126-133">Response</span></span>

<span data-ttu-id="cf126-134">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Notebook](../resources/notebook.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cf126-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf126-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf126-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf126-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf126-136">Request</span></span>
<span data-ttu-id="cf126-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf126-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="cf126-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf126-138">Response</span></span>
<span data-ttu-id="cf126-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf126-139">Here is an example of the response.</span></span> 

><span data-ttu-id="cf126-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cf126-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{notebook-getnotebookfromweburl.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
