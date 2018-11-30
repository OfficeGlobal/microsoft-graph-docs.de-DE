---
title: SynchronizationSchema löschen
description: Löscht das angepasste Schema und setzt das Schema auf die Standardkonfiguration zurück. Wenn das Schema im Kontext der Vorlage gelöscht wird, wird das Schema auf den Standardwert eine der Vorlage zugeordnet zurückgesetzt `factoryTag`.
ms.openlocfilehash: 81c1a918b10e8f4553b3e99312f20bb538bfbe4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064153"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="6bc7b-104">SynchronizationSchema löschen</span><span class="sxs-lookup"><span data-stu-id="6bc7b-104">Delete synchronizationSchema</span></span>

> <span data-ttu-id="6bc7b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bc7b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bc7b-107">Löscht das angepasste Schema und setzt das Schema auf die Standardkonfiguration zurück.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-107">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="6bc7b-108">Wenn das Schema im Kontext der Vorlage gelöscht wird, wird das Schema auf den Standardwert eine der Vorlage zugeordnet zurückgesetzt `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-108">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bc7b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6bc7b-109">Permissions</span></span>
<span data-ttu-id="6bc7b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bc7b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bc7b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6bc7b-112">Permission type</span></span>                        | <span data-ttu-id="6bc7b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6bc7b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bc7b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6bc7b-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="6bc7b-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bc7b-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6bc7b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6bc7b-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6bc7b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bc7b-117">Not supported.</span></span>|
|<span data-ttu-id="6bc7b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6bc7b-118">Application</span></span>                            |<span data-ttu-id="6bc7b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bc7b-119">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="6bc7b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bc7b-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="6bc7b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6bc7b-121">Request headers</span></span>

| <span data-ttu-id="6bc7b-122">Name</span><span class="sxs-lookup"><span data-stu-id="6bc7b-122">Name</span></span>           | <span data-ttu-id="6bc7b-123">Typ</span><span class="sxs-lookup"><span data-stu-id="6bc7b-123">Type</span></span>    | <span data-ttu-id="6bc7b-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bc7b-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6bc7b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bc7b-125">Authorization</span></span>  | <span data-ttu-id="6bc7b-126">string</span><span class="sxs-lookup"><span data-stu-id="6bc7b-126">string</span></span>  | <span data-ttu-id="6bc7b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bc7b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6bc7b-129">Request body</span></span>

<span data-ttu-id="6bc7b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bc7b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bc7b-131">Response</span></span>

<span data-ttu-id="6bc7b-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `201 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-132">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="6bc7b-133">Es gibt keine Suchzeichenfolge in Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-133">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bc7b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6bc7b-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6bc7b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bc7b-135">Request</span></span>
<span data-ttu-id="6bc7b-136">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-136">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="6bc7b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bc7b-137">Response</span></span>
<span data-ttu-id="6bc7b-138">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="6bc7b-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->