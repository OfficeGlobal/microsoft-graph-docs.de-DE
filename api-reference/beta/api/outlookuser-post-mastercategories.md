---
title: Erstellen der Outlook-Kategorie
description: Erstellen eines outlookCategory-Objekts in der Masterliste von Kategorien.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b9cf9ed2ca82e2f676ae1241f64ce361e0004437
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519941"
---
# <a name="create-outlook-category"></a><span data-ttu-id="baef1-103">Erstellen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="baef1-103">Create Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baef1-104">Erstellen eines [outlookCategory](../resources/outlookcategory.md)-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="baef1-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="baef1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="baef1-105">Permissions</span></span>
<span data-ttu-id="baef1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baef1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="baef1-108">Permission type</span></span>      | <span data-ttu-id="baef1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="baef1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baef1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="baef1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="baef1-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baef1-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="baef1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="baef1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baef1-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baef1-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="baef1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="baef1-114">Application</span></span> | <span data-ttu-id="baef1-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baef1-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="baef1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="baef1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="baef1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="baef1-117">Request headers</span></span>
| <span data-ttu-id="baef1-118">Name</span><span class="sxs-lookup"><span data-stu-id="baef1-118">Name</span></span>       | <span data-ttu-id="baef1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="baef1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="baef1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="baef1-120">Authorization</span></span>  | <span data-ttu-id="baef1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="baef1-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="baef1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="baef1-123">Request body</span></span>
<span data-ttu-id="baef1-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [outlookCategory](../resources/outlookcategory.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="baef1-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="baef1-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="baef1-125">Response</span></span>

<span data-ttu-id="baef1-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="baef1-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baef1-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="baef1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baef1-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="baef1-128">Request</span></span>
<span data-ttu-id="baef1-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="baef1-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="baef1-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [outlookCategory](../resources/outlookcategory.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="baef1-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="baef1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="baef1-131">Response</span></span>
<span data-ttu-id="baef1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="baef1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
  "tocPath": "".
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-mastercategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
