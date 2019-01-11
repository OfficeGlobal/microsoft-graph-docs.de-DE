---
title: 'mailFolder: copy'
description: Mit dieser API können Sie ein Objekt des Typs „mailfolder“ samt seinem Inhalt in ein anderes Objekt des Typs „mailfolder“ kopieren.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 94470a21a1a640f4333419620e79eaf7b8d1130b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844092"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="61360-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="61360-103">mailFolder: copy</span></span>

<span data-ttu-id="61360-104">Mit dieser API können Sie ein Objekt des Typs „mailfolder“ samt seinem Inhalt in ein anderes Objekt des Typs „mailfolder“ kopieren.</span><span class="sxs-lookup"><span data-stu-id="61360-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="61360-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61360-105">Permissions</span></span>

<span data-ttu-id="61360-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61360-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61360-108">Permission type</span></span> | <span data-ttu-id="61360-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61360-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="61360-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61360-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61360-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61360-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61360-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61360-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61360-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61360-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61360-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61360-114">Application</span></span> | <span data-ttu-id="61360-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61360-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="61360-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61360-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="61360-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61360-117">Request headers</span></span>
| <span data-ttu-id="61360-118">Header</span><span class="sxs-lookup"><span data-stu-id="61360-118">Header</span></span> | <span data-ttu-id="61360-119">Wert</span><span class="sxs-lookup"><span data-stu-id="61360-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="61360-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="61360-120">Authorization</span></span> | <span data-ttu-id="61360-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="61360-121"></span></span> <span data-ttu-id="61360-122">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61360-122">Required.</span></span> |
| <span data-ttu-id="61360-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61360-123">Content-Type</span></span> | <span data-ttu-id="61360-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="61360-124"></span></span> <span data-ttu-id="61360-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61360-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61360-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61360-126">Request body</span></span>

<span data-ttu-id="61360-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="61360-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61360-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="61360-128">Parameter</span></span> | <span data-ttu-id="61360-129">Typ</span><span class="sxs-lookup"><span data-stu-id="61360-129">Type</span></span> | <span data-ttu-id="61360-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61360-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="61360-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="61360-131">destinationId</span></span>|<span data-ttu-id="61360-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61360-132">String</span></span>|<span data-ttu-id="61360-133">Die Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="61360-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="61360-134">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="61360-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="61360-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="61360-135">Response</span></span>

<span data-ttu-id="61360-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine [MailFolder](../resources/mailfolder.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="61360-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61360-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61360-137">Example</span></span>

<span data-ttu-id="61360-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="61360-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="61360-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61360-139">Request</span></span>
<span data-ttu-id="61360-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61360-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="61360-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="61360-141">Response</span></span>

<span data-ttu-id="61360-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="61360-142">Here is an example of the response.</span></span>

> <span data-ttu-id="61360-143">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="61360-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="61360-144">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="61360-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
