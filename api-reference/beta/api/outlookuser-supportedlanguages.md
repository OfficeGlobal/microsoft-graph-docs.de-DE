---
title: 'outlookUser: supportedLanguages'
description: Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.
ms.openlocfilehash: ac1b9693121f3ba3f180b53532bb6a6c917e2108
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058371"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="ca8e1-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="ca8e1-103">outlookUser: supportedLanguages</span></span>

> <span data-ttu-id="ca8e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca8e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca8e1-106">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-106">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="ca8e1-107">Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Sprache aus dieser unterstützten Liste aus.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-107">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="ca8e1-108">Sie können anschließend die bevorzugte Sprache abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ca8e1-108">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="ca8e1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ca8e1-109">Permissions</span></span>
<span data-ttu-id="ca8e1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8e1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca8e1-112">Permission type</span></span>      | <span data-ttu-id="ca8e1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca8e1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca8e1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca8e1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ca8e1-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ca8e1-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="ca8e1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca8e1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca8e1-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="ca8e1-117">User.Read</span></span>    |
|<span data-ttu-id="ca8e1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca8e1-118">Application</span></span> | <span data-ttu-id="ca8e1-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8e1-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca8e1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca8e1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="ca8e1-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca8e1-121">Request headers</span></span>
| <span data-ttu-id="ca8e1-122">Name</span><span class="sxs-lookup"><span data-stu-id="ca8e1-122">Name</span></span>       | <span data-ttu-id="ca8e1-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ca8e1-123">Type</span></span> | <span data-ttu-id="ca8e1-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca8e1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ca8e1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8e1-125">Authorization</span></span>  | <span data-ttu-id="ca8e1-126">string</span><span class="sxs-lookup"><span data-stu-id="ca8e1-126">string</span></span>  | <span data-ttu-id="ca8e1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ca8e1-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca8e1-129">Request body</span></span>
<span data-ttu-id="ca8e1-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca8e1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca8e1-131">Response</span></span>
<span data-ttu-id="ca8e1-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [localeInfo](../resources/localeinfo.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-132">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8e1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca8e1-133">Example</span></span>
<span data-ttu-id="ca8e1-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ca8e1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca8e1-135">Request</span></span>
<span data-ttu-id="ca8e1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="ca8e1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca8e1-137">Response</span></span>
<span data-ttu-id="ca8e1-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ca8e1-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->