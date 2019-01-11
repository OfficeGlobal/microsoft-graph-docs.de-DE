---
title: Erstellen von mailSearchFolder
description: Verwenden Sie diese API, um eine neue MailSearchFolder in das angegebene Postfach des Benutzers zu erstellen.
localization_priority: Normal
ms.openlocfilehash: 07c6b96bc2dec35d06b5563673012ca0eafb3885
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840187"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="d1b42-103">Erstellen von mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="d1b42-103">Create mailSearchFolder</span></span>

> <span data-ttu-id="d1b42-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d1b42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1b42-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1b42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1b42-106">Verwenden Sie diese API, um eine neue [MailSearchFolder](../resources/mailsearchfolder.md) in das angegebene Postfach des Benutzers zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d1b42-106">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1b42-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d1b42-107">Permissions</span></span>

<span data-ttu-id="d1b42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1b42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1b42-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1b42-110">Permission type</span></span> | <span data-ttu-id="d1b42-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1b42-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d1b42-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1b42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1b42-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1b42-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d1b42-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1b42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1b42-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1b42-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d1b42-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1b42-116">Application</span></span> | <span data-ttu-id="d1b42-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1b42-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1b42-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1b42-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="d1b42-119">Geben Sie in der Abfrage-URL als eine Ordner-ID oder den Ordnernamen einer bekannten des übergeordneten Ordners.</span><span class="sxs-lookup"><span data-stu-id="d1b42-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d1b42-120">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d1b42-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1b42-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1b42-121">Request headers</span></span>

| <span data-ttu-id="d1b42-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d1b42-122">Header</span></span> | <span data-ttu-id="d1b42-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d1b42-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d1b42-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1b42-124">Authorization</span></span> | <span data-ttu-id="d1b42-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d1b42-125"></span></span> <span data-ttu-id="d1b42-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b42-126">Required.</span></span> |
| <span data-ttu-id="d1b42-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1b42-127">Content-Type</span></span> | <span data-ttu-id="d1b42-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d1b42-128"></span></span> <span data-ttu-id="d1b42-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b42-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1b42-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1b42-130">Request body</span></span>

<span data-ttu-id="d1b42-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d1b42-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1b42-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="d1b42-132">Parameter</span></span> | <span data-ttu-id="d1b42-133">Typ</span><span class="sxs-lookup"><span data-stu-id="d1b42-133">Type</span></span> | <span data-ttu-id="d1b42-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1b42-134">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="d1b42-135">@odata.type</span><span class="sxs-lookup"><span data-stu-id="d1b42-135">@odata.type</span></span> | <span data-ttu-id="d1b42-136">String</span><span class="sxs-lookup"><span data-stu-id="d1b42-136">String</span></span> | <span data-ttu-id="d1b42-137">Der Typ des zu erstellenden Ordners.</span><span class="sxs-lookup"><span data-stu-id="d1b42-137">The type of folder to be created.</span></span> <span data-ttu-id="d1b42-138">Legen Sie auf "microsoft.graph.mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="d1b42-138">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="d1b42-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d1b42-139">displayName</span></span> | <span data-ttu-id="d1b42-140">String</span><span class="sxs-lookup"><span data-stu-id="d1b42-140">String</span></span> | <span data-ttu-id="d1b42-141">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="d1b42-141">The display name of the new folder.</span></span>|
| <span data-ttu-id="d1b42-142">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="d1b42-142">includeNestedFolders</span></span> | <span data-ttu-id="d1b42-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1b42-143">Boolean</span></span> | <span data-ttu-id="d1b42-144">Wie sollte die Hierarchie der Postfach-Ordner durchlaufen werden.</span><span class="sxs-lookup"><span data-stu-id="d1b42-144">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="d1b42-145">`true`bedeutet, dass eine umfassende Suche sollte erledigen `false` bedeutet, dass eine flache Suche sollte stattdessen durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d1b42-145">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="d1b42-146">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="d1b42-146">sourceFolderIDs</span></span> | <span data-ttu-id="d1b42-147">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d1b42-147">String collection</span></span> | <span data-ttu-id="d1b42-148">Die Postfachordner, die durchsucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="d1b42-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="d1b42-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="d1b42-149">filterQuery</span></span> | <span data-ttu-id="d1b42-150">String</span><span class="sxs-lookup"><span data-stu-id="d1b42-150">String</span></span> | <span data-ttu-id="d1b42-151">Der OData-Abfrage Nachrichten gefiltert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d1b42-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="d1b42-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1b42-152">Response</span></span>

<span data-ttu-id="d1b42-153">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eines [MailSearchFolder](../resources/mailsearchfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d1b42-153">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1b42-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1b42-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d1b42-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1b42-155">Request</span></span>

<span data-ttu-id="d1b42-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1b42-156">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="d1b42-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1b42-157">Response</span></span>

<span data-ttu-id="d1b42-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d1b42-158">The following is an example of the response.</span></span>

><span data-ttu-id="d1b42-159">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d1b42-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d1b42-160">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d1b42-160">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
