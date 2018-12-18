---
title: 'mailFolder: move'
description: Mit dieser API können Sie ein Objekt des Typs „mailfolder“ samt seinen Inhalten in ein anderes Objekt des Typs „mailfolder“ verschieben.
author: angelgolfer-ms
ms.openlocfilehash: 50c982a9c2277530c884ee2807543f858fd3b696
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348755"
---
# <a name="mailfolder-move"></a><span data-ttu-id="ec89a-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="ec89a-103">mailFolder: move</span></span>

> <span data-ttu-id="ec89a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec89a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec89a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec89a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec89a-106">Mit dieser API können Sie ein Objekt des Typs „mailfolder“ samt seinen Inhalten in ein anderes Objekt des Typs „mailfolder“ verschieben.</span><span class="sxs-lookup"><span data-stu-id="ec89a-106">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec89a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec89a-107">Permissions</span></span>

<span data-ttu-id="ec89a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec89a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec89a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec89a-110">Permission type</span></span> | <span data-ttu-id="ec89a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec89a-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ec89a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec89a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec89a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec89a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ec89a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec89a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec89a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec89a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ec89a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec89a-116">Application</span></span> | <span data-ttu-id="ec89a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec89a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec89a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec89a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="ec89a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec89a-119">Request headers</span></span>

| <span data-ttu-id="ec89a-120">Header</span><span class="sxs-lookup"><span data-stu-id="ec89a-120">Header</span></span> | <span data-ttu-id="ec89a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ec89a-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ec89a-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ec89a-122">Authorization</span></span> | <span data-ttu-id="ec89a-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ec89a-123"></span></span> <span data-ttu-id="ec89a-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec89a-124">Required.</span></span> |
| <span data-ttu-id="ec89a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec89a-125">Content-Type</span></span> | <span data-ttu-id="ec89a-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ec89a-126"></span></span> <span data-ttu-id="ec89a-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec89a-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec89a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec89a-128">Request body</span></span>

<span data-ttu-id="ec89a-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ec89a-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ec89a-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="ec89a-130">Parameter</span></span> | <span data-ttu-id="ec89a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ec89a-131">Type</span></span> | <span data-ttu-id="ec89a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec89a-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ec89a-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="ec89a-133">destinationId</span></span>|<span data-ttu-id="ec89a-134">String</span><span class="sxs-lookup"><span data-stu-id="ec89a-134">String</span></span>|<span data-ttu-id="ec89a-135">Die Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="ec89a-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ec89a-136">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ec89a-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ec89a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec89a-137">Response</span></span>

<span data-ttu-id="ec89a-138">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eines [MailFolder](../resources/mailfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ec89a-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec89a-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec89a-139">Example</span></span>

<span data-ttu-id="ec89a-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ec89a-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ec89a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec89a-141">Request</span></span>

<span data-ttu-id="ec89a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec89a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="ec89a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec89a-143">Response</span></span>

<span data-ttu-id="ec89a-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ec89a-144">Here is an example of the response.</span></span>

> <span data-ttu-id="ec89a-145">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ec89a-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ec89a-146">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ec89a-146">All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
