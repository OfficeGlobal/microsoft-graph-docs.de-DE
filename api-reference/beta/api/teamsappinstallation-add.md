---
title: Team app hinzufügen
description: Installiert das angegebene Team eine app.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3f52d54850d1046d837821de1501968965678e8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990271"
---
# <a name="add-app-to-team"></a><span data-ttu-id="11727-103">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="11727-103">Add app to team</span></span>

> <span data-ttu-id="11727-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11727-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11727-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11727-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11727-106">Installiert das angegebene [Team](../resources/team.md)einer [app](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="11727-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="11727-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11727-107">Permissions</span></span>
<span data-ttu-id="11727-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11727-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11727-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11727-110">Permission type</span></span>      | <span data-ttu-id="11727-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11727-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11727-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11727-112">Delegated (work or school account)</span></span> | <span data-ttu-id="11727-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11727-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="11727-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11727-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11727-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11727-115">Not supported.</span></span>    |
|<span data-ttu-id="11727-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11727-116">Application</span></span> | <span data-ttu-id="11727-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11727-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11727-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11727-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="11727-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11727-119">Request headers</span></span>
| <span data-ttu-id="11727-120">Header</span><span class="sxs-lookup"><span data-stu-id="11727-120">Header</span></span>       | <span data-ttu-id="11727-121">Wert</span><span class="sxs-lookup"><span data-stu-id="11727-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11727-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11727-122">Authorization</span></span>  | <span data-ttu-id="11727-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11727-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11727-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11727-125">Request body</span></span>

| <span data-ttu-id="11727-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11727-126">Property</span></span>     | <span data-ttu-id="11727-127">Typ</span><span class="sxs-lookup"><span data-stu-id="11727-127">Type</span></span>   |<span data-ttu-id="11727-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11727-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11727-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="11727-129">teamsApp</span></span>|<span data-ttu-id="11727-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11727-130">String</span></span>|<span data-ttu-id="11727-131">Die Id der app hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="11727-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="11727-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="11727-132">Response</span></span>

<span data-ttu-id="11727-133">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11727-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="11727-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11727-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="11727-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11727-135">Request</span></span>
<span data-ttu-id="11727-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11727-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="11727-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="11727-137">Response</span></span>
<span data-ttu-id="11727-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11727-138">The following is an example of the response.</span></span> <span data-ttu-id="11727-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="11727-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="11727-140">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11727-140">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="11727-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="11727-141">See also</span></span>

