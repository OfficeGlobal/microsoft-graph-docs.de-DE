---
title: Team app hinzufügen
description: Installiert das angegebene Team eine app.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: d3f67b8ea49f9940b60bcf0aec7eea15a59388b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855860"
---
# <a name="add-app-to-team"></a><span data-ttu-id="3b8fc-103">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="3b8fc-103">Add app to team</span></span>

> <span data-ttu-id="3b8fc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b8fc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b8fc-106">Installiert das angegebene [Team](../resources/team.md)einer [app](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3b8fc-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b8fc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b8fc-107">Permissions</span></span>
<span data-ttu-id="3b8fc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b8fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b8fc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b8fc-110">Permission type</span></span>      | <span data-ttu-id="3b8fc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b8fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b8fc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b8fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b8fc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8fc-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b8fc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b8fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b8fc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b8fc-115">Not supported.</span></span>    |
|<span data-ttu-id="3b8fc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b8fc-116">Application</span></span> | <span data-ttu-id="3b8fc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b8fc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b8fc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b8fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="3b8fc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b8fc-119">Request headers</span></span>
| <span data-ttu-id="3b8fc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3b8fc-120">Header</span></span>       | <span data-ttu-id="3b8fc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3b8fc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b8fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b8fc-122">Authorization</span></span>  | <span data-ttu-id="3b8fc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b8fc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b8fc-125">Request body</span></span>

| <span data-ttu-id="3b8fc-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b8fc-126">Property</span></span>     | <span data-ttu-id="3b8fc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3b8fc-127">Type</span></span>   |<span data-ttu-id="3b8fc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b8fc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b8fc-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3b8fc-129">teamsApp</span></span>|<span data-ttu-id="3b8fc-130">String</span><span class="sxs-lookup"><span data-stu-id="3b8fc-130">String</span></span>|<span data-ttu-id="3b8fc-131">Die Id der app hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="3b8fc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b8fc-132">Response</span></span>

<span data-ttu-id="3b8fc-133">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="3b8fc-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b8fc-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3b8fc-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b8fc-135">Request</span></span>
<span data-ttu-id="3b8fc-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="3b8fc-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b8fc-137">Response</span></span>
<span data-ttu-id="3b8fc-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-138">The following is an example of the response.</span></span> <span data-ttu-id="3b8fc-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3b8fc-140">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b8fc-140">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3b8fc-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3b8fc-141">See also</span></span>

