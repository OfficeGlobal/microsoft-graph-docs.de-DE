---
title: Erstellen von groupLifecyclePolicy
description: Erstellt ein neues groupLifecyclePolicy-Objekt.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b507454705fad4407a9cb9fef61a49e6f1bd051c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942038"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="b1bc2-103">Erstellen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b1bc2-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="b1bc2-104">Erstellt ein neues [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b1bc2-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1bc2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1bc2-105">Permissions</span></span>

<span data-ttu-id="b1bc2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1bc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1bc2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1bc2-108">Permission type</span></span>      | <span data-ttu-id="b1bc2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1bc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1bc2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1bc2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1bc2-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1bc2-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1bc2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1bc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1bc2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1bc2-113">Not supported.</span></span>    |
|<span data-ttu-id="b1bc2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1bc2-114">Application</span></span> | <span data-ttu-id="b1bc2-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1bc2-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1bc2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bc2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="b1bc2-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1bc2-117">Request headers</span></span>

| <span data-ttu-id="b1bc2-118">Name</span><span class="sxs-lookup"><span data-stu-id="b1bc2-118">Name</span></span> | <span data-ttu-id="b1bc2-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1bc2-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b1bc2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1bc2-120">Authorization</span></span> | <span data-ttu-id="b1bc2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1bc2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1bc2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1bc2-123">Content-Type</span></span>  | <span data-ttu-id="b1bc2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1bc2-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1bc2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1bc2-125">Request body</span></span>
<span data-ttu-id="b1bc2-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b1bc2-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1bc2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bc2-127">Response</span></span>

<span data-ttu-id="b1bc2-128">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `201 Created` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b1bc2-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1bc2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1bc2-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1bc2-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bc2-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="b1bc2-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b1bc2-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b1bc2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bc2-132">Response</span></span>

<span data-ttu-id="b1bc2-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1bc2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
