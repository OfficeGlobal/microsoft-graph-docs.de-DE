---
title: 'notebook: getRecentNotebooks'
description: Rufen Sie eine Liste der recentNotebook-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 90f620a82794bb575d9dfa35f2ad31b062b2faf4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527703"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="1a588-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="1a588-103">notebook: getRecentNotebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a588-104">Rufen Sie eine Liste der [recentNotebook](../resources/recentnotebook.md)-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="1a588-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a588-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a588-105">Permissions</span></span>
<span data-ttu-id="1a588-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a588-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a588-108">Permission type</span></span>      | <span data-ttu-id="1a588-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a588-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a588-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a588-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a588-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="1a588-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="1a588-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a588-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a588-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a588-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="1a588-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a588-114">Application</span></span> | <span data-ttu-id="1a588-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a588-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a588-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a588-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="1a588-117">Der `<id | userPrincipalName>` für den Benutzer muss mit dem im Autorisierungstoken (zur Erstellung der Anforderung verwendet) codierten Benutzer übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="1a588-117">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="1a588-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="1a588-118">Function parameters</span></span>

| <span data-ttu-id="1a588-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="1a588-119">Parameter</span></span>    | <span data-ttu-id="1a588-120">Typ</span><span class="sxs-lookup"><span data-stu-id="1a588-120">Type</span></span>   |<span data-ttu-id="1a588-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a588-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a588-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="1a588-122">includePersonalNotebooks</span></span>|<span data-ttu-id="1a588-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a588-123">Boolean</span></span>|<span data-ttu-id="1a588-124">Schließen Sie Notizbücher ein, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="1a588-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="1a588-125">Wählen Sie `true`, um Notizbücher einzuschließen, die dem Benutzer gehören; wählen Sie andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="1a588-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="1a588-126">Wenn Sie den Parameter `includePersonalNotebooks` nicht einschließen, gibt Ihre Anforderung eine `400`-Fehlermeldung zurück.</span><span class="sxs-lookup"><span data-stu-id="1a588-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1a588-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a588-127">Request headers</span></span>
| <span data-ttu-id="1a588-128">Name</span><span class="sxs-lookup"><span data-stu-id="1a588-128">Name</span></span>       | <span data-ttu-id="1a588-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a588-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a588-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a588-130">Authorization</span></span>  | <span data-ttu-id="1a588-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1a588-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a588-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a588-132">Request body</span></span>
<span data-ttu-id="1a588-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1a588-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a588-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a588-134">Response</span></span>
<span data-ttu-id="1a588-135">Eine erfolgreiche Antwort gibt `200 OK` mit einer JSON-Sammlung von **recentNotebooks** zurück.</span><span class="sxs-lookup"><span data-stu-id="1a588-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="1a588-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a588-136">Example</span></span>
<span data-ttu-id="1a588-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="1a588-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1a588-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a588-138">Request</span></span>
<span data-ttu-id="1a588-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a588-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="1a588-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a588-140">Response</span></span>
<span data-ttu-id="1a588-141">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a588-141">The following example shows the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-getrecentnotebooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
