---
title: 'Meldung: Melden Sie sich ab'
description: Fordert die e-Mail im Namen des angemeldeten Benutzers an eine e-Mail-Verteilerliste kündigen. Verwendet die Informationen in der `List-Unsubscribe` Kopfzeile.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f66c24e2900ca4c881d08a402698dacbaf5af5f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877686"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="24d87-104">Meldung: Melden Sie sich ab</span><span class="sxs-lookup"><span data-stu-id="24d87-104">message: unsubscribe</span></span>

> <span data-ttu-id="24d87-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="24d87-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24d87-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24d87-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24d87-107">Fordert die e-Mail im Namen des angemeldeten Benutzers an eine e-Mail-Verteilerliste kündigen.</span><span class="sxs-lookup"><span data-stu-id="24d87-107">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="24d87-108">Verwendet die Informationen in der `List-Unsubscribe` Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="24d87-108">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="24d87-109">Absender einer Nachricht können Adressenlisten benutzerfreundliche durch das Einbeziehen von einer Option für die Empfänger um zu kündigen. Hierzu können sie angeben die `List-Unsubscribe` Kopfzeile in jede Nachricht [RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)folgen.</span><span class="sxs-lookup"><span data-stu-id="24d87-109">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="24d87-110">**Hinweis** Insbesondere für die Aktion **sich abzumelden** funktioniert der Absender muss festlegen `mailto:` und nicht URL-basierte melden Sie sich Informationen ab.</span><span class="sxs-lookup"><span data-stu-id="24d87-110">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="24d87-111">Durch Festlegen dieser Kopfzeile würde Legen Sie auch die **UnsubscribeEnabled** -Eigenschaft der [Nachricht](../resources/message.md) Instanz mit `true`, und die **UnsubscribeData** -Eigenschaft auf die Kopfzeilendaten.</span><span class="sxs-lookup"><span data-stu-id="24d87-111">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="24d87-112">Wenn die **UnsubscribeEnabled** -Eigenschaft einer Nachricht `true`, können Sie die Aktion **Melden Sie sich ab** , um die Benutzer ähnliche zukünftige Nachrichten zu kündigen, wie durch den Absender der Nachricht verwaltet.</span><span class="sxs-lookup"><span data-stu-id="24d87-112">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="24d87-113">Eine Aktion erfolgreich **Kündigen des Abonnements** wird die Nachricht in den Ordner **Gelöschte Objekte** verschoben.</span><span class="sxs-lookup"><span data-stu-id="24d87-113">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="24d87-114">Der tatsächliche Ausschluss des Benutzers aus der zukünftigen Mail Verteilung wird vom Absender verwaltet.</span><span class="sxs-lookup"><span data-stu-id="24d87-114">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="24d87-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24d87-115">Permissions</span></span>
<span data-ttu-id="24d87-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24d87-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d87-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24d87-118">Permission type</span></span>      | <span data-ttu-id="24d87-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24d87-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24d87-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24d87-120">Delegated (work or school account)</span></span> | <span data-ttu-id="24d87-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24d87-121">Mail.Send</span></span>    |
|<span data-ttu-id="24d87-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24d87-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24d87-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24d87-123">Mail.Send</span></span>    |
|<span data-ttu-id="24d87-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24d87-124">Application</span></span> | <span data-ttu-id="24d87-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24d87-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="24d87-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24d87-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="24d87-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24d87-127">Request headers</span></span>
| <span data-ttu-id="24d87-128">Name</span><span class="sxs-lookup"><span data-stu-id="24d87-128">Name</span></span>       | <span data-ttu-id="24d87-129">Typ</span><span class="sxs-lookup"><span data-stu-id="24d87-129">Type</span></span> | <span data-ttu-id="24d87-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24d87-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24d87-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d87-131">Authorization</span></span>  | <span data-ttu-id="24d87-132">string</span><span class="sxs-lookup"><span data-stu-id="24d87-132">string</span></span>  | <span data-ttu-id="24d87-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24d87-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24d87-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24d87-135">Request body</span></span>
<span data-ttu-id="24d87-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="24d87-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24d87-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="24d87-137">Response</span></span>

<span data-ttu-id="24d87-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24d87-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24d87-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24d87-140">Example</span></span>
<span data-ttu-id="24d87-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="24d87-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24d87-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24d87-142">Request</span></span>
<span data-ttu-id="24d87-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24d87-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="24d87-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="24d87-144">Response</span></span>
<span data-ttu-id="24d87-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24d87-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
