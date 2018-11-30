---
title: MailFolder erstellen
description: Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.
ms.openlocfilehash: 79ed32a316a9012c33d3c08d0c95f00ad2f90725
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019494"
---
# <a name="create-mailfolder"></a><span data-ttu-id="74177-103">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="74177-103">Create MailFolder</span></span>

<span data-ttu-id="74177-104">Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="74177-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="74177-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74177-105">Permissions</span></span>

<span data-ttu-id="74177-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74177-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74177-108">Permission type</span></span> | <span data-ttu-id="74177-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74177-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="74177-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74177-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74177-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74177-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74177-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74177-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74177-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74177-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74177-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74177-114">Application</span></span> | <span data-ttu-id="74177-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74177-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74177-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74177-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="74177-117">Geben Sie in der Abfrage-URL als eine Ordner-ID oder den Ordnernamen einer bekannten des übergeordneten Ordners.</span><span class="sxs-lookup"><span data-stu-id="74177-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="74177-118">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="74177-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="74177-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74177-119">Request headers</span></span>

| <span data-ttu-id="74177-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="74177-120">Header</span></span> | <span data-ttu-id="74177-121">Wert</span><span class="sxs-lookup"><span data-stu-id="74177-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="74177-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74177-122">Authorization</span></span> | <span data-ttu-id="74177-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="74177-123"></span></span> <span data-ttu-id="74177-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74177-124">Required.</span></span> |
| <span data-ttu-id="74177-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74177-125">Content-Type</span></span> | <span data-ttu-id="74177-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="74177-126"></span></span> <span data-ttu-id="74177-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74177-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74177-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74177-128">Request body</span></span>

<span data-ttu-id="74177-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="74177-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="74177-130">**DisplayName** ist die nur schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="74177-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="74177-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="74177-131">Parameter</span></span> | <span data-ttu-id="74177-132">Typ</span><span class="sxs-lookup"><span data-stu-id="74177-132">Type</span></span> | <span data-ttu-id="74177-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74177-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="74177-134">displayName</span><span class="sxs-lookup"><span data-stu-id="74177-134">displayName</span></span>|<span data-ttu-id="74177-135">String</span><span class="sxs-lookup"><span data-stu-id="74177-135">String</span></span>|<span data-ttu-id="74177-136">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="74177-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="74177-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="74177-137">Response</span></span>

<span data-ttu-id="74177-138">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [MailFolder](../resources/mailfolder.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="74177-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74177-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74177-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="74177-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74177-140">Request</span></span>

<span data-ttu-id="74177-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74177-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="74177-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="74177-142">Response</span></span>
<span data-ttu-id="74177-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74177-143">Here is an example of the response.</span></span>

> <span data-ttu-id="74177-144">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="74177-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74177-145">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="74177-145">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
