---
title: 'Notizbuch: GetNotebookFromWebUrl'
description: Abrufen der Eigenschaften und die Beziehungen eines Notebook-Objekts verwenden den URL-Pfad.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 226cbd70343feaf8fe5404aac6077f9b2438aba8
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982069"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="c4d0c-103">Notizbuch: GetNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="c4d0c-103">notebook: getNotebookFromWebUrl</span></span>

[! Beta-Haftungsausschluss INCLUDE]

<span data-ttu-id="c4d0c-105">Rufen Sie die Eigenschaften und die Beziehungen eines [Notebook](../resources/notebook.md) -Objekts mithilfe von den URL-Pfad ab.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="c4d0c-106">Der Speicherort kann Benutzer Notizbücher auf Office 365, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-106">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4d0c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c4d0c-107">Permissions</span></span>
<span data-ttu-id="c4d0c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4d0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4d0c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c4d0c-110">Permission type</span></span>      | <span data-ttu-id="c4d0c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c4d0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4d0c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c4d0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4d0c-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d0c-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4d0c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c4d0c-114">Application</span></span> | <span data-ttu-id="c4d0c-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d0c-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4d0c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4d0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="c4d0c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4d0c-117">Request headers</span></span>
| <span data-ttu-id="c4d0c-118">Name</span><span class="sxs-lookup"><span data-stu-id="c4d0c-118">Name</span></span>       | <span data-ttu-id="c4d0c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c4d0c-119">Type</span></span> | <span data-ttu-id="c4d0c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4d0c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c4d0c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4d0c-121">Authorization</span></span>  | <span data-ttu-id="c4d0c-122">string</span><span class="sxs-lookup"><span data-stu-id="c4d0c-122">string</span></span>  | <span data-ttu-id="c4d0c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4d0c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c4d0c-125">Accept</span></span> | <span data-ttu-id="c4d0c-126">string</span><span class="sxs-lookup"><span data-stu-id="c4d0c-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c4d0c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4d0c-127">Request body</span></span>
<span data-ttu-id="c4d0c-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der vollständige URL-Pfad zum Notizbuch, den, das Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="c4d0c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4d0c-129">Property</span></span>     | <span data-ttu-id="c4d0c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c4d0c-130">Type</span></span>        | <span data-ttu-id="c4d0c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4d0c-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="c4d0c-132">Der URL-Pfad des Notizbuchs abgerufen.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="c4d0c-133">Es kann auch enthalten eine "Onenote:" Präfix.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="c4d0c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4d0c-134">Response</span></span>

<span data-ttu-id="c4d0c-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4d0c-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c4d0c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4d0c-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4d0c-137">Request</span></span>
<span data-ttu-id="c4d0c-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="c4d0c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4d0c-139">Response</span></span>
<span data-ttu-id="c4d0c-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-140">Here is an example of the response.</span></span> 

><span data-ttu-id="c4d0c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c4d0c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
