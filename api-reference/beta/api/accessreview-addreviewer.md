---
title: AccessReview Bearbeiter hinzufügen
description: 'In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um einen anderen Benutzer als ein Prüfer hinzuzufügen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a7745cf6424f3aa8b9bca16f4db961801d203431
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956864"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="c752e-105">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c752e-105">Add accessReview reviewer</span></span>

> <span data-ttu-id="c752e-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c752e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c752e-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c752e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c752e-108">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um einen anderen Benutzer als ein Prüfer hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="c752e-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="c752e-109">Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c752e-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="c752e-110">Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="c752e-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c752e-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c752e-111">Permissions</span></span>
<span data-ttu-id="c752e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c752e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c752e-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c752e-114">Permission type</span></span>                        | <span data-ttu-id="c752e-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c752e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c752e-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c752e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c752e-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c752e-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c752e-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c752e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c752e-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c752e-119">Not supported.</span></span> |
|<span data-ttu-id="c752e-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c752e-120">Application</span></span>                            | <span data-ttu-id="c752e-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c752e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c752e-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c752e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="c752e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c752e-123">Request headers</span></span>
| <span data-ttu-id="c752e-124">Name</span><span class="sxs-lookup"><span data-stu-id="c752e-124">Name</span></span>         | <span data-ttu-id="c752e-125">Typ</span><span class="sxs-lookup"><span data-stu-id="c752e-125">Type</span></span>        | <span data-ttu-id="c752e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c752e-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c752e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c752e-127">Authorization</span></span> | <span data-ttu-id="c752e-128">string</span><span class="sxs-lookup"><span data-stu-id="c752e-128">string</span></span> | <span data-ttu-id="c752e-129">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="c752e-129">Bearer \{token\}.</span></span> <span data-ttu-id="c752e-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c752e-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c752e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c752e-131">Request body</span></span>
<span data-ttu-id="c752e-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ID des Benutzers ein, die einem Bearbeiter werden.</span><span class="sxs-lookup"><span data-stu-id="c752e-132">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="c752e-133">In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="c752e-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="c752e-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c752e-134">Property</span></span>     | <span data-ttu-id="c752e-135">Typ</span><span class="sxs-lookup"><span data-stu-id="c752e-135">Type</span></span>        | <span data-ttu-id="c752e-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c752e-136">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="c752e-137">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="c752e-137">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="c752e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c752e-138">Response</span></span>
<span data-ttu-id="c752e-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="c752e-139">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="c752e-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c752e-140">Example</span></span>

<span data-ttu-id="c752e-141">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung mit einer weiteren Person aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c752e-141">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="c752e-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c752e-142">Request</span></span>
<span data-ttu-id="c752e-143">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Id des User-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c752e-143">In the request body, supply a JSON representation of the id of the user object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c752e-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="c752e-144">Response</span></span>
><span data-ttu-id="c752e-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c752e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
