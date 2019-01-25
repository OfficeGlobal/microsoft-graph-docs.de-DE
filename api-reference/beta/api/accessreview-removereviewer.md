---
title: AccessReview Reviewer entfernen
description: 'In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um einen Benutzer als Bearbeiter zu entfernen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b6ea0fecb6b9179f40fa185aa770a743776eaa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523127"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="53c03-105">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="53c03-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53c03-106">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um einen Benutzer als Bearbeiter zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="53c03-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="53c03-107">Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="53c03-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="53c03-108">Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="53c03-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="53c03-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53c03-109">Permissions</span></span>
<span data-ttu-id="53c03-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c03-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53c03-112">Permission type</span></span>                        | <span data-ttu-id="53c03-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53c03-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="53c03-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53c03-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="53c03-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c03-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="53c03-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53c03-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53c03-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53c03-117">Not supported.</span></span> |
|<span data-ttu-id="53c03-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53c03-118">Application</span></span>                            | <span data-ttu-id="53c03-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53c03-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53c03-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53c03-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="53c03-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53c03-121">Request headers</span></span>
| <span data-ttu-id="53c03-122">Name</span><span class="sxs-lookup"><span data-stu-id="53c03-122">Name</span></span>         | <span data-ttu-id="53c03-123">Typ</span><span class="sxs-lookup"><span data-stu-id="53c03-123">Type</span></span>        | <span data-ttu-id="53c03-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53c03-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53c03-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53c03-125">Authorization</span></span> | <span data-ttu-id="53c03-126">string</span><span class="sxs-lookup"><span data-stu-id="53c03-126">string</span></span> | <span data-ttu-id="53c03-127">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="53c03-127">Bearer \{token\}.</span></span> <span data-ttu-id="53c03-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53c03-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53c03-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53c03-129">Request body</span></span>
<span data-ttu-id="53c03-130">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="53c03-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="53c03-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="53c03-131">Response</span></span>
<span data-ttu-id="53c03-132">Wenn erfolgreich, gibt diese Methode einen Antwortcode 200-Serie.</span><span class="sxs-lookup"><span data-stu-id="53c03-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="53c03-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53c03-133">Example</span></span>

<span data-ttu-id="53c03-134">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access-Überprüfung zum Entfernen einer unnötige Reviewer aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="53c03-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="53c03-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53c03-135">Request</span></span>
<span data-ttu-id="53c03-136">Geben Sie in der Anforderungs-URL die Id des AccessReview-Objekts, und klicken Sie dann die Id des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="53c03-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="53c03-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="53c03-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
