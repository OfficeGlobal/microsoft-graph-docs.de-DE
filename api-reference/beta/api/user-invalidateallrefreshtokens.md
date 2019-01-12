---
title: 'Benutzer: InvalidateAllRefreshTokens'
description: Alle des Benutzers Aktualisierungstoken einstufen Applications (als auch Session-Cookies im Browser des Benutzers), die Benutzereigenschaft **RefreshTokensValidFromDateTime** auf das aktuelle Datum-Uhrzeit zurücksetzen ungültig macht. Dieser Vorgang wird in der Regel (durch den Benutzer oder Administrator) ausgeführt, wenn der Benutzer einem verlorenen oder gestohlenen Gerät verfügt.  Dieser Vorgang würde Zugriff auf die Organisation Daten über Anwendungen auf dem Gerät zugegriffen werden, ohne dass der Benutzer zunächst eine erneute Anmeldung erforderlich wird verhindern. Tatsächlich würden diese Operation erzwingen, dass den Benutzer erneut für alle Anwendungen anmelden, die sie zuvor, zugestimmt haben unabhängig vom Gerät.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 740829e4ebd3b64308e514ab1c7633db7f35e7d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950179"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="c5a08-106">Benutzer: InvalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="c5a08-106">user: invalidateAllRefreshTokens</span></span>

> <span data-ttu-id="c5a08-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c5a08-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5a08-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5a08-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5a08-109">Alle des Benutzers Aktualisierungstoken einstufen Applications (als auch Session-Cookies im Browser des Benutzers), die Benutzereigenschaft **RefreshTokensValidFromDateTime** auf das aktuelle Datum-Uhrzeit zurücksetzen ungültig macht.</span><span class="sxs-lookup"><span data-stu-id="c5a08-109">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="c5a08-110">Dieser Vorgang wird in der Regel (durch den Benutzer oder Administrator) ausgeführt, wenn der Benutzer einem verlorenen oder gestohlenen Gerät verfügt.</span><span class="sxs-lookup"><span data-stu-id="c5a08-110">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="c5a08-111">Dieser Vorgang würde Zugriff auf die Organisation Daten über Anwendungen auf dem Gerät zugegriffen werden, ohne dass der Benutzer zunächst eine erneute Anmeldung erforderlich wird verhindern.</span><span class="sxs-lookup"><span data-stu-id="c5a08-111">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="c5a08-112">Tatsächlich würden diese Operation erzwingen, dass den Benutzer erneut für alle Anwendungen anmelden, die sie zuvor, zugestimmt haben unabhängig vom Gerät.</span><span class="sxs-lookup"><span data-stu-id="c5a08-112">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="c5a08-113">Für Entwickler Wenn die Anwendung versucht, ein Token Delegierter Zugriff für diesen Benutzer mithilfe einer ungültig Aktualisierungstoken lösen Sie, erhalten die Anwendung einen Fehler.</span><span class="sxs-lookup"><span data-stu-id="c5a08-113">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="c5a08-114">In diesem Fall muss die Anwendung erwirbt ein neues Aktualisierungstoken durch eine Anforderung an den Endpunkt autorisieren, in der den Benutzer zur Anmeldung bei erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="c5a08-114">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5a08-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c5a08-115">Permissions</span></span>
<span data-ttu-id="c5a08-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a08-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="c5a08-118">Für eine Anwendung an Benutzer Applikationen für ungültig erklärt die signierte zulassen, die sie zum zugestimmt haben: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5a08-118">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="c5a08-119">Für eine Anwendung an Applications ungültig ein Administrator kann ein Benutzer zugestimmt hat: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5a08-119">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c5a08-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a08-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="c5a08-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5a08-121">Request headers</span></span>
| <span data-ttu-id="c5a08-122">Header</span><span class="sxs-lookup"><span data-stu-id="c5a08-122">Header</span></span>       | <span data-ttu-id="c5a08-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c5a08-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5a08-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a08-124">Authorization</span></span>  | <span data-ttu-id="c5a08-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5a08-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5a08-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5a08-127">Request body</span></span>
<span data-ttu-id="c5a08-128">Dieser Vorgang hat keine Anforderung Inhalt.</span><span class="sxs-lookup"><span data-stu-id="c5a08-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="c5a08-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a08-129">Response</span></span>

<span data-ttu-id="c5a08-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5a08-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c5a08-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5a08-131">Example</span></span>
<span data-ttu-id="c5a08-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c5a08-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5a08-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a08-133">Request</span></span>
<span data-ttu-id="c5a08-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5a08-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="c5a08-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a08-135">Response</span></span>
<span data-ttu-id="c5a08-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5a08-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
