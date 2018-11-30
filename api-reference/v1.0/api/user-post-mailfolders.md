---
title: MailFolder erstellen
description: Mit dieser API können Sie neue E-Mail-Ordner im Stammordner des Postfachs eines Benutzers erstellen.
ms.openlocfilehash: 5ab8870de334781b59e68cb1d090db5067d53796
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018004"
---
# <a name="create-mailfolder"></a><span data-ttu-id="38484-103">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="38484-103">Create MailFolder</span></span>

<span data-ttu-id="38484-104">Mit dieser API können Sie neue E-Mail-Ordner im Stammordner des Postfachs eines Benutzers erstellen.</span><span class="sxs-lookup"><span data-stu-id="38484-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="38484-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38484-105">Permissions</span></span>
<span data-ttu-id="38484-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38484-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38484-108">Permission type</span></span>      | <span data-ttu-id="38484-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38484-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38484-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38484-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38484-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38484-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="38484-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38484-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38484-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38484-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="38484-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38484-114">Application</span></span> | <span data-ttu-id="38484-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38484-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="38484-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38484-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="38484-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38484-117">Request headers</span></span>
| <span data-ttu-id="38484-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38484-118">Header</span></span>       | <span data-ttu-id="38484-119">Wert</span><span class="sxs-lookup"><span data-stu-id="38484-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38484-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38484-120">Authorization</span></span>  | <span data-ttu-id="38484-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38484-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="38484-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38484-123">Content-Type</span></span>  | <span data-ttu-id="38484-124">application/json</span><span class="sxs-lookup"><span data-stu-id="38484-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38484-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38484-125">Request body</span></span>
<span data-ttu-id="38484-p103">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="38484-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="38484-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="38484-128">Parameter</span></span>    | <span data-ttu-id="38484-129">Typ</span><span class="sxs-lookup"><span data-stu-id="38484-129">Type</span></span>   |<span data-ttu-id="38484-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38484-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38484-131">displayName</span><span class="sxs-lookup"><span data-stu-id="38484-131">displayName</span></span>|<span data-ttu-id="38484-132">String</span><span class="sxs-lookup"><span data-stu-id="38484-132">String</span></span>|<span data-ttu-id="38484-133">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="38484-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="38484-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="38484-134">Response</span></span>

<span data-ttu-id="38484-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38484-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38484-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38484-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38484-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38484-137">Request</span></span>
<span data-ttu-id="38484-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38484-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="38484-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="38484-139">Response</span></span>
<span data-ttu-id="38484-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38484-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
