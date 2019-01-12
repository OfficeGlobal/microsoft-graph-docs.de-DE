---
title: Auflisten von Regeln
description: Ruft alle messageRule-Objekte ab, die für das Postfach des Benutzers definiert sind.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d5c0dea2844c62133a15a4463cd2ea473f310a37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951229"
---
# <a name="list-rules"></a><span data-ttu-id="25f88-103">Auflisten von Regeln</span><span class="sxs-lookup"><span data-stu-id="25f88-103">List rules</span></span>

> <span data-ttu-id="25f88-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="25f88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25f88-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25f88-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25f88-106">Ruft alle [messageRule](../resources/messagerule.md)-Objekte ab, die für das Postfach des Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="25f88-106">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="25f88-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25f88-107">Permissions</span></span>
<span data-ttu-id="25f88-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25f88-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25f88-110">Permission type</span></span>      | <span data-ttu-id="25f88-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25f88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25f88-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25f88-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25f88-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="25f88-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="25f88-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25f88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25f88-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="25f88-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="25f88-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25f88-116">Application</span></span> | <span data-ttu-id="25f88-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="25f88-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="25f88-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25f88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25f88-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="25f88-119">Optional query parameters</span></span>
<span data-ttu-id="25f88-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="25f88-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="25f88-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25f88-121">Request headers</span></span>
| <span data-ttu-id="25f88-122">Name</span><span class="sxs-lookup"><span data-stu-id="25f88-122">Name</span></span>       | <span data-ttu-id="25f88-123">Typ</span><span class="sxs-lookup"><span data-stu-id="25f88-123">Type</span></span> | <span data-ttu-id="25f88-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25f88-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="25f88-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25f88-125">Authorization</span></span>  | <span data-ttu-id="25f88-126">string</span><span class="sxs-lookup"><span data-stu-id="25f88-126">string</span></span>  | <span data-ttu-id="25f88-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25f88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25f88-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25f88-129">Request body</span></span>
<span data-ttu-id="25f88-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="25f88-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="25f88-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="25f88-131">Response</span></span>
<span data-ttu-id="25f88-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [messageRule](../resources/messagerule.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25f88-132">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25f88-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25f88-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25f88-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25f88-134">Request</span></span>
<span data-ttu-id="25f88-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25f88-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
##### <a name="response"></a><span data-ttu-id="25f88-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="25f88-136">Response</span></span>
<span data-ttu-id="25f88-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25f88-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
