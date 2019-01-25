---
title: Team app hinzufügen
description: Installiert das angegebene Team eine app.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 353298dc43479057e689f43e3a7274523468caee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516826"
---
# <a name="add-app-to-team"></a><span data-ttu-id="0fab3-103">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0fab3-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fab3-104">Installiert das angegebene [Team](../resources/team.md)einer [app](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0fab3-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fab3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0fab3-105">Permissions</span></span>
<span data-ttu-id="0fab3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fab3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0fab3-108">Permission type</span></span>      | <span data-ttu-id="0fab3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0fab3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fab3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0fab3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0fab3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fab3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fab3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0fab3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fab3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fab3-113">Not supported.</span></span>    |
|<span data-ttu-id="0fab3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0fab3-114">Application</span></span> | <span data-ttu-id="0fab3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fab3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fab3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fab3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="0fab3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0fab3-117">Request headers</span></span>
| <span data-ttu-id="0fab3-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0fab3-118">Header</span></span>       | <span data-ttu-id="0fab3-119">Wert</span><span class="sxs-lookup"><span data-stu-id="0fab3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fab3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fab3-120">Authorization</span></span>  | <span data-ttu-id="0fab3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fab3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fab3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0fab3-123">Request body</span></span>

| <span data-ttu-id="0fab3-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fab3-124">Property</span></span>     | <span data-ttu-id="0fab3-125">Typ</span><span class="sxs-lookup"><span data-stu-id="0fab3-125">Type</span></span>   |<span data-ttu-id="0fab3-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fab3-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fab3-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0fab3-127">teamsApp</span></span>|<span data-ttu-id="0fab3-128">String</span><span class="sxs-lookup"><span data-stu-id="0fab3-128">String</span></span>|<span data-ttu-id="0fab3-129">Die Id der app hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="0fab3-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="0fab3-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fab3-130">Response</span></span>

<span data-ttu-id="0fab3-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fab3-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="0fab3-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fab3-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0fab3-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fab3-133">Request</span></span>
<span data-ttu-id="0fab3-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0fab3-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="0fab3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fab3-135">Response</span></span>
<span data-ttu-id="0fab3-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0fab3-136">The following is an example of the response.</span></span> <span data-ttu-id="0fab3-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="0fab3-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0fab3-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fab3-138">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="0fab3-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0fab3-139">See also</span></span>

