---
title: MailFolder aktualisieren
description: Aktualisieren Sie die Eigenschaften des MailFolder-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f9b0af67b4fdedbf6ecbbcfe591057a4aeb86351
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873899"
---
# <a name="update-mailfolder"></a><span data-ttu-id="20750-103">MailFolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="20750-103">Update mailFolder</span></span>

> <span data-ttu-id="20750-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="20750-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20750-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20750-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20750-106">Aktualisieren Sie die Eigenschaften des [MailFolder](../resources/mailfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="20750-106">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20750-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="20750-107">Permissions</span></span>
<span data-ttu-id="20750-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20750-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20750-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20750-110">Permission type</span></span>      | <span data-ttu-id="20750-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20750-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20750-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20750-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20750-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20750-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="20750-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20750-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20750-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20750-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="20750-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20750-116">Application</span></span> | <span data-ttu-id="20750-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20750-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="20750-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20750-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20750-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20750-119">Request headers</span></span>
| <span data-ttu-id="20750-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="20750-120">Header</span></span>       | <span data-ttu-id="20750-121">Wert</span><span class="sxs-lookup"><span data-stu-id="20750-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="20750-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20750-122">Authorization</span></span>  | <span data-ttu-id="20750-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="20750-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="20750-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20750-125">Content-Type</span></span>  | <span data-ttu-id="20750-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="20750-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="20750-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20750-128">Request body</span></span>
<span data-ttu-id="20750-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="20750-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="20750-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20750-132">Property</span></span>     | <span data-ttu-id="20750-133">Typ</span><span class="sxs-lookup"><span data-stu-id="20750-133">Type</span></span>   |<span data-ttu-id="20750-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20750-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20750-135">displayName</span><span class="sxs-lookup"><span data-stu-id="20750-135">displayName</span></span>|<span data-ttu-id="20750-136">String</span><span class="sxs-lookup"><span data-stu-id="20750-136">String</span></span>|<span data-ttu-id="20750-137">Der Anzeigename des mailFolder-Elements.</span><span class="sxs-lookup"><span data-stu-id="20750-137">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="20750-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="20750-138">Response</span></span>
<span data-ttu-id="20750-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20750-139">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20750-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20750-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="20750-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20750-141">Request</span></span>
<span data-ttu-id="20750-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20750-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="20750-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="20750-143">Response</span></span>
<span data-ttu-id="20750-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="20750-144">The following is an example of the response.</span></span>
><span data-ttu-id="20750-145">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="20750-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="20750-146">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="20750-146">All the properties will be returned from an actual call.</span></span>
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
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
