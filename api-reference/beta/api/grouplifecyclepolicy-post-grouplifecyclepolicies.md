---
title: Erstellen von groupLifecyclePolicy
description: Erstellt ein neues groupLifecyclePolicy-Objekt.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b4fe572e67d0b55ea4ee7adb431f5c0705c9b6db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959454"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="7bda0-103">Erstellen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bda0-103">Create groupLifecyclePolicy</span></span>

> <span data-ttu-id="7bda0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7bda0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bda0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7bda0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7bda0-106">Erstellt ein neues [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7bda0-106">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bda0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7bda0-107">Permissions</span></span>

<span data-ttu-id="7bda0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bda0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7bda0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7bda0-110">Permission type</span></span>      | <span data-ttu-id="7bda0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7bda0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bda0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7bda0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7bda0-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bda0-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bda0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7bda0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bda0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bda0-115">Not supported</span></span> |
|<span data-ttu-id="7bda0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7bda0-116">Application</span></span> |  <span data-ttu-id="7bda0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bda0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bda0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bda0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="7bda0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7bda0-119">Request headers</span></span>

| <span data-ttu-id="7bda0-120">Name</span><span class="sxs-lookup"><span data-stu-id="7bda0-120">Name</span></span> | <span data-ttu-id="7bda0-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bda0-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7bda0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bda0-122">Authorization</span></span> | <span data-ttu-id="7bda0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7bda0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bda0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bda0-125">Content-Type</span></span>  | <span data-ttu-id="7bda0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bda0-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bda0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7bda0-127">Request body</span></span>
<span data-ttu-id="7bda0-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7bda0-128">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7bda0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bda0-129">Response</span></span>

<span data-ttu-id="7bda0-130">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `201 Created` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7bda0-130">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bda0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7bda0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7bda0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bda0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="7bda0-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7bda0-133">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7bda0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bda0-134">Response</span></span>

<span data-ttu-id="7bda0-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bda0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
