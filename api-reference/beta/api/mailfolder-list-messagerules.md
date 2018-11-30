---
title: Auflisten von Regeln
description: Ruft alle messageRule-Objekte ab, die für das Postfach des Benutzers definiert sind.
ms.openlocfilehash: 9cd56e3ad7c63a2b8ad84758ac7d26c3c349810a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065526"
---
# <a name="list-rules"></a><span data-ttu-id="8f1eb-103">Auflisten von Regeln</span><span class="sxs-lookup"><span data-stu-id="8f1eb-103">List rules</span></span>

> <span data-ttu-id="8f1eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f1eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f1eb-106">Ruft alle [messageRule](../resources/messagerule.md)-Objekte ab, die für das Postfach des Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-106">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f1eb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8f1eb-107">Permissions</span></span>
<span data-ttu-id="8f1eb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f1eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f1eb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f1eb-110">Permission type</span></span>      | <span data-ttu-id="8f1eb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f1eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f1eb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f1eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f1eb-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8f1eb-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="8f1eb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f1eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f1eb-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8f1eb-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="8f1eb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f1eb-116">Application</span></span> | <span data-ttu-id="8f1eb-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8f1eb-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f1eb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f1eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8f1eb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8f1eb-119">Optional query parameters</span></span>
<span data-ttu-id="8f1eb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8f1eb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f1eb-121">Request headers</span></span>
| <span data-ttu-id="8f1eb-122">Name</span><span class="sxs-lookup"><span data-stu-id="8f1eb-122">Name</span></span>       | <span data-ttu-id="8f1eb-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8f1eb-123">Type</span></span> | <span data-ttu-id="8f1eb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f1eb-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f1eb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f1eb-125">Authorization</span></span>  | <span data-ttu-id="8f1eb-126">string</span><span class="sxs-lookup"><span data-stu-id="8f1eb-126">string</span></span>  | <span data-ttu-id="8f1eb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f1eb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f1eb-129">Request body</span></span>
<span data-ttu-id="8f1eb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8f1eb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f1eb-131">Response</span></span>
<span data-ttu-id="8f1eb-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [messageRule](../resources/messagerule.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-132">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f1eb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f1eb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f1eb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f1eb-134">Request</span></span>
<span data-ttu-id="8f1eb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
##### <a name="response"></a><span data-ttu-id="8f1eb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f1eb-136">Response</span></span>
<span data-ttu-id="8f1eb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f1eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
      "id":"AQAAAJ5dZqA=",
      "displayName":"From partner",
      "sequence":2,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "senderContains":[
          "ADELE"
        ]
      },
      "actions":{
        "stopProcessingRules":true,
        "forwardTo":[
          {
            "emailAddress":{
              "name":"Alex Wilbur",
              "address":"AlexW@contoso.onmicrosoft.com"
            }
          }
        ]
      }
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
