---
title: 'outlookUser: supportedLanguages'
description: Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7898bc48d436c0d4b71b9c911802ecc348592245
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510722"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="9fb9c-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="9fb9c-103">outlookUser: supportedLanguages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fb9c-104">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="9fb9c-105">Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Sprache aus dieser unterstützten Liste aus.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="9fb9c-106">Sie können anschließend die bevorzugte Sprache abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="9fb9c-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="9fb9c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9fb9c-107">Permissions</span></span>
<span data-ttu-id="9fb9c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb9c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9fb9c-110">Permission type</span></span>      | <span data-ttu-id="9fb9c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9fb9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fb9c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9fb9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9fb9c-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="9fb9c-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="9fb9c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9fb9c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb9c-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="9fb9c-115">User.Read</span></span>    |
|<span data-ttu-id="9fb9c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9fb9c-116">Application</span></span> | <span data-ttu-id="9fb9c-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fb9c-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb9c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb9c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="9fb9c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9fb9c-119">Request headers</span></span>
| <span data-ttu-id="9fb9c-120">Name</span><span class="sxs-lookup"><span data-stu-id="9fb9c-120">Name</span></span>       | <span data-ttu-id="9fb9c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb9c-121">Type</span></span> | <span data-ttu-id="9fb9c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb9c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9fb9c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fb9c-123">Authorization</span></span>  | <span data-ttu-id="9fb9c-124">string</span><span class="sxs-lookup"><span data-stu-id="9fb9c-124">string</span></span>  | <span data-ttu-id="9fb9c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9fb9c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9fb9c-127">Request body</span></span>
<span data-ttu-id="9fb9c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fb9c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb9c-129">Response</span></span>
<span data-ttu-id="9fb9c-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [localeInfo](../resources/localeinfo.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fb9c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9fb9c-131">Example</span></span>
<span data-ttu-id="9fb9c-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9fb9c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb9c-133">Request</span></span>
<span data-ttu-id="9fb9c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="9fb9c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb9c-135">Response</span></span>
<span data-ttu-id="9fb9c-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9fb9c-136">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-supportedlanguages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
