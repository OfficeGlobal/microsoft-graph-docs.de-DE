---
title: Liste agreementAcceptances
description: Abrufen einer Liste der AgreementAcceptance-Objekte des Benutzers an.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb92ff6c4a59b266735c09ed8e9d902813f5012f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953595"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="7d7fc-103">Liste agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="7d7fc-103">List agreementAcceptances</span></span>

> <span data-ttu-id="7d7fc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7d7fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d7fc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7d7fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d7fc-106">Abrufen einer Liste der [AgreementAcceptance](../resources/agreementacceptance.md) -Objekte des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="7d7fc-106">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d7fc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7d7fc-107">Permissions</span></span>
<span data-ttu-id="7d7fc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7fc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d7fc-110">Permission type</span></span>                        | <span data-ttu-id="7d7fc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d7fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d7fc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d7fc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d7fc-113">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="7d7fc-113">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="7d7fc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d7fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d7fc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d7fc-115">Not supported.</span></span> |
|<span data-ttu-id="7d7fc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d7fc-116">Application</span></span>                            | <span data-ttu-id="7d7fc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d7fc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d7fc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d7fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="7d7fc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d7fc-119">Request headers</span></span>
| <span data-ttu-id="7d7fc-120">Name</span><span class="sxs-lookup"><span data-stu-id="7d7fc-120">Name</span></span>      |<span data-ttu-id="7d7fc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d7fc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d7fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d7fc-122">Authorization</span></span> | <span data-ttu-id="7d7fc-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7d7fc-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d7fc-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d7fc-124">Request body</span></span>
<span data-ttu-id="7d7fc-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7d7fc-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7d7fc-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d7fc-126">Response</span></span>
<span data-ttu-id="7d7fc-127">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AgreementAcceptance](../resources/agreementacceptance.md) .</span><span class="sxs-lookup"><span data-stu-id="7d7fc-127">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d7fc-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d7fc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d7fc-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d7fc-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="7d7fc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d7fc-130">Response</span></span>
><span data-ttu-id="7d7fc-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7d7fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
