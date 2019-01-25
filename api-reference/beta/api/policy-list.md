---
title: Listenrichtlinien
description: Rufen Sie aller Gruppenrichtlinienobjekte im Verzeichnis ab.
localization_priority: Normal
ms.openlocfilehash: 292eb457b87629d0034b97b3c781d75adc0da4e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510022"
---
# <a name="list-policies"></a><span data-ttu-id="040c1-103">Listenrichtlinien</span><span class="sxs-lookup"><span data-stu-id="040c1-103">List Policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="040c1-104">Rufen Sie [aller Gruppenrichtlinienobjekte im Verzeichnis ab](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="040c1-104">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="040c1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="040c1-105">Permissions</span></span>
<span data-ttu-id="040c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="040c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="040c1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="040c1-108">Permission type</span></span>      | <span data-ttu-id="040c1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="040c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="040c1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="040c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="040c1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="040c1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="040c1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="040c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="040c1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="040c1-113">Not supported.</span></span>    |
|<span data-ttu-id="040c1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="040c1-114">Application</span></span> | <span data-ttu-id="040c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="040c1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="040c1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="040c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="040c1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="040c1-117">Request headers</span></span>
| <span data-ttu-id="040c1-118">Name</span><span class="sxs-lookup"><span data-stu-id="040c1-118">Name</span></span>       | <span data-ttu-id="040c1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="040c1-119">Type</span></span> | <span data-ttu-id="040c1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="040c1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="040c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="040c1-121">Authorization</span></span>  | <span data-ttu-id="040c1-122">string</span><span class="sxs-lookup"><span data-stu-id="040c1-122">string</span></span>  | <span data-ttu-id="040c1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="040c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="040c1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="040c1-125">Request body</span></span>
<span data-ttu-id="040c1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="040c1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="040c1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="040c1-127">Response</span></span>

<span data-ttu-id="040c1-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekte Code und [Richtlinie](../resources/policy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="040c1-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="040c1-129">Wenn Sie nicht erfolgreich...</span><span class="sxs-lookup"><span data-stu-id="040c1-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="040c1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="040c1-130">Example</span></span>
<span data-ttu-id="040c1-131">Im folgende Beispiel werden alle Richtlinien abgerufen.</span><span class="sxs-lookup"><span data-stu-id="040c1-131">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="040c1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="040c1-132">Request</span></span>
<span data-ttu-id="040c1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="040c1-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="040c1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="040c1-134">Response</span></span>
<span data-ttu-id="040c1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="040c1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
