---
title: 'notebook: getRecentNotebooks'
description: Rufen Sie eine Liste der recentNotebook-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.
author: Jewan-microsoft
ms.openlocfilehash: 43141d7734a3427a3325a852d8185ebbee5d752c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350498"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="a5caf-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="a5caf-103">notebook: getRecentNotebooks</span></span>

> <span data-ttu-id="a5caf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a5caf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5caf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5caf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5caf-106">Rufen Sie eine Liste der [recentNotebook](../resources/recentnotebook.md)-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="a5caf-106">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5caf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a5caf-107">Permissions</span></span>
<span data-ttu-id="a5caf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5caf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5caf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5caf-110">Permission type</span></span>      | <span data-ttu-id="a5caf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5caf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5caf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5caf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5caf-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="a5caf-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="a5caf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5caf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5caf-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5caf-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="a5caf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5caf-116">Application</span></span> | <span data-ttu-id="a5caf-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5caf-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5caf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5caf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="a5caf-119">Der `<id | userPrincipalName>` für den Benutzer muss mit dem im Autorisierungstoken (zur Erstellung der Anforderung verwendet) codierten Benutzer übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="a5caf-119">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="a5caf-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="a5caf-120">Function parameters</span></span>

| <span data-ttu-id="a5caf-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="a5caf-121">Parameter</span></span>    | <span data-ttu-id="a5caf-122">Typ</span><span class="sxs-lookup"><span data-stu-id="a5caf-122">Type</span></span>   |<span data-ttu-id="a5caf-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5caf-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5caf-124">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="a5caf-124">includePersonalNotebooks</span></span>|<span data-ttu-id="a5caf-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5caf-125">Boolean</span></span>|<span data-ttu-id="a5caf-126">Schließen Sie Notizbücher ein, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="a5caf-126">Include notebooks owned by the user.</span></span> <span data-ttu-id="a5caf-127">Wählen Sie `true`, um Notizbücher einzuschließen, die dem Benutzer gehören; wählen Sie andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="a5caf-127">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="a5caf-128">Wenn Sie den Parameter `includePersonalNotebooks` nicht einschließen, gibt Ihre Anforderung eine `400`-Fehlermeldung zurück.</span><span class="sxs-lookup"><span data-stu-id="a5caf-128">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a5caf-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5caf-129">Request headers</span></span>
| <span data-ttu-id="a5caf-130">Name</span><span class="sxs-lookup"><span data-stu-id="a5caf-130">Name</span></span>       | <span data-ttu-id="a5caf-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5caf-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a5caf-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a5caf-132">Authorization</span></span>  | <span data-ttu-id="a5caf-133">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a5caf-133">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5caf-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5caf-134">Request body</span></span>
<span data-ttu-id="a5caf-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a5caf-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5caf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5caf-136">Response</span></span>
<span data-ttu-id="a5caf-137">Eine erfolgreiche Antwort gibt `200 OK` mit einer JSON-Sammlung von **recentNotebooks** zurück.</span><span class="sxs-lookup"><span data-stu-id="a5caf-137">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="a5caf-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5caf-138">Example</span></span>
<span data-ttu-id="a5caf-139">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="a5caf-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a5caf-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5caf-140">Request</span></span>
<span data-ttu-id="a5caf-141">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="a5caf-141">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="a5caf-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5caf-142">Response</span></span>
<span data-ttu-id="a5caf-143">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="a5caf-143">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
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
