---
title: Team app hinzufügen
description: Installiert das angegebene Team eine app.
author: nkramer
ms.openlocfilehash: 41682d1280b9aaa76f6ef09d0b5ddbd5338d110f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302002"
---
# <a name="add-app-to-team"></a><span data-ttu-id="82966-103">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="82966-103">Add app to team</span></span>



<span data-ttu-id="82966-104">Installiert das angegebene [Team](../resources/team.md)einer [app](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="82966-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="82966-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="82966-105">Permissions</span></span>
<span data-ttu-id="82966-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82966-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82966-108">Permission type</span></span>      | <span data-ttu-id="82966-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82966-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82966-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82966-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82966-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82966-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82966-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82966-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82966-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82966-113">Not supported.</span></span>    |
|<span data-ttu-id="82966-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82966-114">Application</span></span> | <span data-ttu-id="82966-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82966-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82966-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82966-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="82966-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82966-117">Request headers</span></span>
| <span data-ttu-id="82966-118">Header</span><span class="sxs-lookup"><span data-stu-id="82966-118">Header</span></span>       | <span data-ttu-id="82966-119">Wert</span><span class="sxs-lookup"><span data-stu-id="82966-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82966-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="82966-120">Authorization</span></span>  | <span data-ttu-id="82966-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82966-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82966-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82966-123">Request body</span></span>

| <span data-ttu-id="82966-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82966-124">Property</span></span>     | <span data-ttu-id="82966-125">Typ</span><span class="sxs-lookup"><span data-stu-id="82966-125">Type</span></span>   |<span data-ttu-id="82966-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82966-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82966-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="82966-127">teamsApp</span></span>| [<span data-ttu-id="82966-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="82966-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="82966-129">Die app hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="82966-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="82966-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="82966-130">Response</span></span>

<span data-ttu-id="82966-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82966-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82966-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82966-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="82966-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82966-133">Request</span></span>
<span data-ttu-id="82966-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82966-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST /teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="82966-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="82966-135">Response</span></span>
<span data-ttu-id="82966-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="82966-136">The following is an example of the response.</span></span> <span data-ttu-id="82966-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="82966-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="82966-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82966-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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

## <a name="see-also"></a><span data-ttu-id="82966-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="82966-139">See also</span></span>

