---
title: Erstellen der Anwendung
description: Verwenden Sie diese API, um eine neue Anwendung erstellen.
author: lleonard-msft
ms.openlocfilehash: 9530c94598eeb2413af67782b50bbf70f415e2a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361530"
---
# <a name="create-application"></a><span data-ttu-id="d182b-103">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="d182b-103">Create Application</span></span>

> <span data-ttu-id="d182b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d182b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d182b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d182b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d182b-106">Verwenden Sie diese API, um eine neue Anwendung erstellen.</span><span class="sxs-lookup"><span data-stu-id="d182b-106">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d182b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d182b-107">Permissions</span></span>
<span data-ttu-id="d182b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d182b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d182b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d182b-110">Permission type</span></span>      | <span data-ttu-id="d182b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d182b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d182b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d182b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d182b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d182b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d182b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d182b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d182b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d182b-115">Not supported.</span></span>    |
|<span data-ttu-id="d182b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d182b-116">Application</span></span> | <span data-ttu-id="d182b-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d182b-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d182b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d182b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="d182b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d182b-119">Request headers</span></span>
| <span data-ttu-id="d182b-120">Name</span><span class="sxs-lookup"><span data-stu-id="d182b-120">Name</span></span>       | <span data-ttu-id="d182b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d182b-121">Type</span></span> | <span data-ttu-id="d182b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d182b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d182b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d182b-123">Authorization</span></span>  | <span data-ttu-id="d182b-124">string</span><span class="sxs-lookup"><span data-stu-id="d182b-124">string</span></span>  | <span data-ttu-id="d182b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d182b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d182b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d182b-127">Request body</span></span>
<span data-ttu-id="d182b-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Application](../resources/application.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d182b-128">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d182b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d182b-129">Response</span></span>

<span data-ttu-id="d182b-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [Anwendung](../resources/application.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d182b-130">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d182b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d182b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d182b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d182b-132">Request</span></span>
<span data-ttu-id="d182b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d182b-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="d182b-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Application](../resources/application.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d182b-134">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d182b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d182b-135">Response</span></span>
<span data-ttu-id="d182b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d182b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->