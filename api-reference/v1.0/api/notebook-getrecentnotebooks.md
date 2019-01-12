---
title: 'notebook: getRecentNotebooks'
description: Rufen Sie eine Liste der recentNotebook-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 31f95d8e94ef22c6b0cbea1cbb5ff8b98c58d187
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931671"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="0f72e-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="0f72e-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="0f72e-104">Rufen Sie eine Liste der [recentNotebook](../resources/recentnotebook.md)-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="0f72e-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f72e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f72e-105">Permissions</span></span>
<span data-ttu-id="0f72e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f72e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f72e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f72e-108">Permission type</span></span>      | <span data-ttu-id="0f72e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f72e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f72e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f72e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f72e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="0f72e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="0f72e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f72e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f72e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f72e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="0f72e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f72e-114">Application</span></span> | <span data-ttu-id="0f72e-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f72e-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f72e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f72e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="0f72e-117">Der `<id | userPrincipalName>` für den Benutzer muss mit dem im Autorisierungstoken (zur Erstellung der Anforderung verwendet) codierten Benutzer übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="0f72e-117">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="0f72e-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0f72e-118">Function parameters</span></span>

| <span data-ttu-id="0f72e-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="0f72e-119">Parameter</span></span>    | <span data-ttu-id="0f72e-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0f72e-120">Type</span></span>   |<span data-ttu-id="0f72e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f72e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f72e-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="0f72e-122">includePersonalNotebooks</span></span>|<span data-ttu-id="0f72e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f72e-123">Boolean</span></span>|<span data-ttu-id="0f72e-124">Schließen Sie Notizbücher ein, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="0f72e-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="0f72e-125">Wählen Sie `true`, um Notizbücher einzuschließen, die dem Benutzer gehören; wählen Sie andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="0f72e-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="0f72e-126">Wenn Sie den Parameter `includePersonalNotebooks` nicht einschließen, gibt Ihre Anforderung eine `400`-Fehlermeldung zurück.</span><span class="sxs-lookup"><span data-stu-id="0f72e-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0f72e-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f72e-127">Request headers</span></span>
| <span data-ttu-id="0f72e-128">Name</span><span class="sxs-lookup"><span data-stu-id="0f72e-128">Name</span></span>       | <span data-ttu-id="0f72e-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f72e-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0f72e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f72e-130">Authorization</span></span>  | <span data-ttu-id="0f72e-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0f72e-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f72e-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f72e-132">Request body</span></span>
<span data-ttu-id="0f72e-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f72e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f72e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f72e-134">Response</span></span>
<span data-ttu-id="0f72e-135">Eine erfolgreiche Antwort gibt `200 OK` mit einer JSON-Sammlung von **recentNotebooks** zurück.</span><span class="sxs-lookup"><span data-stu-id="0f72e-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="0f72e-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f72e-136">Example</span></span>
<span data-ttu-id="0f72e-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="0f72e-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0f72e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f72e-138">Request</span></span>
<span data-ttu-id="0f72e-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f72e-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="0f72e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f72e-140">Response</span></span>
<span data-ttu-id="0f72e-141">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f72e-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
