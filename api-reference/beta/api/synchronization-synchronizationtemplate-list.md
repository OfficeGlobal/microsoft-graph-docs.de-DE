---
title: Vorhandene Synchronisierung Listenvorlagen
description: Listen Sie die Synchronisierung Vorlagen, die einer bestimmten Anwendung oder Dienstprinzipal zugeordnet.
localization_priority: Normal
ms.openlocfilehash: 49e9e257322886fe294807207276f8b6d6919909
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839438"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="4983e-103">Vorhandene Synchronisierung Listenvorlagen</span><span class="sxs-lookup"><span data-stu-id="4983e-103">List existing synchronization templates</span></span>

> <span data-ttu-id="4983e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4983e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4983e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4983e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4983e-106">Listen Sie die Synchronisierung Vorlagen, die einer bestimmten Anwendung oder Dienstprinzipal zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4983e-106">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="4983e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4983e-107">Permissions</span></span>
<span data-ttu-id="4983e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4983e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4983e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4983e-110">Permission type</span></span>                        | <span data-ttu-id="4983e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4983e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4983e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4983e-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4983e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4983e-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4983e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4983e-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4983e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4983e-115">Not supported.</span></span>|
|<span data-ttu-id="4983e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4983e-116">Application</span></span>                            |<span data-ttu-id="4983e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4983e-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="4983e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4983e-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="4983e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4983e-119">Request headers</span></span>

| <span data-ttu-id="4983e-120">Name</span><span class="sxs-lookup"><span data-stu-id="4983e-120">Name</span></span>           | <span data-ttu-id="4983e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4983e-121">Type</span></span>    | <span data-ttu-id="4983e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4983e-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4983e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4983e-123">Authorization</span></span>  | <span data-ttu-id="4983e-124">string</span><span class="sxs-lookup"><span data-stu-id="4983e-124">string</span></span>  | <span data-ttu-id="4983e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4983e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4983e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4983e-127">Request body</span></span>

<span data-ttu-id="4983e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4983e-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4983e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4983e-129">Response</span></span>

<span data-ttu-id="4983e-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Acollection [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekte in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4983e-130">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="4983e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4983e-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4983e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4983e-132">Request</span></span>
<span data-ttu-id="4983e-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4983e-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="4983e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4983e-134">Response</span></span>
<span data-ttu-id="4983e-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="4983e-135">The following is an example of a response.</span></span>
><span data-ttu-id="4983e-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="4983e-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4983e-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4983e-137">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
