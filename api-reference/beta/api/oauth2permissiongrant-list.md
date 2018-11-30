---
title: Liste oauth2PermissionGrants
description: Abrufen einer Liste von oauth2PermissionGrant-Objekten.
ms.openlocfilehash: 947041262ddac7ef0aab43ee455979ee0cf9bbf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062784"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="fc3f4-103">Liste oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="fc3f4-103">List oauth2PermissionGrants</span></span>

> <span data-ttu-id="fc3f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc3f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc3f4-106">Abrufen einer Liste von oauth2PermissionGrant-Objekten.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-106">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc3f4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc3f4-107">Permissions</span></span>

<span data-ttu-id="fc3f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc3f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc3f4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc3f4-110">Permission type</span></span>      | <span data-ttu-id="fc3f4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc3f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc3f4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc3f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc3f4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc3f4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc3f4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc3f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc3f4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc3f4-115">Not supported.</span></span>    |
|<span data-ttu-id="fc3f4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc3f4-116">Application</span></span> | <span data-ttu-id="fc3f4-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3f4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc3f4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc3f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc3f4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fc3f4-119">Optional query parameters</span></span>
<span data-ttu-id="fc3f4-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc3f4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc3f4-121">Request headers</span></span>
| <span data-ttu-id="fc3f4-122">Name</span><span class="sxs-lookup"><span data-stu-id="fc3f4-122">Name</span></span> | <span data-ttu-id="fc3f4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc3f4-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="fc3f4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc3f4-124">Authorization</span></span>  | <span data-ttu-id="fc3f4-125">string</span><span class="sxs-lookup"><span data-stu-id="fc3f4-125">string</span></span>  | <span data-ttu-id="fc3f4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc3f4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc3f4-128">Request body</span></span>
<span data-ttu-id="fc3f4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc3f4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc3f4-130">Response</span></span>

<span data-ttu-id="fc3f4-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="fc3f4-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc3f4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc3f4-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc3f4-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc3f4-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="fc3f4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc3f4-134">Response</span></span>

<span data-ttu-id="fc3f4-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc3f4-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->