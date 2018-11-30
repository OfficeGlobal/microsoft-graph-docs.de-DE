---
title: Regel abrufen
description: Abrufen der Eigenschaften und Beziehungen eines messageRule-Objekts.
ms.openlocfilehash: fa71a8447656fbf89fffe60bccec27d46d17c92a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018722"
---
# <a name="get-rule"></a><span data-ttu-id="d93cf-103">Regel abrufen</span><span class="sxs-lookup"><span data-stu-id="d93cf-103">Get rule</span></span>


<span data-ttu-id="d93cf-104">Abrufen der Eigenschaften und Beziehungen eines [messageRule](../resources/messagerule.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d93cf-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="d93cf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d93cf-105">Permissions</span></span>
<span data-ttu-id="d93cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93cf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d93cf-108">Permission type</span></span>      | <span data-ttu-id="d93cf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d93cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d93cf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d93cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d93cf-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d93cf-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d93cf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d93cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d93cf-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d93cf-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d93cf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d93cf-114">Application</span></span> | <span data-ttu-id="d93cf-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d93cf-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d93cf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d93cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d93cf-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d93cf-117">Optional query parameters</span></span>
<span data-ttu-id="d93cf-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d93cf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d93cf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d93cf-119">Request headers</span></span>
| <span data-ttu-id="d93cf-120">Name</span><span class="sxs-lookup"><span data-stu-id="d93cf-120">Name</span></span>      |<span data-ttu-id="d93cf-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d93cf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d93cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d93cf-122">Authorization</span></span>  | <span data-ttu-id="d93cf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d93cf-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d93cf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d93cf-125">Request body</span></span>
<span data-ttu-id="d93cf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d93cf-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d93cf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d93cf-127">Response</span></span>
<span data-ttu-id="d93cf-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [messageRule](../resources/messagerule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d93cf-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d93cf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d93cf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d93cf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d93cf-130">Request</span></span>
<span data-ttu-id="d93cf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d93cf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="d93cf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d93cf-132">Response</span></span>
<span data-ttu-id="d93cf-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d93cf-133">Here is an example of the response.</span></span> <span data-ttu-id="d93cf-134">Standardmäßig sind die Datums-/Uhrzeiteigenschaften in der Antwort in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="d93cf-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="d93cf-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d93cf-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->