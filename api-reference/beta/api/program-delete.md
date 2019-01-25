---
title: Programm löschen
description: In Azure AD zugreifen auf Berichte-Funktion, löschen Sie ein Programmobjekt zu.
localization_priority: Normal
ms.openlocfilehash: 930367e6c61d354655e73fb7ece9c8776e15f34e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519507"
---
# <a name="delete-program"></a><span data-ttu-id="eb2bd-103">Programm löschen</span><span class="sxs-lookup"><span data-stu-id="eb2bd-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb2bd-104">Löschen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [Programm](../resources/program.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="eb2bd-105">Löschen Sie ein Programm die immer noch nicht `programControl` verknüpft sein, die Access-Bewertungen müssen zuerst gelöscht oder aus dem Programm aufgehoben und zu einem anderen Programm verknüpft.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="eb2bd-106">Bitte beachten Sie, dass die integrierte Anwendung kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="eb2bd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb2bd-107">Permissions</span></span>
<span data-ttu-id="eb2bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb2bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb2bd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb2bd-110">Permission type</span></span>                        | <span data-ttu-id="eb2bd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb2bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb2bd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb2bd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb2bd-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-113"></span></span>  <span data-ttu-id="eb2bd-114">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen eines Programms zulässt.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="eb2bd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb2bd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb2bd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb2bd-116">Not supported.</span></span> |
|<span data-ttu-id="eb2bd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb2bd-117">Application</span></span>                            | <span data-ttu-id="eb2bd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb2bd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb2bd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb2bd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="eb2bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb2bd-120">Request headers</span></span>
| <span data-ttu-id="eb2bd-121">Name</span><span class="sxs-lookup"><span data-stu-id="eb2bd-121">Name</span></span>         | <span data-ttu-id="eb2bd-122">Typ</span><span class="sxs-lookup"><span data-stu-id="eb2bd-122">Type</span></span>        | <span data-ttu-id="eb2bd-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb2bd-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eb2bd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb2bd-124">Authorization</span></span> | <span data-ttu-id="eb2bd-125">string</span><span class="sxs-lookup"><span data-stu-id="eb2bd-125">string</span></span> | <span data-ttu-id="eb2bd-126">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="eb2bd-126">Bearer \{token\}.</span></span> <span data-ttu-id="eb2bd-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb2bd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb2bd-128">Request body</span></span>
<span data-ttu-id="eb2bd-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="eb2bd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb2bd-130">Response</span></span>
<span data-ttu-id="eb2bd-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb2bd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb2bd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb2bd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb2bd-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="eb2bd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb2bd-135">Response</span></span>
><span data-ttu-id="eb2bd-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="eb2bd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
