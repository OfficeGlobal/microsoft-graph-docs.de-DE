---
title: Team app hinzufügen
description: Installiert das angegebene Team eine app.
author: nkramer
ms.openlocfilehash: ed38f809c784c4178f7be2b028dc4c71a6206b1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349168"
---
# <a name="add-app-to-team"></a><span data-ttu-id="3b779-103">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="3b779-103">Add app to team</span></span>

> <span data-ttu-id="3b779-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b779-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b779-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b779-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b779-106">Installiert das angegebene [Team](../resources/team.md)einer [app](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3b779-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b779-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b779-107">Permissions</span></span>
<span data-ttu-id="3b779-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b779-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b779-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b779-110">Permission type</span></span>      | <span data-ttu-id="3b779-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b779-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b779-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b779-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b779-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b779-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b779-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b779-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b779-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b779-115">Not supported.</span></span>    |
|<span data-ttu-id="3b779-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b779-116">Application</span></span> | <span data-ttu-id="3b779-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b779-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b779-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b779-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="3b779-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b779-119">Request headers</span></span>
| <span data-ttu-id="3b779-120">Header</span><span class="sxs-lookup"><span data-stu-id="3b779-120">Header</span></span>       | <span data-ttu-id="3b779-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3b779-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b779-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b779-122">Authorization</span></span>  | <span data-ttu-id="3b779-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b779-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b779-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b779-125">Request body</span></span>

| <span data-ttu-id="3b779-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b779-126">Property</span></span>     | <span data-ttu-id="3b779-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3b779-127">Type</span></span>   |<span data-ttu-id="3b779-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b779-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b779-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3b779-129">teamsApp</span></span>|<span data-ttu-id="3b779-130">String</span><span class="sxs-lookup"><span data-stu-id="3b779-130">String</span></span>|<span data-ttu-id="3b779-131">Die Id der app hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="3b779-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="3b779-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b779-132">Response</span></span>

<span data-ttu-id="3b779-133">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b779-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="3b779-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b779-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3b779-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b779-135">Request</span></span>
<span data-ttu-id="3b779-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b779-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="3b779-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b779-137">Response</span></span>
<span data-ttu-id="3b779-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b779-138">The following is an example of the response.</span></span> <span data-ttu-id="3b779-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3b779-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3b779-140">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b779-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="3b779-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3b779-141">See also</span></span>

