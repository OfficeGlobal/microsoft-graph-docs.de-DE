---
title: MailSearchFolder aktualisieren
description: Aktualisieren Sie die schreibbaren Eigenschaften des MailSearchFolder-Objekts.
localization_priority: Normal
ms.openlocfilehash: 843dbe4d4312fdeb3485b0eb9e441a76b761dd46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867229"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="2d5e3-103">MailSearchFolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2d5e3-103">Update mailSearchFolder</span></span>

> <span data-ttu-id="2d5e3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d5e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d5e3-106">Aktualisieren Sie die schreibbaren Eigenschaften des [MailSearchFolder](../resources/mailsearchfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-106">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d5e3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d5e3-107">Permissions</span></span>
<span data-ttu-id="2d5e3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d5e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d5e3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d5e3-110">Permission type</span></span>      | <span data-ttu-id="2d5e3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d5e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d5e3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d5e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d5e3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d5e3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d5e3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d5e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d5e3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d5e3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d5e3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d5e3-116">Application</span></span> | <span data-ttu-id="2d5e3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d5e3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d5e3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d5e3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2d5e3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d5e3-119">Request headers</span></span>
| <span data-ttu-id="2d5e3-120">Header</span><span class="sxs-lookup"><span data-stu-id="2d5e3-120">Header</span></span>       | <span data-ttu-id="2d5e3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2d5e3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d5e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d5e3-122">Authorization</span></span>  | <span data-ttu-id="2d5e3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2d5e3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d5e3-125">Content-Type</span></span>  | <span data-ttu-id="2d5e3-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2d5e3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d5e3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d5e3-128">Request body</span></span>
<span data-ttu-id="2d5e3-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d5e3-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d5e3-132">Property</span></span>     | <span data-ttu-id="2d5e3-133">Typ</span><span class="sxs-lookup"><span data-stu-id="2d5e3-133">Type</span></span>   |<span data-ttu-id="2d5e3-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d5e3-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d5e3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2d5e3-135">displayName</span></span> | <span data-ttu-id="2d5e3-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d5e3-136">String</span></span> | <span data-ttu-id="2d5e3-137">Der Anzeigename des der [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2d5e3-137">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="2d5e3-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="2d5e3-138">includeNestedFolders</span></span> | <span data-ttu-id="2d5e3-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2d5e3-139">Boolean</span></span> | <span data-ttu-id="2d5e3-140">Wie sollte die Hierarchie der Postfach-Ordner durchlaufen werden.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-140">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="2d5e3-141">`true`bedeutet, dass eine umfassende Suche sollte erledigen `false` bedeutet, dass eine flache Suche sollte stattdessen durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="2d5e3-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="2d5e3-142">sourceFolderIDs</span></span> | <span data-ttu-id="2d5e3-143">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="2d5e3-143">String collection</span></span> | <span data-ttu-id="2d5e3-144">Die Postfachordner, die durchsucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="2d5e3-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="2d5e3-145">filterQuery</span></span> | <span data-ttu-id="2d5e3-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d5e3-146">String</span></span> | <span data-ttu-id="2d5e3-147">Der OData-Abfrage Nachrichten gefiltert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-147">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="2d5e3-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d5e3-148">Response</span></span>
<span data-ttu-id="2d5e3-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-149">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d5e3-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d5e3-150">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2d5e3-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d5e3-151">Request</span></span>
<span data-ttu-id="2d5e3-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="2d5e3-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d5e3-153">Response</span></span>
<span data-ttu-id="2d5e3-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-154">The following is an example of the response.</span></span>
><span data-ttu-id="2d5e3-155">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2d5e3-156">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2d5e3-156">All the properties will be returned from an actual call.</span></span>
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
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
