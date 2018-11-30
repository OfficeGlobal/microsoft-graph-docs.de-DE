---
title: Abrufen von oAuth2Permissiongrant
description: Rufen Sie die Eigenschaften und Beziehungen des oAuth2Permissiongrant-Objekts ab.
ms.openlocfilehash: f5df8e647c2e71df67f7ac3fad6a81e8f2383f8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062058"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="cd204-103">Abrufen von oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="cd204-103">Get oAuth2Permissiongrant</span></span>

> <span data-ttu-id="cd204-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cd204-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd204-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd204-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd204-106">Rufen Sie die Eigenschaften und Beziehungen des oAuth2Permissiongrant-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="cd204-106">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd204-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd204-107">Permissions</span></span>
<span data-ttu-id="cd204-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd204-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd204-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd204-110">Permission type</span></span>      | <span data-ttu-id="cd204-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd204-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd204-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd204-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd204-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd204-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd204-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd204-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd204-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd204-115">Not supported.</span></span>    |
|<span data-ttu-id="cd204-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd204-116">Application</span></span> | <span data-ttu-id="cd204-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd204-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd204-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd204-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd204-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd204-119">Optional query parameters</span></span>
<span data-ttu-id="cd204-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd204-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd204-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd204-121">Request headers</span></span>
| <span data-ttu-id="cd204-122">Name</span><span class="sxs-lookup"><span data-stu-id="cd204-122">Name</span></span>       | <span data-ttu-id="cd204-123">Typ</span><span class="sxs-lookup"><span data-stu-id="cd204-123">Type</span></span> | <span data-ttu-id="cd204-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd204-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd204-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd204-125">Authorization</span></span>  | <span data-ttu-id="cd204-126">string</span><span class="sxs-lookup"><span data-stu-id="cd204-126">string</span></span>  | <span data-ttu-id="cd204-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd204-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd204-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd204-129">Request body</span></span>
<span data-ttu-id="cd204-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cd204-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd204-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd204-131">Response</span></span>

<span data-ttu-id="cd204-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cd204-132">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd204-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd204-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd204-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd204-134">Request</span></span>
<span data-ttu-id="cd204-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd204-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="cd204-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd204-136">Response</span></span>
<span data-ttu-id="cd204-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd204-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->