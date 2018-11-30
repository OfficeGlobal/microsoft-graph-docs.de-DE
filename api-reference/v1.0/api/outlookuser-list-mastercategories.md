---
title: Auflisten von Outlook-Kategorien
description: Ruft alle Kategorien ab, die für den Benutzer definiert wurden.
ms.openlocfilehash: a27d8083a3a19e14d4c077e97c32525925538997
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016738"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="3b7f5-103">Auflisten von Outlook-Kategorien</span><span class="sxs-lookup"><span data-stu-id="3b7f5-103">List Outlook categories</span></span>


<span data-ttu-id="3b7f5-104">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b7f5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b7f5-105">Permissions</span></span>
<span data-ttu-id="3b7f5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b7f5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b7f5-108">Permission type</span></span>      | <span data-ttu-id="3b7f5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b7f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b7f5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b7f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b7f5-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="3b7f5-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="3b7f5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b7f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b7f5-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="3b7f5-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="3b7f5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b7f5-114">Application</span></span> | <span data-ttu-id="3b7f5-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="3b7f5-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b7f5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b7f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b7f5-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3b7f5-117">Optional query parameters</span></span>
<span data-ttu-id="3b7f5-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b7f5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b7f5-119">Request headers</span></span>
| <span data-ttu-id="3b7f5-120">Name</span><span class="sxs-lookup"><span data-stu-id="3b7f5-120">Name</span></span>      |<span data-ttu-id="3b7f5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b7f5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b7f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b7f5-122">Authorization</span></span>  | <span data-ttu-id="3b7f5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b7f5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b7f5-125">Request body</span></span>
<span data-ttu-id="3b7f5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b7f5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b7f5-127">Response</span></span>

<span data-ttu-id="3b7f5-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [outlookCategory](../resources/outlookcategory.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b7f5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b7f5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b7f5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b7f5-130">Request</span></span>
<span data-ttu-id="3b7f5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="3b7f5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b7f5-132">Response</span></span>
<span data-ttu-id="3b7f5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b7f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->