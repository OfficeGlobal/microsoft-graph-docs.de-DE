---
title: Liste servicePrincipals
description: Abrufen einer Liste von ServicePrincipal-Objekten.
ms.openlocfilehash: deb0fdc0634d7702beaba5b4066b4e83b28c267b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065012"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="84fba-103">Liste servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="84fba-103">List servicePrincipals</span></span>

> <span data-ttu-id="84fba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="84fba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84fba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84fba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84fba-106">Abrufen einer Liste von ServicePrincipal-Objekten.</span><span class="sxs-lookup"><span data-stu-id="84fba-106">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="84fba-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="84fba-107">Permissions</span></span>

<span data-ttu-id="84fba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84fba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84fba-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84fba-110">Permission type</span></span>      | <span data-ttu-id="84fba-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84fba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84fba-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84fba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="84fba-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84fba-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="84fba-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84fba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84fba-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84fba-115">Not supported.</span></span>    |
|<span data-ttu-id="84fba-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84fba-116">Application</span></span> | <span data-ttu-id="84fba-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="84fba-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84fba-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84fba-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84fba-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="84fba-119">Optional query parameters</span></span>

<span data-ttu-id="84fba-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84fba-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84fba-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84fba-121">Request headers</span></span>
| <span data-ttu-id="84fba-122">Name</span><span class="sxs-lookup"><span data-stu-id="84fba-122">Name</span></span> | <span data-ttu-id="84fba-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84fba-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="84fba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="84fba-124">Authorization</span></span>  | <span data-ttu-id="84fba-125">string</span><span class="sxs-lookup"><span data-stu-id="84fba-125">string</span></span>  | <span data-ttu-id="84fba-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84fba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84fba-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84fba-128">Request body</span></span>

<span data-ttu-id="84fba-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84fba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84fba-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="84fba-130">Response</span></span>

<span data-ttu-id="84fba-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ServicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="84fba-131">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84fba-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84fba-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="84fba-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84fba-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="84fba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="84fba-134">Response</span></span>

<span data-ttu-id="84fba-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84fba-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
