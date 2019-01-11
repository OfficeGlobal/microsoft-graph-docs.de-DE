---
title: SynchronisationVorlage aktualisieren
description: Aktualisieren Sie (Override) die Synchronisierung-Vorlage mit einer bestimmten Anwendung verbunden sind.
localization_priority: Normal
ms.openlocfilehash: ea4dfdc418d04467a6060a8c3d7d83423ba16e38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816737"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="b6f80-103">SynchronisationVorlage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b6f80-103">Update synchronizationTemplate</span></span>

> <span data-ttu-id="b6f80-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b6f80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6f80-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6f80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6f80-106">Aktualisieren Sie (Override) die Synchronisierung-Vorlage mit einer bestimmten Anwendung verbunden sind.</span><span class="sxs-lookup"><span data-stu-id="b6f80-106">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6f80-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b6f80-107">Permissions</span></span>
<span data-ttu-id="b6f80-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f80-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6f80-110">Permission type</span></span>                        | <span data-ttu-id="b6f80-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6f80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f80-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6f80-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="b6f80-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f80-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b6f80-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6f80-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b6f80-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6f80-115">Not supported.</span></span>|
|<span data-ttu-id="b6f80-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6f80-116">Application</span></span>                            |<span data-ttu-id="b6f80-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6f80-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="b6f80-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6f80-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="b6f80-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6f80-119">Request headers</span></span>

| <span data-ttu-id="b6f80-120">Name</span><span class="sxs-lookup"><span data-stu-id="b6f80-120">Name</span></span>           | <span data-ttu-id="b6f80-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b6f80-121">Type</span></span>    | <span data-ttu-id="b6f80-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6f80-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b6f80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6f80-123">Authorization</span></span>  | <span data-ttu-id="b6f80-124">string</span><span class="sxs-lookup"><span data-stu-id="b6f80-124">string</span></span>  | <span data-ttu-id="b6f80-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6f80-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6f80-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6f80-127">Request body</span></span>

<span data-ttu-id="b6f80-128">Geben Sie im Textkörper Anforderung das [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekt, um die vorhandene Vorlage ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b6f80-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="b6f80-129">Stellen Sie sicher, dass alle Eigenschaften vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="b6f80-129">Make sure all properties are provided.</span></span> <span data-ttu-id="b6f80-130">Fehlende Eigenschaften werden gelöscht.</span><span class="sxs-lookup"><span data-stu-id="b6f80-130">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="b6f80-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6f80-131">Response</span></span>

<span data-ttu-id="b6f80-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6f80-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="b6f80-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b6f80-134">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="b6f80-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6f80-135">Request</span></span>
<span data-ttu-id="b6f80-136">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6f80-136">The following is an example of a request.</span></span> 

><span data-ttu-id="b6f80-137">**Hinweis:** Das hier gezeigte Request-Objekt wird zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="b6f80-137">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="b6f80-138">Alle Eigenschaften in eine tatsächliche aufrufen einschließen.</span><span class="sxs-lookup"><span data-stu-id="b6f80-138">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="b6f80-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6f80-139">Response</span></span>
<span data-ttu-id="b6f80-140">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6f80-140">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
