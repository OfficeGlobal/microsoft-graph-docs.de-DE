---
title: Sicherheitsaktion abrufen
description: Abrufen der Eigenschaften und Beziehungen des SecurityAction-Objekts.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 336a8a73d0ec161f26dd3fcbd36caf86097108f5
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366917"
---
# <a name="get-security-action"></a><span data-ttu-id="ff789-103">Sicherheitsaktion abrufen</span><span class="sxs-lookup"><span data-stu-id="ff789-103">Get security action</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff789-104">Ruft die Eigenschaften und Beziehungen eines [SecurityAction](../resources/securityaction.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="ff789-104">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff789-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ff789-105">Permissions</span></span>

<span data-ttu-id="ff789-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff789-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff789-108">Permission type</span></span>                        | <span data-ttu-id="ff789-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff789-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff789-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff789-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff789-111">SecurityActions. Read. all, SecurityActions. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="ff789-111">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="ff789-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff789-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff789-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff789-113">Not supported.</span></span> |
| <span data-ttu-id="ff789-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff789-114">Application</span></span>                            | <span data-ttu-id="ff789-115">SecurityActions. Read. all, SecurityActions. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="ff789-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff789-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff789-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff789-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ff789-117">Optional query parameters</span></span>

<span data-ttu-id="ff789-118">Diese Methode unterstützt einige der OData-Abfrageparameter zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff789-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ff789-119">Allgemeine Informationen finden Sie unter [OData Query Parameters](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ff789-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff789-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff789-120">Request headers</span></span>

| <span data-ttu-id="ff789-121">Name</span><span class="sxs-lookup"><span data-stu-id="ff789-121">Name</span></span>      |<span data-ttu-id="ff789-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff789-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff789-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff789-123">Authorization</span></span> | <span data-ttu-id="ff789-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ff789-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff789-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff789-125">Request body</span></span>

<span data-ttu-id="ff789-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff789-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff789-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff789-127">Response</span></span>

<span data-ttu-id="ff789-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [SecurityAction](../resources/securityaction.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff789-128">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff789-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="ff789-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff789-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff789-130">Request</span></span>

<span data-ttu-id="ff789-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff789-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```

### <a name="response"></a><span data-ttu-id="ff789-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff789-132">Response</span></span>

<span data-ttu-id="ff789-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff789-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ff789-134">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ff789-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff789-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ff789-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
