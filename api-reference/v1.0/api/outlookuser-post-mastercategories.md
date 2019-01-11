---
title: Erstellen der Outlook-Kategorie
description: Erstellen eines outlookCategory-Objekts in der Masterliste von Kategorien.
localization_priority: Normal
ms.openlocfilehash: 71bb00d96119b06fda624b02fa9b64be67313f6e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815379"
---
# <a name="create-outlook-category"></a><span data-ttu-id="f3a5e-103">Erstellen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="f3a5e-103">Create Outlook category</span></span>


<span data-ttu-id="f3a5e-104">Erstellen eines [outlookCategory](../resources/outlookcategory.md)-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3a5e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f3a5e-105">Permissions</span></span>
<span data-ttu-id="f3a5e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3a5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a5e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3a5e-108">Permission type</span></span>      | <span data-ttu-id="f3a5e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3a5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3a5e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3a5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3a5e-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3a5e-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f3a5e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3a5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3a5e-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3a5e-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="f3a5e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3a5e-114">Application</span></span> | <span data-ttu-id="f3a5e-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3a5e-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3a5e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3a5e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="f3a5e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3a5e-117">Request headers</span></span>
| <span data-ttu-id="f3a5e-118">Name</span><span class="sxs-lookup"><span data-stu-id="f3a5e-118">Name</span></span>       | <span data-ttu-id="f3a5e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3a5e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3a5e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3a5e-120">Authorization</span></span>  | <span data-ttu-id="f3a5e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f3a5e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3a5e-123">Request body</span></span>
<span data-ttu-id="f3a5e-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [outlookCategory](../resources/outlookcategory.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f3a5e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3a5e-125">Response</span></span>

<span data-ttu-id="f3a5e-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a5e-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3a5e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3a5e-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3a5e-128">Request</span></span>
<span data-ttu-id="f3a5e-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="f3a5e-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [outlookCategory](../resources/outlookcategory.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f3a5e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3a5e-131">Response</span></span>
<span data-ttu-id="f3a5e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3a5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
