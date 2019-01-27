---
title: Anwendung abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des Anwendungsobjekts.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9470243651d668d8a1440077be89225b0ebe7b21
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515762"
---
# <a name="get-application"></a><span data-ttu-id="0d595-103">Anwendung abrufen</span><span class="sxs-lookup"><span data-stu-id="0d595-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d595-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des Anwendungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="0d595-104">Retrieve the properties and relationships of application object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d595-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d595-105">Permissions</span></span>
<span data-ttu-id="0d595-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d595-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d595-108">Permission type</span></span>      | <span data-ttu-id="0d595-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d595-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d595-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d595-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d595-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d595-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d595-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d595-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d595-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d595-113">Not supported.</span></span>    |
|<span data-ttu-id="0d595-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d595-114">Application</span></span> | <span data-ttu-id="0d595-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d595-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d595-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d595-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d595-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0d595-117">Optional query parameters</span></span>
<span data-ttu-id="0d595-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0d595-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d595-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d595-119">Request headers</span></span>
| <span data-ttu-id="0d595-120">Name</span><span class="sxs-lookup"><span data-stu-id="0d595-120">Name</span></span>       | <span data-ttu-id="0d595-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0d595-121">Type</span></span> | <span data-ttu-id="0d595-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d595-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0d595-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d595-123">Authorization</span></span>  | <span data-ttu-id="0d595-124">string</span><span class="sxs-lookup"><span data-stu-id="0d595-124">string</span></span>  | <span data-ttu-id="0d595-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d595-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d595-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d595-127">Request body</span></span>
<span data-ttu-id="0d595-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0d595-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d595-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d595-129">Response</span></span>

<span data-ttu-id="0d595-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [application](../resources/application.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d595-130">If successful, this method returns a `200 OK` response code and a [deviceManagementExchangeConnector](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d595-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d595-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d595-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d595-132">Request</span></span>
<span data-ttu-id="0d595-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d595-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="0d595-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d595-134">Response</span></span>
<span data-ttu-id="0d595-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d595-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
  "api": {
    "acceptedAccessTokenVersion": 1,
    "publishedPermissionScopes": [
      {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
      }
    ]
  },
  "allowPublicClient": true,
  "applicationAliases": [
    "applicationAliases-value"
  ],
  "createdDateTime": "datetime-value",
  "installedClients": {
    "redirectUrls": [
      "redirectUrls-value"
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
