---
title: MailFolder erstellen
description: Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 92c57b5336eb60377915a4abc64b070b28bb98ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516490"
---
# <a name="create-mailfolder"></a><span data-ttu-id="e784f-103">Create MailFolder</span><span class="sxs-lookup"><span data-stu-id="e784f-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e784f-104">Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e784f-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e784f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e784f-105">Permissions</span></span>

<span data-ttu-id="e784f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e784f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e784f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e784f-108">Permission type</span></span> | <span data-ttu-id="e784f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e784f-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="e784f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e784f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e784f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e784f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e784f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e784f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e784f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e784f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e784f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e784f-114">Application</span></span> | <span data-ttu-id="e784f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e784f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e784f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e784f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="e784f-117">Geben Sie in der Abfrage-URL als eine Ordner-ID oder den Ordnernamen einer bekannten des übergeordneten Ordners.</span><span class="sxs-lookup"><span data-stu-id="e784f-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="e784f-118">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e784f-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e784f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e784f-119">Request headers</span></span>

| <span data-ttu-id="e784f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e784f-120">Header</span></span> | <span data-ttu-id="e784f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e784f-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="e784f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e784f-122">Authorization</span></span> | <span data-ttu-id="e784f-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="e784f-123"></span></span> <span data-ttu-id="e784f-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e784f-124">Required.</span></span> |
| <span data-ttu-id="e784f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e784f-125">Content-Type</span></span> | <span data-ttu-id="e784f-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="e784f-126"></span></span> <span data-ttu-id="e784f-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e784f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e784f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e784f-128">Request body</span></span>

<span data-ttu-id="e784f-p105">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e784f-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="e784f-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="e784f-131">Parameter</span></span> | <span data-ttu-id="e784f-132">Typ</span><span class="sxs-lookup"><span data-stu-id="e784f-132">Type</span></span> | <span data-ttu-id="e784f-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e784f-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="e784f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e784f-134">displayName</span></span>|<span data-ttu-id="e784f-135">String</span><span class="sxs-lookup"><span data-stu-id="e784f-135">String</span></span>|<span data-ttu-id="e784f-136">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="e784f-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e784f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e784f-137">Response</span></span>

<span data-ttu-id="e784f-138">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eines [MailFolder](../resources/mailfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e784f-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e784f-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e784f-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e784f-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e784f-140">Request</span></span>

<span data-ttu-id="e784f-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e784f-141">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="e784f-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e784f-142">Response</span></span>

<span data-ttu-id="e784f-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e784f-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e784f-144">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="e784f-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e784f-145">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e784f-145">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
