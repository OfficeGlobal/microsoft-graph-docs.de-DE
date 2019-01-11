---
title: ProgramControl löschen
description: In Azure AD zugreifen auf Berichte-Funktion, löschen Sie ein ProgramControl-Objekt zu.  Dies hebt die Verknüpfung mit einer Access-Überprüfung aus einem Programm.
localization_priority: Normal
ms.openlocfilehash: 782cc8f336e84f82d937e3180d7de6af69e67e52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843918"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="0623b-104">ProgramControl löschen</span><span class="sxs-lookup"><span data-stu-id="0623b-104">Delete programControl</span></span>

> <span data-ttu-id="0623b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0623b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0623b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0623b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0623b-107">Löschen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [ProgramControl](../resources/programcontrol.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="0623b-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="0623b-108">Dies hebt die Verknüpfung mit einer Access-Überprüfung aus einem Programm.</span><span class="sxs-lookup"><span data-stu-id="0623b-108">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="0623b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0623b-109">Permissions</span></span>
<span data-ttu-id="0623b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0623b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0623b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0623b-112">Permission type</span></span>                        | <span data-ttu-id="0623b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0623b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0623b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0623b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0623b-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="0623b-115"></span></span>  <span data-ttu-id="0623b-116">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Löschen einer ProgramControl zulässt.</span><span class="sxs-lookup"><span data-stu-id="0623b-116">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="0623b-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0623b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0623b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0623b-118">Not supported.</span></span> |
|<span data-ttu-id="0623b-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0623b-119">Application</span></span>                            | <span data-ttu-id="0623b-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0623b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0623b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0623b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="0623b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0623b-122">Request headers</span></span>
| <span data-ttu-id="0623b-123">Name</span><span class="sxs-lookup"><span data-stu-id="0623b-123">Name</span></span>         | <span data-ttu-id="0623b-124">Typ</span><span class="sxs-lookup"><span data-stu-id="0623b-124">Type</span></span>        | <span data-ttu-id="0623b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0623b-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0623b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0623b-126">Authorization</span></span> | <span data-ttu-id="0623b-127">string</span><span class="sxs-lookup"><span data-stu-id="0623b-127">string</span></span> | <span data-ttu-id="0623b-128">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="0623b-128">Bearer \{token\}.</span></span> <span data-ttu-id="0623b-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0623b-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0623b-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0623b-130">Request body</span></span>
<span data-ttu-id="0623b-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0623b-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0623b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0623b-132">Response</span></span>
<span data-ttu-id="0623b-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0623b-p107">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0623b-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0623b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0623b-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0623b-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="0623b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="0623b-137">Response</span></span>
><span data-ttu-id="0623b-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0623b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
