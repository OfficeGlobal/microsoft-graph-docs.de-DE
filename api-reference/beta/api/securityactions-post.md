---
title: Sicherheitsaktion erstellen
description: Erstellen eines neuen Sicherheits Aktionsobjekts. "
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e1958f80219234fcae54220491629a921dd8bcfd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366889"
---
# <a name="create-security-action"></a><span data-ttu-id="e94bf-103">Sicherheitsaktion erstellen</span><span class="sxs-lookup"><span data-stu-id="e94bf-103">Create security action</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e94bf-104">Erstellen eines neuen [SecurityAction](../resources/securityaction.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e94bf-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e94bf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e94bf-105">Permissions</span></span>

<span data-ttu-id="e94bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e94bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e94bf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e94bf-108">Permission type</span></span>                        | <span data-ttu-id="e94bf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e94bf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e94bf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e94bf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e94bf-111">SecurityActions. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="e94bf-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="e94bf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e94bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e94bf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e94bf-113">Not supported.</span></span> |
| <span data-ttu-id="e94bf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e94bf-114">Application</span></span>                            | <span data-ttu-id="e94bf-115">SecurityActions. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="e94bf-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e94bf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e94bf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="e94bf-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e94bf-117">Request headers</span></span>

| <span data-ttu-id="e94bf-118">Name</span><span class="sxs-lookup"><span data-stu-id="e94bf-118">Name</span></span>          | <span data-ttu-id="e94bf-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e94bf-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e94bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e94bf-120">Authorization</span></span> | <span data-ttu-id="e94bf-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e94bf-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e94bf-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e94bf-122">Request body</span></span>

<span data-ttu-id="e94bf-123">Geben Sie im Anforderungstext eine JSON-Darstellung eines [SecurityAction](../resources/securityaction.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e94bf-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e94bf-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="e94bf-124">Response</span></span>

<span data-ttu-id="e94bf-125">Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode und ein [SecurityAction](../resources/securityaction.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e94bf-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e94bf-126">Beispiele</span><span class="sxs-lookup"><span data-stu-id="e94bf-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e94bf-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e94bf-127">Request</span></span>

<span data-ttu-id="e94bf-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e94bf-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions
Content-type: application/json

{
  "name": "BlockIp",
  "actionReason": "Test",
  "parameters": [
    {
      "name": "IP",
      "value": "1.2.3.4"
    }
  ],
  "vendorInformation": {
    "provider": "Windows Defender ATP",
    "vendor": "Microsoft"
  }
}
```

### <a name="response"></a><span data-ttu-id="e94bf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e94bf-129">Response</span></span>

<span data-ttu-id="e94bf-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e94bf-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e94bf-131">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="e94bf-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e94bf-132">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e94bf-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id" : "1234567890",
    "status" : "notStarted",
    "createdDateTime": "2019-01-10 12:23:23.33333",
    "lastActionDateTime": "2019-01-10 12:23:23.33333",
    "name": "blockIp",
    "actionReason": "Test",
    "errorInfo": null,
    "vendorInformation": {
        "provider": "Windows Defender ATP",
        "providerVersion": null,
        "subProvider": null,
        "vendor": "Microsoft"
    },
    "parameters": [
        {
            "name": "IP",
            "value": "1.2.3.4"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->