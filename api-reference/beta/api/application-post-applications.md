---
title: Anwendung erstellen
description: Verwenden Sie diese API, um eine neue Anwendung zu erstellen.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b86030eede69b85d7b66e4ec5acdd7e2dfef0ce4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515223"
---
# <a name="create-application"></a><span data-ttu-id="a785c-103">Anwendung erstellen</span><span class="sxs-lookup"><span data-stu-id="a785c-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a785c-104">Verwenden Sie diese API, um eine neue Anwendung zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="a785c-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="a785c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a785c-105">Permissions</span></span>
<span data-ttu-id="a785c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a785c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a785c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a785c-108">Permission type</span></span>      | <span data-ttu-id="a785c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a785c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a785c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a785c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a785c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a785c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a785c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a785c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a785c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a785c-113">Not supported.</span></span>    |
|<span data-ttu-id="a785c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a785c-114">Application</span></span> | <span data-ttu-id="a785c-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a785c-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a785c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a785c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="a785c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a785c-117">Request headers</span></span>
| <span data-ttu-id="a785c-118">Name</span><span class="sxs-lookup"><span data-stu-id="a785c-118">Name</span></span>       | <span data-ttu-id="a785c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="a785c-119">Type</span></span> | <span data-ttu-id="a785c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a785c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a785c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a785c-121">Authorization</span></span>  | <span data-ttu-id="a785c-122">string</span><span class="sxs-lookup"><span data-stu-id="a785c-122">string</span></span>  | <span data-ttu-id="a785c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a785c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a785c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a785c-125">Request body</span></span>
<span data-ttu-id="a785c-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [application](../resources/application.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a785c-126">In the request body, supply a JSON representation of [plannerBucket](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a785c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a785c-127">Response</span></span>

<span data-ttu-id="a785c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [application](../resources/application.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a785c-128">If successful, this method returns `201 Created` response code and the [Contact](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a785c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a785c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a785c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a785c-130">Request</span></span>
<span data-ttu-id="a785c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a785c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
<span data-ttu-id="a785c-132">Geben Sie im Anforderungstext eine JSON-Darstellung eines [application](../resources/application.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a785c-132">In the request body, supply a JSON representation of [plannerBucket](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a785c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a785c-133">Response</span></span>
<span data-ttu-id="a785c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a785c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
