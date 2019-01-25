---
title: AccessReview zurücksetzen
description: In der Azure AD-Zugriff zurücksetzen Bewertungen-Funktion, die Entscheidungen der eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  Frühere Entscheidungen werden nicht mehr aufgezeichnet, aber Bearbeiter können weiterhin Entscheidungen zu aktualisieren.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e258a781707d2c3fe5419e3ebd5f7c6b43f271b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517015"
---
# <a name="reset-accessreview"></a><span data-ttu-id="9c3a7-105">AccessReview zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="9c3a7-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c3a7-106">Klicken Sie in Azure AD Feature [Access überprüft](../resources/accessreviews-root.md) die Entscheidungen der eine derzeit aktive [AccessReview](../resources/accessreview.md)zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="9c3a7-107">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="9c3a7-108">Frühere Entscheidungen werden nicht mehr aufgezeichnet, aber Bearbeiter können weiterhin Entscheidungen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c3a7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c3a7-109">Permissions</span></span>
<span data-ttu-id="9c3a7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c3a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c3a7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c3a7-112">Permission type</span></span>                        | <span data-ttu-id="9c3a7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c3a7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c3a7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c3a7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c3a7-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3a7-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9c3a7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c3a7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c3a7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c3a7-117">Not supported.</span></span> |
|<span data-ttu-id="9c3a7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c3a7-118">Application</span></span>                            | <span data-ttu-id="9c3a7-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c3a7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c3a7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c3a7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="9c3a7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c3a7-121">Request headers</span></span>
| <span data-ttu-id="9c3a7-122">Name</span><span class="sxs-lookup"><span data-stu-id="9c3a7-122">Name</span></span>         | <span data-ttu-id="9c3a7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9c3a7-123">Type</span></span>        | <span data-ttu-id="9c3a7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c3a7-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9c3a7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c3a7-125">Authorization</span></span> | <span data-ttu-id="9c3a7-126">string</span><span class="sxs-lookup"><span data-stu-id="9c3a7-126">string</span></span> | <span data-ttu-id="9c3a7-127">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="9c3a7-127">Bearer \{token\}.</span></span> <span data-ttu-id="9c3a7-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c3a7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c3a7-129">Request body</span></span>
<span data-ttu-id="9c3a7-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9c3a7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c3a7-131">Response</span></span>
<span data-ttu-id="9c3a7-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c3a7-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c3a7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c3a7-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c3a7-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="9c3a7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c3a7-136">Response</span></span>
><span data-ttu-id="9c3a7-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9c3a7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
