---
title: List servicePrincipals
description: Abrufen einer Liste von servicePrincipal-Objekten.
localization_priority: Normal
ms.openlocfilehash: cd61b69e330ac376d15bfaf99c1147b8f9402d7f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643629"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="fab30-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="fab30-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fab30-104">Abrufen einer Liste von servicePrincipal-Objekten.</span><span class="sxs-lookup"><span data-stu-id="fab30-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fab30-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fab30-105">Permissions</span></span>

<span data-ttu-id="fab30-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fab30-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fab30-108">Permission type</span></span>      | <span data-ttu-id="fab30-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fab30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fab30-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fab30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fab30-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fab30-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fab30-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fab30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fab30-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fab30-113">Not supported.</span></span>    |
|<span data-ttu-id="fab30-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fab30-114">Application</span></span> | <span data-ttu-id="fab30-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fab30-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fab30-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fab30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fab30-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fab30-117">Optional query parameters</span></span>

<span data-ttu-id="fab30-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fab30-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fab30-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fab30-119">Request headers</span></span>
| <span data-ttu-id="fab30-120">Name</span><span class="sxs-lookup"><span data-stu-id="fab30-120">Name</span></span> | <span data-ttu-id="fab30-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fab30-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="fab30-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fab30-122">Authorization</span></span>  | <span data-ttu-id="fab30-123">string</span><span class="sxs-lookup"><span data-stu-id="fab30-123">string</span></span>  | <span data-ttu-id="fab30-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fab30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fab30-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fab30-126">Request body</span></span>

<span data-ttu-id="fab30-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fab30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fab30-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="fab30-128">Response</span></span>

<span data-ttu-id="fab30-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ServicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="fab30-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab30-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fab30-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fab30-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fab30-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="fab30-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fab30-132">Response</span></span>

<span data-ttu-id="fab30-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fab30-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
