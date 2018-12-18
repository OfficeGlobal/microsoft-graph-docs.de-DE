---
title: DDE-Kanal löschen
description: Löschen Sie den Kanal.
author: nkramer
ms.openlocfilehash: e3500c536deca45b7444e149477c399cf1609a52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359556"
---
# <a name="delete-channel"></a><span data-ttu-id="74cf8-103">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="74cf8-103">Delete channel</span></span>



<span data-ttu-id="74cf8-104">Löschen Sie den [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="74cf8-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="74cf8-105">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="74cf8-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="74cf8-106">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="74cf8-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="74cf8-107">**Hinweis**: die Daten in der gelöschten Kanäle weiterhin Wochen Teambesitzer Wiederherstellung gelöschter Kanal zulassen gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="74cf8-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="74cf8-108">Während dieser Zeit kann ein neuer Kanal mit der gleichen DisplayName nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="74cf8-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="74cf8-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74cf8-109">Permissions</span></span>
<span data-ttu-id="74cf8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74cf8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74cf8-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74cf8-112">Permission type</span></span>      | <span data-ttu-id="74cf8-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74cf8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74cf8-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74cf8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="74cf8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74cf8-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="74cf8-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74cf8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74cf8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74cf8-117">Not supported.</span></span>    |
|<span data-ttu-id="74cf8-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74cf8-118">Application</span></span> | <span data-ttu-id="74cf8-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74cf8-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="74cf8-120">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="74cf8-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="74cf8-121">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="74cf8-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="74cf8-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74cf8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="74cf8-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74cf8-123">Request headers</span></span>
| <span data-ttu-id="74cf8-124">Header</span><span class="sxs-lookup"><span data-stu-id="74cf8-124">Header</span></span>       | <span data-ttu-id="74cf8-125">Wert</span><span class="sxs-lookup"><span data-stu-id="74cf8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74cf8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="74cf8-126">Authorization</span></span>  | <span data-ttu-id="74cf8-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74cf8-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74cf8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74cf8-129">Request body</span></span>
<span data-ttu-id="74cf8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="74cf8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74cf8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="74cf8-131">Response</span></span>

<span data-ttu-id="74cf8-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74cf8-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74cf8-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74cf8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74cf8-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74cf8-135">Request</span></span>
<span data-ttu-id="74cf8-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74cf8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="74cf8-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="74cf8-137">Response</span></span>

<span data-ttu-id="74cf8-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74cf8-138">The following is an example of the response.</span></span> 
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
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
