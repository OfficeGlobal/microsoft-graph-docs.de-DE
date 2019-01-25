---
title: Erstellen von mailSearchFolder
description: Verwenden Sie diese API, um eine neue MailSearchFolder in das angegebene Postfach des Benutzers zu erstellen.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ef9992e1b0eaee83c39831424215cb9756f895d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517729"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="4eb72-103">Erstellen von mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="4eb72-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb72-104">Verwenden Sie diese API, um eine neue [MailSearchFolder](../resources/mailsearchfolder.md) in das angegebene Postfach des Benutzers zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="4eb72-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="4eb72-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4eb72-105">Permissions</span></span>

<span data-ttu-id="4eb72-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4eb72-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4eb72-108">Permission type</span></span> | <span data-ttu-id="4eb72-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4eb72-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="4eb72-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4eb72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4eb72-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb72-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4eb72-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4eb72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb72-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb72-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4eb72-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4eb72-114">Application</span></span> | <span data-ttu-id="4eb72-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb72-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eb72-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4eb72-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="4eb72-117">Geben Sie in der Abfrage-URL als eine Ordner-ID oder den Ordnernamen einer bekannten des übergeordneten Ordners.</span><span class="sxs-lookup"><span data-stu-id="4eb72-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="4eb72-118">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="4eb72-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eb72-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4eb72-119">Request headers</span></span>

| <span data-ttu-id="4eb72-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4eb72-120">Header</span></span> | <span data-ttu-id="4eb72-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4eb72-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="4eb72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eb72-122">Authorization</span></span> | <span data-ttu-id="4eb72-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="4eb72-123"></span></span> <span data-ttu-id="4eb72-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4eb72-124">Required.</span></span> |
| <span data-ttu-id="4eb72-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4eb72-125">Content-Type</span></span> | <span data-ttu-id="4eb72-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="4eb72-126"></span></span> <span data-ttu-id="4eb72-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4eb72-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4eb72-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4eb72-128">Request body</span></span>

<span data-ttu-id="4eb72-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4eb72-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4eb72-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="4eb72-130">Parameter</span></span> | <span data-ttu-id="4eb72-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4eb72-131">Type</span></span> | <span data-ttu-id="4eb72-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4eb72-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="4eb72-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="4eb72-133">@odata.type</span></span> | <span data-ttu-id="4eb72-134">String</span><span class="sxs-lookup"><span data-stu-id="4eb72-134">String</span></span> | <span data-ttu-id="4eb72-135">Der Typ des zu erstellenden Ordners.</span><span class="sxs-lookup"><span data-stu-id="4eb72-135">The type of folder to be created.</span></span> <span data-ttu-id="4eb72-136">Legen Sie auf "microsoft.graph.mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="4eb72-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="4eb72-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4eb72-137">displayName</span></span> | <span data-ttu-id="4eb72-138">String</span><span class="sxs-lookup"><span data-stu-id="4eb72-138">String</span></span> | <span data-ttu-id="4eb72-139">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="4eb72-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="4eb72-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="4eb72-140">includeNestedFolders</span></span> | <span data-ttu-id="4eb72-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4eb72-141">Boolean</span></span> | <span data-ttu-id="4eb72-142">Wie sollte die Hierarchie der Postfach-Ordner durchlaufen werden.</span><span class="sxs-lookup"><span data-stu-id="4eb72-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="4eb72-143">`true`bedeutet, dass eine umfassende Suche sollte erledigen `false` bedeutet, dass eine flache Suche sollte stattdessen durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="4eb72-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="4eb72-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="4eb72-144">sourceFolderIDs</span></span> | <span data-ttu-id="4eb72-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4eb72-145">String collection</span></span> | <span data-ttu-id="4eb72-146">Die Postfachordner, die durchsucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="4eb72-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="4eb72-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="4eb72-147">filterQuery</span></span> | <span data-ttu-id="4eb72-148">String</span><span class="sxs-lookup"><span data-stu-id="4eb72-148">String</span></span> | <span data-ttu-id="4eb72-149">Der OData-Abfrage Nachrichten gefiltert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4eb72-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="4eb72-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="4eb72-150">Response</span></span>

<span data-ttu-id="4eb72-151">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eines [MailSearchFolder](../resources/mailsearchfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4eb72-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb72-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4eb72-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4eb72-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4eb72-153">Request</span></span>

<span data-ttu-id="4eb72-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4eb72-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a><span data-ttu-id="4eb72-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="4eb72-155">Response</span></span>

<span data-ttu-id="4eb72-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4eb72-156">The following is an example of the response.</span></span>

><span data-ttu-id="4eb72-157">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="4eb72-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4eb72-158">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4eb72-158">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
