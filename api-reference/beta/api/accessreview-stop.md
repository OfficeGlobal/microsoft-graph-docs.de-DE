---
title: AccessReview beenden
description: In Azure AD Access Feature überprüft, und beenden Sie eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  (Um zu verhindern, dass sich wiederholenden Access Wiederholung zukünftige Instanzen starten, aktualisieren Sie, um die geplante Enddatum ändern).  Überprüfen Sie nach dem Zugriff wird beendet, Bearbeiter können nicht mehr liefern Input und die Zugriff überprüfen Entscheidungen angewendet werden können.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d71796272cf9852683688a47f3d78eebd849357
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941464"
---
# <a name="stop-accessreview"></a><span data-ttu-id="023cf-106">AccessReview beenden</span><span class="sxs-lookup"><span data-stu-id="023cf-106">Stop accessReview</span></span>

> <span data-ttu-id="023cf-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="023cf-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="023cf-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="023cf-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="023cf-109">Beenden Sie eine derzeit aktive [AccessReview](../resources/accessreview.md)in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="023cf-109">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="023cf-110">Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.</span><span class="sxs-lookup"><span data-stu-id="023cf-110">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="023cf-111">(Sie wiederkehrende Access Wiederholung verhindern, dass zukünftige Instanzen, so ändern Sie das Enddatum des geplanten [Aktualisieren](accessreview-update.md) ).</span><span class="sxs-lookup"><span data-stu-id="023cf-111">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="023cf-112">Überprüfen Sie nach dem Zugriff wird beendet, Bearbeiter können nicht mehr liefern Input und die Zugriff überprüfen Entscheidungen angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="023cf-112">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="023cf-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="023cf-113">Permissions</span></span>
<span data-ttu-id="023cf-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="023cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="023cf-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="023cf-116">Permission type</span></span>                        | <span data-ttu-id="023cf-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="023cf-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="023cf-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="023cf-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="023cf-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="023cf-119">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="023cf-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="023cf-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="023cf-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="023cf-121">Not supported.</span></span> |
|<span data-ttu-id="023cf-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="023cf-122">Application</span></span>                            | <span data-ttu-id="023cf-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="023cf-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="023cf-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="023cf-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="023cf-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="023cf-125">Request headers</span></span>
| <span data-ttu-id="023cf-126">Name</span><span class="sxs-lookup"><span data-stu-id="023cf-126">Name</span></span>         | <span data-ttu-id="023cf-127">Typ</span><span class="sxs-lookup"><span data-stu-id="023cf-127">Type</span></span>        | <span data-ttu-id="023cf-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="023cf-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="023cf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="023cf-129">Authorization</span></span> | <span data-ttu-id="023cf-130">string</span><span class="sxs-lookup"><span data-stu-id="023cf-130">string</span></span> | <span data-ttu-id="023cf-131">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="023cf-131">Bearer \{token\}.</span></span> <span data-ttu-id="023cf-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="023cf-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="023cf-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="023cf-133">Request body</span></span>
<span data-ttu-id="023cf-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="023cf-134">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="023cf-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="023cf-135">Response</span></span>
<span data-ttu-id="023cf-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="023cf-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="023cf-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="023cf-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="023cf-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="023cf-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="023cf-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="023cf-140">Response</span></span>
><span data-ttu-id="023cf-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="023cf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
