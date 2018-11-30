---
title: Abrufen von servicePrincipal
description: Rufen Sie die Eigenschaften und Beziehungen des Serviceprincipal-Objekts ab.
ms.openlocfilehash: 903bec11787b4b5acc5da688f7b73bf2bbd76262
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065628"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="d9efe-103">Abrufen von servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="d9efe-103">Get servicePrincipal</span></span>

> <span data-ttu-id="d9efe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d9efe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9efe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9efe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9efe-106">Rufen Sie die Eigenschaften und Beziehungen des Serviceprincipal-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="d9efe-106">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9efe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9efe-107">Permissions</span></span>
<span data-ttu-id="d9efe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9efe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9efe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9efe-110">Permission type</span></span>      | <span data-ttu-id="d9efe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9efe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9efe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9efe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9efe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9efe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9efe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9efe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9efe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9efe-115">Not supported.</span></span>    |
|<span data-ttu-id="d9efe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9efe-116">Application</span></span> | <span data-ttu-id="d9efe-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9efe-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9efe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9efe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9efe-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d9efe-119">Optional query parameters</span></span>
<span data-ttu-id="d9efe-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9efe-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9efe-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9efe-121">Request headers</span></span>
| <span data-ttu-id="d9efe-122">Name</span><span class="sxs-lookup"><span data-stu-id="d9efe-122">Name</span></span>       | <span data-ttu-id="d9efe-123">Typ</span><span class="sxs-lookup"><span data-stu-id="d9efe-123">Type</span></span> | <span data-ttu-id="d9efe-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9efe-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d9efe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9efe-125">Authorization</span></span>  | <span data-ttu-id="d9efe-126">string</span><span class="sxs-lookup"><span data-stu-id="d9efe-126">string</span></span>  | <span data-ttu-id="d9efe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9efe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9efe-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9efe-129">Request body</span></span>
<span data-ttu-id="d9efe-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9efe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9efe-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9efe-131">Response</span></span>

<span data-ttu-id="d9efe-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ServicePrincipal](../resources/serviceprincipal.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d9efe-132">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9efe-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9efe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9efe-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9efe-134">Request</span></span>
<span data-ttu-id="d9efe-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9efe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="d9efe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9efe-136">Response</span></span>
<span data-ttu-id="d9efe-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9efe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->