---
title: Anwenden von accessReview
description: 'In Azure AD zugreifen auf Berichte-Funktion, anwenden Sie die Entscheidungen von einer abgeschlossenen AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e230a9638e865fbca69448f3a7683b95db954598
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951333"
---
# <a name="apply-accessreview"></a><span data-ttu-id="85117-104">Anwenden von accessReview</span><span class="sxs-lookup"><span data-stu-id="85117-104">Apply accessReview</span></span>

> <span data-ttu-id="85117-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85117-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85117-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85117-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85117-107">Gelten Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature die Entscheidungen von einer abgeschlossenen [AccessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="85117-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="85117-108">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="85117-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="85117-109">Nach Abschluss eine Access-Überprüfung entweder, da es das Enddatum erreicht oder ein Administrator manuell angehalten, und automatisch zugewiesenes wurde nicht konfiguriert für die Überprüfung können Sie aufrufen, übernehmen, um die Änderungen zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="85117-109">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="85117-110">Bis übernehmen auftritt, erscheinen die Entscheidungen Zugriffsrechte entfernen nicht für die Ressource Quelle die Benutzer ihrer Gruppenmitgliedschaften für die Instanz beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="85117-110">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="85117-111">Durch Aufrufen von anwendbar sind, wird das Ergebnis der Überprüfung durch Aktualisieren der Gruppe oder einer Anwendung implementiert.</span><span class="sxs-lookup"><span data-stu-id="85117-111">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="85117-112">Wenn Sie den Zugriff eines Benutzers bei der Überprüfung verweigert wurde, wenn ein Administrator diese API aufruft, entfernt Azure AD ihre Aufgaben Mitgliedschaft oder der Anwendung an.</span><span class="sxs-lookup"><span data-stu-id="85117-112">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="85117-113">Nach eine Access-Überprüfung abgeschlossen ist, und automatisch zugewiesenes wurde so konfiguriert, und klicken Sie dann der Status der Überprüfung von abgeschlossen durch intermediate Zustände geändert und schließlich Applied Status geändert wird.</span><span class="sxs-lookup"><span data-stu-id="85117-113">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="85117-114">Sie sollten verweigerte Benutzer sehen erwarten, wenn vorhanden, wird von der Ressource entfernt Mitgliedschaft oder app-Zuordnung in ein paar Minuten gruppieren.</span><span class="sxs-lookup"><span data-stu-id="85117-114">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="85117-115">Eine konfigurierte automatische Überprüfung anwenden, oder übernehmen auswählen keinen Effekt auf eine Gruppe, die in einem lokalen Verzeichnis stammt oder eine dynamische Gruppe.</span><span class="sxs-lookup"><span data-stu-id="85117-115">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="85117-116">Wenn Sie eine Gruppe ändern, die lokalen stammt möchten, laden Sie die Ergebnisse und gelten Sie diese Änderungen für die Darstellung der Gruppe in dieses Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="85117-116">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="85117-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="85117-117">Permissions</span></span>
<span data-ttu-id="85117-p107">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85117-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85117-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85117-120">Permission type</span></span>                        | <span data-ttu-id="85117-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85117-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="85117-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85117-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="85117-123">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85117-123">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="85117-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85117-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85117-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85117-125">Not supported.</span></span> |
|<span data-ttu-id="85117-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85117-126">Application</span></span>                            | <span data-ttu-id="85117-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85117-127">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85117-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85117-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="85117-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85117-129">Request headers</span></span>
| <span data-ttu-id="85117-130">Name</span><span class="sxs-lookup"><span data-stu-id="85117-130">Name</span></span>         | <span data-ttu-id="85117-131">Typ</span><span class="sxs-lookup"><span data-stu-id="85117-131">Type</span></span>        | <span data-ttu-id="85117-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85117-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85117-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="85117-133">Authorization</span></span> | <span data-ttu-id="85117-134">string</span><span class="sxs-lookup"><span data-stu-id="85117-134">string</span></span> | <span data-ttu-id="85117-135">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="85117-135">Bearer \{token\}.</span></span> <span data-ttu-id="85117-136">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85117-136">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85117-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85117-137">Request body</span></span>
<span data-ttu-id="85117-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85117-138">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="85117-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="85117-139">Response</span></span>
<span data-ttu-id="85117-p109">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85117-p109">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="85117-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="85117-142">See also</span></span>

- [<span data-ttu-id="85117-143">Wie Sie für die Durchführung eine Access-Überprüfung</span><span class="sxs-lookup"><span data-stu-id="85117-143">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="85117-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85117-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85117-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85117-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="85117-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="85117-146">Response</span></span>
><span data-ttu-id="85117-p110">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="85117-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
