---
title: MailFolder erstellen
description: Mit dieser API können Sie neue E-Mail-Ordner im Stammordner des Postfachs eines Benutzers erstellen.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b4a339338063c4aa511a41eac4342b376d8bc1e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974063"
---
# <a name="create-mailfolder"></a><span data-ttu-id="58a4c-103">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="58a4c-103">Create MailFolder</span></span>

> <span data-ttu-id="58a4c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="58a4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58a4c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58a4c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58a4c-106">Mit dieser API können Sie neue E-Mail-Ordner im Stammordner des Postfachs eines Benutzers erstellen.</span><span class="sxs-lookup"><span data-stu-id="58a4c-106">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="58a4c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58a4c-107">Permissions</span></span>
<span data-ttu-id="58a4c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58a4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a4c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58a4c-110">Permission type</span></span>      | <span data-ttu-id="58a4c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58a4c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58a4c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58a4c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="58a4c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58a4c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="58a4c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58a4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58a4c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58a4c-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="58a4c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58a4c-116">Application</span></span> | <span data-ttu-id="58a4c-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58a4c-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="58a4c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58a4c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="58a4c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58a4c-119">Request headers</span></span>
| <span data-ttu-id="58a4c-120">Header</span><span class="sxs-lookup"><span data-stu-id="58a4c-120">Header</span></span>       | <span data-ttu-id="58a4c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="58a4c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="58a4c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a4c-122">Authorization</span></span>  | <span data-ttu-id="58a4c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58a4c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="58a4c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58a4c-125">Content-Type</span></span>  | <span data-ttu-id="58a4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58a4c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58a4c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58a4c-127">Request body</span></span>
<span data-ttu-id="58a4c-p104">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="58a4c-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="58a4c-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="58a4c-130">Parameter</span></span>    | <span data-ttu-id="58a4c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="58a4c-131">Type</span></span>   |<span data-ttu-id="58a4c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58a4c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58a4c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="58a4c-133">displayName</span></span>|<span data-ttu-id="58a4c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58a4c-134">String</span></span>|<span data-ttu-id="58a4c-135">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="58a4c-135">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="58a4c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="58a4c-136">Response</span></span>

<span data-ttu-id="58a4c-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58a4c-137">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a4c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58a4c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58a4c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58a4c-139">Request</span></span>
<span data-ttu-id="58a4c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58a4c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="58a4c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="58a4c-141">Response</span></span>
<span data-ttu-id="58a4c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58a4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
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
