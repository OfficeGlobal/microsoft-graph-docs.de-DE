---
title: Erstellen von mailFolder
description: Verwenden Sie diese API, um eine neue untergeordnete MailFolder erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d466de7ae3952c85891c1798afa03b96aa887de0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962751"
---
# <a name="create-mailfolder"></a><span data-ttu-id="72b9a-103">Erstellen von mailFolder</span><span class="sxs-lookup"><span data-stu-id="72b9a-103">Create mailFolder</span></span>

> <span data-ttu-id="72b9a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="72b9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72b9a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72b9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72b9a-106">Verwenden Sie diese API, um eine neue untergeordnete [MailFolder](../resources/mailfolder.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="72b9a-106">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72b9a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="72b9a-107">Permissions</span></span>

<span data-ttu-id="72b9a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72b9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72b9a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72b9a-110">Permission type</span></span> | <span data-ttu-id="72b9a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72b9a-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="72b9a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72b9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72b9a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72b9a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="72b9a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72b9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72b9a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72b9a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="72b9a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72b9a-116">Application</span></span> | <span data-ttu-id="72b9a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72b9a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="72b9a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72b9a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="72b9a-119">Geben Sie in der Abfrage-URL als eine Ordner-ID oder den Ordnernamen einer bekannten des übergeordneten Ordners.</span><span class="sxs-lookup"><span data-stu-id="72b9a-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="72b9a-120">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="72b9a-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72b9a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72b9a-121">Request headers</span></span>

| <span data-ttu-id="72b9a-122">Header</span><span class="sxs-lookup"><span data-stu-id="72b9a-122">Header</span></span> | <span data-ttu-id="72b9a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="72b9a-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="72b9a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72b9a-124">Authorization</span></span> | <span data-ttu-id="72b9a-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="72b9a-125"></span></span> <span data-ttu-id="72b9a-126">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="72b9a-126">Required.</span></span> |
| <span data-ttu-id="72b9a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72b9a-127">Content-Type</span></span> | <span data-ttu-id="72b9a-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="72b9a-128"></span></span> <span data-ttu-id="72b9a-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="72b9a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72b9a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72b9a-130">Request body</span></span>

<span data-ttu-id="72b9a-p106">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="72b9a-p106">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="72b9a-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="72b9a-133">Parameter</span></span> | <span data-ttu-id="72b9a-134">Typ</span><span class="sxs-lookup"><span data-stu-id="72b9a-134">Type</span></span> | <span data-ttu-id="72b9a-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72b9a-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="72b9a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="72b9a-136">displayName</span></span>|<span data-ttu-id="72b9a-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b9a-137">String</span></span>|<span data-ttu-id="72b9a-138">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="72b9a-138">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="72b9a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="72b9a-139">Response</span></span>

<span data-ttu-id="72b9a-140">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eines [MailFolder](../resources/mailfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="72b9a-140">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72b9a-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72b9a-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="72b9a-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72b9a-142">Request</span></span>

<span data-ttu-id="72b9a-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72b9a-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="72b9a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="72b9a-144">Response</span></span>

<span data-ttu-id="72b9a-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="72b9a-145">The following is an example of the response.</span></span>

> <span data-ttu-id="72b9a-146">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="72b9a-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72b9a-147">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="72b9a-147">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
