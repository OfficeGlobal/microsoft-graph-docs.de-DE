---
title: SynchronizationSchema löschen
description: Löscht das angepasste Schema und setzt das Schema auf die Standardkonfiguration zurück. Wenn das Schema im Kontext der Vorlage gelöscht wird, wird das Schema auf den Standardwert eine der Vorlage zugeordnet zurückgesetzt `factoryTag`.
localization_priority: Normal
ms.openlocfilehash: cb4c6295fe962ea9570da19b9b6ee8190b2024f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526991"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="b8c40-104">SynchronizationSchema löschen</span><span class="sxs-lookup"><span data-stu-id="b8c40-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8c40-105">Löscht das angepasste Schema und setzt das Schema auf die Standardkonfiguration zurück.</span><span class="sxs-lookup"><span data-stu-id="b8c40-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="b8c40-106">Wenn das Schema im Kontext der Vorlage gelöscht wird, wird das Schema auf den Standardwert eine der Vorlage zugeordnet zurückgesetzt `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="b8c40-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c40-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8c40-107">Permissions</span></span>
<span data-ttu-id="b8c40-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8c40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8c40-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8c40-110">Permission type</span></span>                        | <span data-ttu-id="b8c40-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8c40-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8c40-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8c40-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="b8c40-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c40-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b8c40-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8c40-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b8c40-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8c40-115">Not supported.</span></span>|
|<span data-ttu-id="b8c40-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8c40-116">Application</span></span>                            |<span data-ttu-id="b8c40-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8c40-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b8c40-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8c40-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="b8c40-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8c40-119">Request headers</span></span>

| <span data-ttu-id="b8c40-120">Name</span><span class="sxs-lookup"><span data-stu-id="b8c40-120">Name</span></span>           | <span data-ttu-id="b8c40-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b8c40-121">Type</span></span>    | <span data-ttu-id="b8c40-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8c40-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b8c40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8c40-123">Authorization</span></span>  | <span data-ttu-id="b8c40-124">string</span><span class="sxs-lookup"><span data-stu-id="b8c40-124">string</span></span>  | <span data-ttu-id="b8c40-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8c40-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8c40-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8c40-127">Request body</span></span>

<span data-ttu-id="b8c40-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8c40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8c40-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8c40-129">Response</span></span>

<span data-ttu-id="b8c40-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `201 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8c40-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="b8c40-131">Es gibt keine Suchzeichenfolge in Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8c40-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c40-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8c40-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8c40-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8c40-133">Request</span></span>
<span data-ttu-id="b8c40-134">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8c40-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="b8c40-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8c40-135">Response</span></span>
<span data-ttu-id="b8c40-136">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8c40-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
