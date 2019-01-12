---
title: SendReminder accessReview
description: 'Zugriff auf in Azure AD Feature Reviews (engl.), senden Sie eine Erinnerung an die Bearbeiter eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cf5b78d2c67993fbf2da9be7c55a07fb752985c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917279"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="7a5b9-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="7a5b9-104">SendReminder accessReview</span></span>

> <span data-ttu-id="7a5b9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a5b9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a5b9-107">Senden Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion eine Erinnerung an die Bearbeiter eine derzeit aktive [AccessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="7a5b9-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="7a5b9-108">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7a5b9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7a5b9-109">Permissions</span></span>
<span data-ttu-id="7a5b9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a5b9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a5b9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a5b9-112">Permission type</span></span>                        | <span data-ttu-id="7a5b9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a5b9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a5b9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a5b9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a5b9-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a5b9-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7a5b9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a5b9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a5b9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a5b9-117">Not supported.</span></span> |
|<span data-ttu-id="7a5b9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a5b9-118">Application</span></span>                            | <span data-ttu-id="7a5b9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a5b9-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a5b9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a5b9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="7a5b9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a5b9-121">Request headers</span></span>
| <span data-ttu-id="7a5b9-122">Name</span><span class="sxs-lookup"><span data-stu-id="7a5b9-122">Name</span></span>         | <span data-ttu-id="7a5b9-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7a5b9-123">Type</span></span>        | <span data-ttu-id="7a5b9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a5b9-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7a5b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a5b9-125">Authorization</span></span> | <span data-ttu-id="7a5b9-126">string</span><span class="sxs-lookup"><span data-stu-id="7a5b9-126">string</span></span> | <span data-ttu-id="7a5b9-127">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-127">Bearer \{token\}.</span></span> <span data-ttu-id="7a5b9-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a5b9-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a5b9-129">Request body</span></span>
<span data-ttu-id="7a5b9-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7a5b9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a5b9-131">Response</span></span>
<span data-ttu-id="7a5b9-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a5b9-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a5b9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a5b9-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a5b9-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="7a5b9-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a5b9-136">Response</span></span>
><span data-ttu-id="7a5b9-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7a5b9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
