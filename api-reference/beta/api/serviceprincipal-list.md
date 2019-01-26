---
title: Liste servicePrincipals
description: Abrufen einer Liste von ServicePrincipal-Objekten.
localization_priority: Normal
ms.openlocfilehash: e8698e9715b4443d49224afcac8a5b363132db93
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574257"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="893e8-103">Liste servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="893e8-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="893e8-104">Abrufen einer Liste von ServicePrincipal-Objekten.</span><span class="sxs-lookup"><span data-stu-id="893e8-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="893e8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="893e8-105">Permissions</span></span>

<span data-ttu-id="893e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="893e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="893e8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="893e8-108">Permission type</span></span>      | <span data-ttu-id="893e8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="893e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="893e8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="893e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="893e8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="893e8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="893e8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="893e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="893e8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="893e8-113">Not supported.</span></span>    |
|<span data-ttu-id="893e8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="893e8-114">Application</span></span> | <span data-ttu-id="893e8-115">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="893e8-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="893e8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="893e8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="893e8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="893e8-117">Optional query parameters</span></span>

<span data-ttu-id="893e8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="893e8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="893e8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="893e8-119">Request headers</span></span>
| <span data-ttu-id="893e8-120">Name</span><span class="sxs-lookup"><span data-stu-id="893e8-120">Name</span></span> | <span data-ttu-id="893e8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="893e8-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="893e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="893e8-122">Authorization</span></span>  | <span data-ttu-id="893e8-123">string</span><span class="sxs-lookup"><span data-stu-id="893e8-123">string</span></span>  | <span data-ttu-id="893e8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="893e8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="893e8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="893e8-126">Request body</span></span>

<span data-ttu-id="893e8-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="893e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="893e8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="893e8-128">Response</span></span>

<span data-ttu-id="893e8-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ServicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="893e8-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="893e8-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="893e8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="893e8-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="893e8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="893e8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="893e8-132">Response</span></span>

<span data-ttu-id="893e8-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="893e8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
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
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
