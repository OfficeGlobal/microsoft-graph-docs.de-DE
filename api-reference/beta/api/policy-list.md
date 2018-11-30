---
title: Listenrichtlinien
description: Rufen Sie aller Gruppenrichtlinienobjekte im Verzeichnis ab.
ms.openlocfilehash: 5abff0973a53dc3bddfd256dbc43faad519e20e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065274"
---
# <a name="list-policies"></a><span data-ttu-id="118b7-103">Listenrichtlinien</span><span class="sxs-lookup"><span data-stu-id="118b7-103">List Policies</span></span>

> <span data-ttu-id="118b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="118b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="118b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="118b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="118b7-106">Rufen Sie [aller Gruppenrichtlinienobjekte im Verzeichnis ab](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="118b7-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="118b7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="118b7-107">Permissions</span></span>
<span data-ttu-id="118b7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="118b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="118b7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="118b7-110">Permission type</span></span>      | <span data-ttu-id="118b7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="118b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="118b7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="118b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="118b7-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="118b7-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="118b7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="118b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="118b7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="118b7-115">Not supported.</span></span>    |
|<span data-ttu-id="118b7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="118b7-116">Application</span></span> | <span data-ttu-id="118b7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="118b7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="118b7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="118b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="118b7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="118b7-119">Request headers</span></span>
| <span data-ttu-id="118b7-120">Name</span><span class="sxs-lookup"><span data-stu-id="118b7-120">Name</span></span>       | <span data-ttu-id="118b7-121">Typ</span><span class="sxs-lookup"><span data-stu-id="118b7-121">Type</span></span> | <span data-ttu-id="118b7-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="118b7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="118b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="118b7-123">Authorization</span></span>  | <span data-ttu-id="118b7-124">string</span><span class="sxs-lookup"><span data-stu-id="118b7-124">string</span></span>  | <span data-ttu-id="118b7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="118b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="118b7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="118b7-127">Request body</span></span>
<span data-ttu-id="118b7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="118b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="118b7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="118b7-129">Response</span></span>

<span data-ttu-id="118b7-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekte Code und [Richtlinie](../resources/policy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="118b7-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="118b7-131">Wenn Sie nicht erfolgreich...</span><span class="sxs-lookup"><span data-stu-id="118b7-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="118b7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="118b7-132">Example</span></span>
<span data-ttu-id="118b7-133">Im folgende Beispiel werden alle Richtlinien abgerufen.</span><span class="sxs-lookup"><span data-stu-id="118b7-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="118b7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="118b7-134">Request</span></span>
<span data-ttu-id="118b7-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="118b7-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="118b7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="118b7-136">Response</span></span>
<span data-ttu-id="118b7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="118b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
