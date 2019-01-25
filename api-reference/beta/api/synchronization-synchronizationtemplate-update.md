---
title: SynchronisationVorlage aktualisieren
description: Aktualisieren Sie (Override) die Synchronisierung-Vorlage mit einer bestimmten Anwendung verbunden sind.
localization_priority: Normal
ms.openlocfilehash: 152186afd9f7b7cce2a04170de7148d454525d80
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517463"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="de271-103">SynchronisationVorlage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="de271-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de271-104">Aktualisieren Sie (Override) die Synchronisierung-Vorlage mit einer bestimmten Anwendung verbunden sind.</span><span class="sxs-lookup"><span data-stu-id="de271-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="de271-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de271-105">Permissions</span></span>
<span data-ttu-id="de271-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de271-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de271-108">Permission type</span></span>                        | <span data-ttu-id="de271-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de271-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="de271-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de271-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="de271-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de271-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="de271-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de271-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="de271-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de271-113">Not supported.</span></span>|
|<span data-ttu-id="de271-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de271-114">Application</span></span>                            |<span data-ttu-id="de271-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de271-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="de271-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de271-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="de271-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de271-117">Request headers</span></span>

| <span data-ttu-id="de271-118">Name</span><span class="sxs-lookup"><span data-stu-id="de271-118">Name</span></span>           | <span data-ttu-id="de271-119">Typ</span><span class="sxs-lookup"><span data-stu-id="de271-119">Type</span></span>    | <span data-ttu-id="de271-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de271-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="de271-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de271-121">Authorization</span></span>  | <span data-ttu-id="de271-122">string</span><span class="sxs-lookup"><span data-stu-id="de271-122">string</span></span>  | <span data-ttu-id="de271-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de271-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de271-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de271-125">Request body</span></span>

<span data-ttu-id="de271-126">Geben Sie im Textkörper Anforderung das [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekt, um die vorhandene Vorlage ersetzt.</span><span class="sxs-lookup"><span data-stu-id="de271-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="de271-127">Stellen Sie sicher, dass alle Eigenschaften vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="de271-127">Make sure all properties are provided.</span></span> <span data-ttu-id="de271-128">Fehlende Eigenschaften werden gelöscht.</span><span class="sxs-lookup"><span data-stu-id="de271-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="de271-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="de271-129">Response</span></span>

<span data-ttu-id="de271-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de271-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="de271-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="de271-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="de271-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de271-133">Request</span></span>
<span data-ttu-id="de271-134">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de271-134">The following is an example of a request.</span></span> 

><span data-ttu-id="de271-135">**Hinweis:** Das hier gezeigte Request-Objekt wird zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="de271-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="de271-136">Alle Eigenschaften in eine tatsächliche aufrufen einschließen.</span><span class="sxs-lookup"><span data-stu-id="de271-136">Include all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="de271-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="de271-137">Response</span></span>
<span data-ttu-id="de271-138">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="de271-138">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
