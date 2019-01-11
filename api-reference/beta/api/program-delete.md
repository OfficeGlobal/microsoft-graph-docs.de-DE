---
title: Programm löschen
description: In Azure AD zugreifen auf Berichte-Funktion, löschen Sie ein Programmobjekt zu.
localization_priority: Normal
ms.openlocfilehash: 10b8c1e6eab7b3a42b053f854ae5f08faefc2e12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872009"
---
# <a name="delete-program"></a><span data-ttu-id="f2469-103">Programm löschen</span><span class="sxs-lookup"><span data-stu-id="f2469-103">Delete program</span></span>

> <span data-ttu-id="f2469-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f2469-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2469-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f2469-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2469-106">Löschen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [Programm](../resources/program.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="f2469-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="f2469-107">Löschen Sie ein Programm die immer noch nicht `programControl` verknüpft sein, die Access-Bewertungen müssen zuerst gelöscht oder aus dem Programm aufgehoben und zu einem anderen Programm verknüpft.</span><span class="sxs-lookup"><span data-stu-id="f2469-107">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="f2469-108">Bitte beachten Sie, dass die integrierte Anwendung kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="f2469-108">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="f2469-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2469-109">Permissions</span></span>
<span data-ttu-id="f2469-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2469-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2469-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2469-112">Permission type</span></span>                        | <span data-ttu-id="f2469-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2469-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2469-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2469-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2469-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f2469-115"></span></span>  <span data-ttu-id="f2469-116">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen eines Programms zulässt.</span><span class="sxs-lookup"><span data-stu-id="f2469-116">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="f2469-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2469-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2469-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2469-118">Not supported.</span></span> |
|<span data-ttu-id="f2469-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2469-119">Application</span></span>                            | <span data-ttu-id="f2469-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2469-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2469-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2469-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="f2469-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2469-122">Request headers</span></span>
| <span data-ttu-id="f2469-123">Name</span><span class="sxs-lookup"><span data-stu-id="f2469-123">Name</span></span>         | <span data-ttu-id="f2469-124">Typ</span><span class="sxs-lookup"><span data-stu-id="f2469-124">Type</span></span>        | <span data-ttu-id="f2469-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2469-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f2469-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2469-126">Authorization</span></span> | <span data-ttu-id="f2469-127">string</span><span class="sxs-lookup"><span data-stu-id="f2469-127">string</span></span> | <span data-ttu-id="f2469-128">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="f2469-128">Bearer \{token\}.</span></span> <span data-ttu-id="f2469-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2469-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2469-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2469-130">Request body</span></span>
<span data-ttu-id="f2469-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f2469-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f2469-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2469-132">Response</span></span>
<span data-ttu-id="f2469-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2469-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2469-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2469-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2469-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2469-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="f2469-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2469-137">Response</span></span>
><span data-ttu-id="f2469-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f2469-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
