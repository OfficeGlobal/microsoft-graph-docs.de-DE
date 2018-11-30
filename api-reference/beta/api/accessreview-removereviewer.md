---
title: AccessReview Reviewer entfernen
description: 'In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um einen Benutzer als Bearbeiter zu entfernen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. '
ms.openlocfilehash: 2f2e1be904b98ed4dc2b3b34088b344e05b03473
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059652"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="af2cb-105">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="af2cb-105">Remove accessReview reviewer</span></span>

> <span data-ttu-id="af2cb-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="af2cb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af2cb-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af2cb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af2cb-108">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um einen Benutzer als Bearbeiter zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="af2cb-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="af2cb-109">Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="af2cb-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="af2cb-110">Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="af2cb-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="af2cb-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="af2cb-111">Permissions</span></span>
<span data-ttu-id="af2cb-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af2cb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af2cb-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af2cb-114">Permission type</span></span>                        | <span data-ttu-id="af2cb-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af2cb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="af2cb-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af2cb-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="af2cb-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af2cb-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="af2cb-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af2cb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af2cb-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af2cb-119">Not supported.</span></span> |
|<span data-ttu-id="af2cb-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af2cb-120">Application</span></span>                            | <span data-ttu-id="af2cb-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af2cb-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af2cb-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af2cb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="af2cb-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af2cb-123">Request headers</span></span>
| <span data-ttu-id="af2cb-124">Name</span><span class="sxs-lookup"><span data-stu-id="af2cb-124">Name</span></span>         | <span data-ttu-id="af2cb-125">Typ</span><span class="sxs-lookup"><span data-stu-id="af2cb-125">Type</span></span>        | <span data-ttu-id="af2cb-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af2cb-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="af2cb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="af2cb-127">Authorization</span></span> | <span data-ttu-id="af2cb-128">string</span><span class="sxs-lookup"><span data-stu-id="af2cb-128">string</span></span> | <span data-ttu-id="af2cb-129">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="af2cb-129">Bearer \{token\}.</span></span> <span data-ttu-id="af2cb-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="af2cb-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af2cb-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af2cb-131">Request body</span></span>
<span data-ttu-id="af2cb-132">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="af2cb-132">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="af2cb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="af2cb-133">Response</span></span>
<span data-ttu-id="af2cb-134">Wenn erfolgreich, gibt diese Methode einen Antwortcode 200-Serie.</span><span class="sxs-lookup"><span data-stu-id="af2cb-134">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="af2cb-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af2cb-135">Example</span></span>

<span data-ttu-id="af2cb-136">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access-Überprüfung zum Entfernen einer unnötige Reviewer aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="af2cb-136">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="af2cb-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af2cb-137">Request</span></span>
<span data-ttu-id="af2cb-138">Geben Sie in der Anforderungs-URL die Id des AccessReview-Objekts, und klicken Sie dann die Id des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="af2cb-138">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="af2cb-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="af2cb-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
