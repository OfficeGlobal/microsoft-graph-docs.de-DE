---
title: SendReminder accessReview
description: 'Zugriff auf in Azure AD Feature Reviews (engl.), senden Sie eine Erinnerung an die Bearbeiter eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db394036a228f405a8cebb783a9279779054b04d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518548"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="3f35f-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="3f35f-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f35f-105">Senden Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion eine Erinnerung an die Bearbeiter eine derzeit aktive [AccessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="3f35f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="3f35f-106">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="3f35f-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3f35f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3f35f-107">Permissions</span></span>
<span data-ttu-id="3f35f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f35f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f35f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f35f-110">Permission type</span></span>                        | <span data-ttu-id="3f35f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f35f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f35f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f35f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f35f-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f35f-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="3f35f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f35f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f35f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f35f-115">Not supported.</span></span> |
|<span data-ttu-id="3f35f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3f35f-116">Application</span></span>                            | <span data-ttu-id="3f35f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f35f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f35f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f35f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="3f35f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f35f-119">Request headers</span></span>
| <span data-ttu-id="3f35f-120">Name</span><span class="sxs-lookup"><span data-stu-id="3f35f-120">Name</span></span>         | <span data-ttu-id="3f35f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3f35f-121">Type</span></span>        | <span data-ttu-id="3f35f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f35f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3f35f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f35f-123">Authorization</span></span> | <span data-ttu-id="3f35f-124">string</span><span class="sxs-lookup"><span data-stu-id="3f35f-124">string</span></span> | <span data-ttu-id="3f35f-125">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="3f35f-125">Bearer \{token\}.</span></span> <span data-ttu-id="3f35f-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3f35f-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f35f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3f35f-127">Request body</span></span>
<span data-ttu-id="3f35f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3f35f-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3f35f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f35f-129">Response</span></span>
<span data-ttu-id="3f35f-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f35f-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f35f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f35f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f35f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f35f-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="3f35f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f35f-134">Response</span></span>
><span data-ttu-id="3f35f-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3f35f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
