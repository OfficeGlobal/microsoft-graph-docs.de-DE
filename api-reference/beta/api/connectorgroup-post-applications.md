---
title: Erstellen der Anwendung
description: Verwenden Sie diese API, um eine neue Anwendung erstellen.
localization_priority: Normal
ms.openlocfilehash: e9d1c76f153c27ab3df24a93b44a570c2c1d836a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824668"
---
# <a name="create-application"></a><span data-ttu-id="db0f0-103">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="db0f0-103">Create application</span></span>

> <span data-ttu-id="db0f0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db0f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db0f0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db0f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db0f0-106">Verwenden Sie diese API, um eine neue Anwendung erstellen.</span><span class="sxs-lookup"><span data-stu-id="db0f0-106">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="db0f0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db0f0-107">Permissions</span></span>
<span data-ttu-id="db0f0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db0f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db0f0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db0f0-110">Permission type</span></span>      | <span data-ttu-id="db0f0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db0f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db0f0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db0f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db0f0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db0f0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db0f0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db0f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db0f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db0f0-115">Not supported.</span></span>    |
|<span data-ttu-id="db0f0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db0f0-116">Application</span></span> | <span data-ttu-id="db0f0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db0f0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db0f0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db0f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="db0f0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db0f0-119">Request headers</span></span>
| <span data-ttu-id="db0f0-120">Name</span><span class="sxs-lookup"><span data-stu-id="db0f0-120">Name</span></span>       | <span data-ttu-id="db0f0-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db0f0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db0f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db0f0-122">Authorization</span></span>  | <span data-ttu-id="db0f0-123">Bearer.</span><span class="sxs-lookup"><span data-stu-id="db0f0-123">Bearer.</span></span> <span data-ttu-id="db0f0-124">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="db0f0-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="db0f0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db0f0-125">Request body</span></span>
<span data-ttu-id="db0f0-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Application](../resources/application.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="db0f0-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db0f0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="db0f0-127">Response</span></span>

<span data-ttu-id="db0f0-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [Anwendung](../resources/application.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="db0f0-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db0f0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db0f0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db0f0-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db0f0-130">Request</span></span>
<span data-ttu-id="db0f0-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db0f0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="db0f0-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Application](../resources/application.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="db0f0-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="db0f0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="db0f0-133">Response</span></span>
<span data-ttu-id="db0f0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db0f0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

{
  "appId": "appId-value",
  "onPremisesPublishing": {
    "externalUrl": "externalUrl-value",
    "internalUrl": "internalUrl-value",
    "externalAuthenticationType": "externalAuthenticationType-value",
    "customDomainCertificate": "customDomainCertificate-value",
    "isTranslateHostHeaderEnabled": true,
    "isOnPremPublishingEnabled": true
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
