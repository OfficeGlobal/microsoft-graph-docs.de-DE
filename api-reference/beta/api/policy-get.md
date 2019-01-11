---
title: Abrufen von Gruppenrichtlinien
description: Rufen Sie die Eigenschaften einer Richtlinie ab.
localization_priority: Normal
ms.openlocfilehash: 9b3e23639bdeea673ccbe56bbce0c74443a99480
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870595"
---
# <a name="get-policy"></a><span data-ttu-id="bd915-103">Abrufen von Gruppenrichtlinien</span><span class="sxs-lookup"><span data-stu-id="bd915-103">Get Policy</span></span>

> <span data-ttu-id="bd915-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd915-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd915-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd915-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd915-106">Rufen Sie die Eigenschaften einer [Richtlinie](../resources/policy.md)ab.</span><span class="sxs-lookup"><span data-stu-id="bd915-106">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd915-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd915-107">Permissions</span></span>
<span data-ttu-id="bd915-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd915-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd915-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd915-110">Permission type</span></span>      | <span data-ttu-id="bd915-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd915-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd915-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd915-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bd915-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd915-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd915-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd915-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd915-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd915-115">Not supported.</span></span>    |
|<span data-ttu-id="bd915-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd915-116">Application</span></span> | <span data-ttu-id="bd915-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd915-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd915-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd915-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bd915-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd915-119">Request headers</span></span>
| <span data-ttu-id="bd915-120">Name</span><span class="sxs-lookup"><span data-stu-id="bd915-120">Name</span></span>       | <span data-ttu-id="bd915-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bd915-121">Type</span></span> | <span data-ttu-id="bd915-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd915-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bd915-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd915-123">Authorization</span></span>  | <span data-ttu-id="bd915-124">string</span><span class="sxs-lookup"><span data-stu-id="bd915-124">string</span></span>  | <span data-ttu-id="bd915-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd915-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd915-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd915-127">Request body</span></span>
<span data-ttu-id="bd915-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bd915-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd915-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd915-129">Response</span></span>

<span data-ttu-id="bd915-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [Sie ein Gruppenrichtlinienobjekt in der Antworttext](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="bd915-130">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="bd915-131">Wenn Unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="bd915-131">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="bd915-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd915-132">Example</span></span>
<span data-ttu-id="bd915-133">Das folgende Beispiel ruft eine bestimmte Richtlinie ab.</span><span class="sxs-lookup"><span data-stu-id="bd915-133">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="bd915-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd915-134">Request</span></span>
<span data-ttu-id="bd915-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd915-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="bd915-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd915-136">Response</span></span>
<span data-ttu-id="bd915-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd915-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
