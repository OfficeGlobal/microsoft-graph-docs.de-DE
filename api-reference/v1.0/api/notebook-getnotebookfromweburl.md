---
title: 'Notizbuch: GetNotebookFromWebUrl'
description: Abrufen der Eigenschaften und die Beziehungen eines Notebook-Objekts verwenden den URL-Pfad.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3d14edf5a8992f9f4386e4b50aa74d54986b62f1
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982062"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="cc47d-103">Notizbuch: GetNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="cc47d-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="cc47d-104">Rufen Sie die Eigenschaften und die Beziehungen eines [Notebook](../resources/notebook.md) -Objekts mithilfe von den URL-Pfad ab.</span><span class="sxs-lookup"><span data-stu-id="cc47d-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="cc47d-105">Der Speicherort kann Benutzer Notizbücher auf Office 365, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein.</span><span class="sxs-lookup"><span data-stu-id="cc47d-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc47d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cc47d-106">Permissions</span></span>
<span data-ttu-id="cc47d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc47d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc47d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cc47d-109">Permission type</span></span>      | <span data-ttu-id="cc47d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cc47d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc47d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cc47d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc47d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc47d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc47d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cc47d-113">Application</span></span> | <span data-ttu-id="cc47d-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc47d-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc47d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc47d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="cc47d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cc47d-116">Request headers</span></span>
| <span data-ttu-id="cc47d-117">Name</span><span class="sxs-lookup"><span data-stu-id="cc47d-117">Name</span></span>       | <span data-ttu-id="cc47d-118">Typ</span><span class="sxs-lookup"><span data-stu-id="cc47d-118">Type</span></span> | <span data-ttu-id="cc47d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc47d-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cc47d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc47d-120">Authorization</span></span>  | <span data-ttu-id="cc47d-121">string</span><span class="sxs-lookup"><span data-stu-id="cc47d-121">string</span></span>  | <span data-ttu-id="cc47d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cc47d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc47d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cc47d-124">Accept</span></span> | <span data-ttu-id="cc47d-125">string</span><span class="sxs-lookup"><span data-stu-id="cc47d-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cc47d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cc47d-126">Request body</span></span>
<span data-ttu-id="cc47d-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der vollständige URL-Pfad zum Notizbuch, den, das Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="cc47d-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="cc47d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cc47d-128">Property</span></span>     | <span data-ttu-id="cc47d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cc47d-129">Type</span></span>        | <span data-ttu-id="cc47d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc47d-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="cc47d-131">Der URL-Pfad des Notizbuchs abgerufen.</span><span class="sxs-lookup"><span data-stu-id="cc47d-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="cc47d-132">Es kann auch enthalten eine "Onenote:" Präfix.</span><span class="sxs-lookup"><span data-stu-id="cc47d-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="cc47d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc47d-133">Response</span></span>

<span data-ttu-id="cc47d-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc47d-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc47d-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cc47d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc47d-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc47d-136">Request</span></span>
<span data-ttu-id="cc47d-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cc47d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="cc47d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc47d-138">Response</span></span>
<span data-ttu-id="cc47d-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cc47d-139">Here is an example of the response.</span></span> 

><span data-ttu-id="cc47d-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cc47d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
