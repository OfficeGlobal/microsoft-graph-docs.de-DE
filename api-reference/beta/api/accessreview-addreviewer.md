---
title: AccessReview Bearbeiter hinzufügen
description: 'In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um einen anderen Benutzer als ein Prüfer hinzuzufügen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516364"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="004ac-105">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="004ac-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="004ac-106">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um einen anderen Benutzer als ein Prüfer hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="004ac-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="004ac-107">Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="004ac-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="004ac-108">Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="004ac-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="004ac-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="004ac-109">Permissions</span></span>
<span data-ttu-id="004ac-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="004ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="004ac-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="004ac-112">Permission type</span></span>                        | <span data-ttu-id="004ac-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="004ac-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="004ac-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="004ac-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="004ac-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004ac-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="004ac-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="004ac-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="004ac-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="004ac-117">Not supported.</span></span> |
|<span data-ttu-id="004ac-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="004ac-118">Application</span></span>                            | <span data-ttu-id="004ac-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="004ac-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="004ac-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="004ac-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="004ac-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="004ac-121">Request headers</span></span>
| <span data-ttu-id="004ac-122">Name</span><span class="sxs-lookup"><span data-stu-id="004ac-122">Name</span></span>         | <span data-ttu-id="004ac-123">Typ</span><span class="sxs-lookup"><span data-stu-id="004ac-123">Type</span></span>        | <span data-ttu-id="004ac-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="004ac-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="004ac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="004ac-125">Authorization</span></span> | <span data-ttu-id="004ac-126">string</span><span class="sxs-lookup"><span data-stu-id="004ac-126">string</span></span> | <span data-ttu-id="004ac-127">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="004ac-127">Bearer \{token\}.</span></span> <span data-ttu-id="004ac-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="004ac-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="004ac-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="004ac-129">Request body</span></span>
<span data-ttu-id="004ac-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ID des Benutzers ein, die einem Bearbeiter werden.</span><span class="sxs-lookup"><span data-stu-id="004ac-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="004ac-131">In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="004ac-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="004ac-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="004ac-132">Property</span></span>     | <span data-ttu-id="004ac-133">Typ</span><span class="sxs-lookup"><span data-stu-id="004ac-133">Type</span></span>        | <span data-ttu-id="004ac-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="004ac-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="004ac-135">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="004ac-135">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="004ac-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="004ac-136">Response</span></span>
<span data-ttu-id="004ac-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="004ac-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="004ac-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="004ac-138">Example</span></span>

<span data-ttu-id="004ac-139">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung mit einer weiteren Person aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="004ac-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="004ac-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="004ac-140">Request</span></span>
<span data-ttu-id="004ac-141">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Id des User-Objekts.</span><span class="sxs-lookup"><span data-stu-id="004ac-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="004ac-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="004ac-142">Response</span></span>
><span data-ttu-id="004ac-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="004ac-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
