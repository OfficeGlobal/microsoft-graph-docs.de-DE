---
title: AccessReview beenden
description: In Azure AD Access Feature überprüft, und beenden Sie eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  (Um zu verhindern, dass sich wiederholenden Access Wiederholung zukünftige Instanzen starten, aktualisieren Sie, um die geplante Enddatum ändern).  Überprüfen Sie nach dem Zugriff wird beendet, Bearbeiter können nicht mehr liefern Input und die Zugriff überprüfen Entscheidungen angewendet werden können.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 070f91faa411fcc6d98db419d1683a7fb6493859
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521838"
---
# <a name="stop-accessreview"></a><span data-ttu-id="e3b01-106">AccessReview beenden</span><span class="sxs-lookup"><span data-stu-id="e3b01-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3b01-107">Beenden Sie eine derzeit aktive [AccessReview](../resources/accessreview.md)in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="e3b01-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="e3b01-108">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="e3b01-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="e3b01-109">(Sie wiederkehrende Access Wiederholung verhindern, dass zukünftige Instanzen, so ändern Sie das Enddatum des geplanten [Aktualisieren](accessreview-update.md) ).</span><span class="sxs-lookup"><span data-stu-id="e3b01-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="e3b01-110">Überprüfen Sie nach dem Zugriff wird beendet, Bearbeiter können nicht mehr liefern Input und die Zugriff überprüfen Entscheidungen angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e3b01-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3b01-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3b01-111">Permissions</span></span>
<span data-ttu-id="e3b01-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3b01-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3b01-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3b01-114">Permission type</span></span>                        | <span data-ttu-id="e3b01-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3b01-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3b01-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3b01-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3b01-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3b01-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e3b01-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3b01-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b01-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3b01-119">Not supported.</span></span> |
|<span data-ttu-id="e3b01-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3b01-120">Application</span></span>                            | <span data-ttu-id="e3b01-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3b01-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3b01-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3b01-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="e3b01-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3b01-123">Request headers</span></span>
| <span data-ttu-id="e3b01-124">Name</span><span class="sxs-lookup"><span data-stu-id="e3b01-124">Name</span></span>         | <span data-ttu-id="e3b01-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e3b01-125">Type</span></span>        | <span data-ttu-id="e3b01-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3b01-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3b01-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b01-127">Authorization</span></span> | <span data-ttu-id="e3b01-128">string</span><span class="sxs-lookup"><span data-stu-id="e3b01-128">string</span></span> | <span data-ttu-id="e3b01-129">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="e3b01-129">Bearer \{token\}.</span></span> <span data-ttu-id="e3b01-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3b01-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3b01-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3b01-131">Request body</span></span>
<span data-ttu-id="e3b01-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3b01-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e3b01-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3b01-133">Response</span></span>
<span data-ttu-id="e3b01-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3b01-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3b01-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3b01-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3b01-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3b01-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="e3b01-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3b01-138">Response</span></span>
><span data-ttu-id="e3b01-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e3b01-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
