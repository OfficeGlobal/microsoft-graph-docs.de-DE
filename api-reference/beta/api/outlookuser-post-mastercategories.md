---
title: Erstellen der Outlook-Kategorie
description: Erstellen eines outlookCategory-Objekts in der Masterliste von Kategorien.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e76f6ddc0f733bd2e50b3aac62707acbed370ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984703"
---
# <a name="create-outlook-category"></a><span data-ttu-id="acacb-103">Erstellen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="acacb-103">Create Outlook category</span></span>

> <span data-ttu-id="acacb-104">**Wichtig**: unter der /beta Version von Microsoft Graph-APIs sind in der Vorschau und kann geändert werden.</span><span class="sxs-lookup"><span data-stu-id="acacb-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acacb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acacb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acacb-106">Erstellen eines [outlookCategory](../resources/outlookcategory.md)-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="acacb-106">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="acacb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="acacb-107">Permissions</span></span>
<span data-ttu-id="acacb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acacb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acacb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acacb-110">Permission type</span></span>      | <span data-ttu-id="acacb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acacb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acacb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acacb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="acacb-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acacb-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="acacb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acacb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acacb-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acacb-115">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="acacb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acacb-116">Application</span></span> | <span data-ttu-id="acacb-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acacb-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="acacb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acacb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="acacb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acacb-119">Request headers</span></span>
| <span data-ttu-id="acacb-120">Name</span><span class="sxs-lookup"><span data-stu-id="acacb-120">Name</span></span>       | <span data-ttu-id="acacb-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acacb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="acacb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acacb-122">Authorization</span></span>  | <span data-ttu-id="acacb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="acacb-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="acacb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acacb-125">Request body</span></span>
<span data-ttu-id="acacb-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [outlookCategory](../resources/outlookcategory.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="acacb-126">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="acacb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="acacb-127">Response</span></span>

<span data-ttu-id="acacb-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acacb-128">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acacb-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acacb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acacb-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acacb-130">Request</span></span>
<span data-ttu-id="acacb-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acacb-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="acacb-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [outlookCategory](../resources/outlookcategory.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="acacb-132">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="acacb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="acacb-133">Response</span></span>
<span data-ttu-id="acacb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acacb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
