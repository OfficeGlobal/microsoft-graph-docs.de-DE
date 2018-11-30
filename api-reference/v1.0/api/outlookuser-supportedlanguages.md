---
title: 'outlookUser: supportedLanguages'
description: Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.
ms.openlocfilehash: 18913deffa71ceec8ddd0df96fee6236b8f31832
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018744"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="a470f-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="a470f-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="a470f-104">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="a470f-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="a470f-105">Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Sprache aus dieser unterstützten Liste aus.</span><span class="sxs-lookup"><span data-stu-id="a470f-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="a470f-106">Sie können anschließend die bevorzugte Sprache abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a470f-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="a470f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a470f-107">Permissions</span></span>
<span data-ttu-id="a470f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a470f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a470f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a470f-110">Permission type</span></span>      | <span data-ttu-id="a470f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a470f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a470f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a470f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a470f-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="a470f-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="a470f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a470f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a470f-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="a470f-115">User.Read</span></span>    |
|<span data-ttu-id="a470f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a470f-116">Application</span></span> | <span data-ttu-id="a470f-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a470f-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a470f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a470f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="a470f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a470f-119">Request headers</span></span>
| <span data-ttu-id="a470f-120">Name</span><span class="sxs-lookup"><span data-stu-id="a470f-120">Name</span></span>       | <span data-ttu-id="a470f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a470f-121">Type</span></span> | <span data-ttu-id="a470f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a470f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a470f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a470f-123">Authorization</span></span>  | <span data-ttu-id="a470f-124">string</span><span class="sxs-lookup"><span data-stu-id="a470f-124">string</span></span>  | <span data-ttu-id="a470f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a470f-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a470f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a470f-127">Request body</span></span>
<span data-ttu-id="a470f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a470f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a470f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a470f-129">Response</span></span>
<span data-ttu-id="a470f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [localeInfo](../resources/localeinfo.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a470f-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a470f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a470f-131">Example</span></span>
<span data-ttu-id="a470f-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a470f-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a470f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a470f-133">Request</span></span>
<span data-ttu-id="a470f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a470f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="a470f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a470f-135">Response</span></span>
<span data-ttu-id="a470f-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a470f-136">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
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