---
title: SendReminder accessReview
description: 'Zugriff auf in Azure AD Feature Reviews (engl.), senden Sie eine Erinnerung an die Bearbeiter eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein. '
localization_priority: Normal
ms.openlocfilehash: 3fa5c648a1b159a54560ad03f70a4f0251624119
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844198"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="ba204-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="ba204-104">SendReminder accessReview</span></span>

> <span data-ttu-id="ba204-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ba204-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba204-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba204-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba204-107">Senden Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion eine Erinnerung an die Bearbeiter eine derzeit aktive [AccessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="ba204-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="ba204-108">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="ba204-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ba204-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ba204-109">Permissions</span></span>
<span data-ttu-id="ba204-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba204-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba204-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba204-112">Permission type</span></span>                        | <span data-ttu-id="ba204-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba204-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba204-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba204-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba204-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba204-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ba204-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba204-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba204-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba204-117">Not supported.</span></span> |
|<span data-ttu-id="ba204-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba204-118">Application</span></span>                            | <span data-ttu-id="ba204-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba204-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba204-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba204-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="ba204-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba204-121">Request headers</span></span>
| <span data-ttu-id="ba204-122">Name</span><span class="sxs-lookup"><span data-stu-id="ba204-122">Name</span></span>         | <span data-ttu-id="ba204-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ba204-123">Type</span></span>        | <span data-ttu-id="ba204-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba204-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ba204-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba204-125">Authorization</span></span> | <span data-ttu-id="ba204-126">string</span><span class="sxs-lookup"><span data-stu-id="ba204-126">string</span></span> | <span data-ttu-id="ba204-127">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="ba204-127">Bearer \{token\}.</span></span> <span data-ttu-id="ba204-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ba204-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba204-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba204-129">Request body</span></span>
<span data-ttu-id="ba204-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ba204-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ba204-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba204-131">Response</span></span>
<span data-ttu-id="ba204-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba204-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba204-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba204-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba204-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba204-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="ba204-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba204-136">Response</span></span>
><span data-ttu-id="ba204-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ba204-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
