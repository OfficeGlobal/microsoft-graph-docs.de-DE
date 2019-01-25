---
title: Anwenden von accessReview
description: 'In Azure AD zugreifen auf Berichte-Funktion, anwenden Sie die Entscheidungen von einer abgeschlossenen AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512213"
---
# <a name="apply-accessreview"></a><span data-ttu-id="28b94-104">Anwenden von accessReview</span><span class="sxs-lookup"><span data-stu-id="28b94-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b94-105">Gelten Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature die Entscheidungen von einer abgeschlossenen [AccessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="28b94-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="28b94-106">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="28b94-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="28b94-107">Nach Abschluss eine Access-Überprüfung entweder, da es das Enddatum erreicht oder ein Administrator manuell angehalten, und automatisch zugewiesenes wurde nicht konfiguriert für die Überprüfung können Sie aufrufen, übernehmen, um die Änderungen zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="28b94-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="28b94-108">Bis übernehmen auftritt, erscheinen die Entscheidungen Zugriffsrechte entfernen nicht für die Ressource Quelle die Benutzer ihrer Gruppenmitgliedschaften für die Instanz beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="28b94-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="28b94-109">Durch Aufrufen von anwendbar sind, wird das Ergebnis der Überprüfung durch Aktualisieren der Gruppe oder einer Anwendung implementiert.</span><span class="sxs-lookup"><span data-stu-id="28b94-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="28b94-110">Wenn Sie den Zugriff eines Benutzers bei der Überprüfung verweigert wurde, wenn ein Administrator diese API aufruft, entfernt Azure AD ihre Aufgaben Mitgliedschaft oder der Anwendung an.</span><span class="sxs-lookup"><span data-stu-id="28b94-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="28b94-111">Nach eine Access-Überprüfung abgeschlossen ist, und automatisch zugewiesenes wurde so konfiguriert, und klicken Sie dann der Status der Überprüfung von abgeschlossen durch intermediate Zustände geändert und schließlich Applied Status geändert wird.</span><span class="sxs-lookup"><span data-stu-id="28b94-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="28b94-112">Sie sollten verweigerte Benutzer sehen erwarten, wenn vorhanden, wird von der Ressource entfernt Mitgliedschaft oder app-Zuordnung in ein paar Minuten gruppieren.</span><span class="sxs-lookup"><span data-stu-id="28b94-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="28b94-113">Eine konfigurierte automatische Überprüfung anwenden, oder übernehmen auswählen keinen Effekt auf eine Gruppe, die in einem lokalen Verzeichnis stammt oder eine dynamische Gruppe.</span><span class="sxs-lookup"><span data-stu-id="28b94-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="28b94-114">Wenn Sie eine Gruppe ändern, die lokalen stammt möchten, laden Sie die Ergebnisse und gelten Sie diese Änderungen für die Darstellung der Gruppe in dieses Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="28b94-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="28b94-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="28b94-115">Permissions</span></span>
<span data-ttu-id="28b94-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b94-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28b94-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28b94-118">Permission type</span></span>                        | <span data-ttu-id="28b94-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28b94-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="28b94-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28b94-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="28b94-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28b94-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="28b94-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28b94-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b94-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28b94-123">Not supported.</span></span> |
|<span data-ttu-id="28b94-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28b94-124">Application</span></span>                            | <span data-ttu-id="28b94-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28b94-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b94-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28b94-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="28b94-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28b94-127">Request headers</span></span>
| <span data-ttu-id="28b94-128">Name</span><span class="sxs-lookup"><span data-stu-id="28b94-128">Name</span></span>         | <span data-ttu-id="28b94-129">Typ</span><span class="sxs-lookup"><span data-stu-id="28b94-129">Type</span></span>        | <span data-ttu-id="28b94-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28b94-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="28b94-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="28b94-131">Authorization</span></span> | <span data-ttu-id="28b94-132">string</span><span class="sxs-lookup"><span data-stu-id="28b94-132">string</span></span> | <span data-ttu-id="28b94-133">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="28b94-133">Bearer \{token\}.</span></span> <span data-ttu-id="28b94-134">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28b94-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28b94-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28b94-135">Request body</span></span>
<span data-ttu-id="28b94-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="28b94-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="28b94-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="28b94-137">Response</span></span>
<span data-ttu-id="28b94-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28b94-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="28b94-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="28b94-140">See also</span></span>

- [<span data-ttu-id="28b94-141">Wie Sie für die Durchführung eine Access-Überprüfung</span><span class="sxs-lookup"><span data-stu-id="28b94-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="28b94-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28b94-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28b94-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28b94-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="28b94-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="28b94-144">Response</span></span>
><span data-ttu-id="28b94-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="28b94-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
