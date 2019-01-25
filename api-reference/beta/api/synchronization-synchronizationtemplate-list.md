---
title: Vorhandene Synchronisierung Listenvorlagen
description: Listen Sie die Synchronisierung Vorlagen, die einer bestimmten Anwendung oder Dienstprinzipal zugeordnet.
localization_priority: Normal
ms.openlocfilehash: 309d1ddd6d702652b14e10895de10486a5d23783
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523631"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="1ca7d-103">Vorhandene Synchronisierung Listenvorlagen</span><span class="sxs-lookup"><span data-stu-id="1ca7d-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca7d-104">Listen Sie die Synchronisierung Vorlagen, die einer bestimmten Anwendung oder Dienstprinzipal zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ca7d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1ca7d-105">Permissions</span></span>
<span data-ttu-id="1ca7d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca7d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ca7d-108">Permission type</span></span>                        | <span data-ttu-id="1ca7d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ca7d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ca7d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ca7d-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="1ca7d-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ca7d-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1ca7d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ca7d-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1ca7d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ca7d-113">Not supported.</span></span>|
|<span data-ttu-id="1ca7d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ca7d-114">Application</span></span>                            |<span data-ttu-id="1ca7d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ca7d-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="1ca7d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ca7d-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="1ca7d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ca7d-117">Request headers</span></span>

| <span data-ttu-id="1ca7d-118">Name</span><span class="sxs-lookup"><span data-stu-id="1ca7d-118">Name</span></span>           | <span data-ttu-id="1ca7d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="1ca7d-119">Type</span></span>    | <span data-ttu-id="1ca7d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ca7d-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1ca7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ca7d-121">Authorization</span></span>  | <span data-ttu-id="1ca7d-122">string</span><span class="sxs-lookup"><span data-stu-id="1ca7d-122">string</span></span>  | <span data-ttu-id="1ca7d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ca7d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ca7d-125">Request body</span></span>

<span data-ttu-id="1ca7d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="1ca7d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ca7d-127">Response</span></span>

<span data-ttu-id="1ca7d-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Acollection [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekte in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="1ca7d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ca7d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1ca7d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ca7d-130">Request</span></span>
<span data-ttu-id="1ca7d-131">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="1ca7d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ca7d-132">Response</span></span>
<span data-ttu-id="1ca7d-133">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-133">The following is an example of a response.</span></span>
><span data-ttu-id="1ca7d-134">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ca7d-135">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ca7d-135">All the properties will be returned in an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
