---
title: AccessReview zurücksetzen
description: In der Azure AD-Zugriff zurücksetzen Bewertungen-Funktion, die Entscheidungen der eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  Frühere Entscheidungen werden nicht mehr aufgezeichnet, aber Bearbeiter können weiterhin Entscheidungen zu aktualisieren.
ms.openlocfilehash: b633a56926b56b33c509214d7574971056831967
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059349"
---
# <a name="reset-accessreview"></a><span data-ttu-id="307cc-105">AccessReview zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="307cc-105">Reset accessReview</span></span>

> <span data-ttu-id="307cc-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="307cc-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="307cc-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="307cc-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="307cc-108">Klicken Sie in Azure AD Feature [Access überprüft](../resources/accessreviews-root.md) die Entscheidungen der eine derzeit aktive [AccessReview](../resources/accessreview.md)zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="307cc-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="307cc-109">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="307cc-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="307cc-110">Frühere Entscheidungen werden nicht mehr aufgezeichnet, aber Bearbeiter können weiterhin Entscheidungen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="307cc-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="307cc-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="307cc-111">Permissions</span></span>
<span data-ttu-id="307cc-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="307cc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="307cc-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="307cc-114">Permission type</span></span>                        | <span data-ttu-id="307cc-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="307cc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="307cc-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="307cc-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="307cc-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="307cc-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="307cc-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="307cc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="307cc-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="307cc-119">Not supported.</span></span> |
|<span data-ttu-id="307cc-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="307cc-120">Application</span></span>                            | <span data-ttu-id="307cc-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="307cc-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="307cc-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="307cc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="307cc-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="307cc-123">Request headers</span></span>
| <span data-ttu-id="307cc-124">Name</span><span class="sxs-lookup"><span data-stu-id="307cc-124">Name</span></span>         | <span data-ttu-id="307cc-125">Typ</span><span class="sxs-lookup"><span data-stu-id="307cc-125">Type</span></span>        | <span data-ttu-id="307cc-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="307cc-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="307cc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="307cc-127">Authorization</span></span> | <span data-ttu-id="307cc-128">string</span><span class="sxs-lookup"><span data-stu-id="307cc-128">string</span></span> | <span data-ttu-id="307cc-129">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="307cc-129">Bearer \{token\}.</span></span> <span data-ttu-id="307cc-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="307cc-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="307cc-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="307cc-131">Request body</span></span>
<span data-ttu-id="307cc-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="307cc-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="307cc-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="307cc-133">Response</span></span>
<span data-ttu-id="307cc-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="307cc-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="307cc-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="307cc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="307cc-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="307cc-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="307cc-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="307cc-138">Response</span></span>
><span data-ttu-id="307cc-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="307cc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
