---
title: Apps im Team auflisten
description: Ruft die Liste der im angegebenen Team installierten apps ab.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 749a0c0e0c3a93b54487d9dea8823ad59a2658fd
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057008"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="93f38-103">Apps im Team auflisten</span><span class="sxs-lookup"><span data-stu-id="93f38-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f38-104">Ruft die Liste der im angegebenen [Team](../resources/team.md) [installierten apps](../resources/teamsappinstallation.md) ab.</span><span class="sxs-lookup"><span data-stu-id="93f38-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93f38-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93f38-105">Permissions</span></span>

<span data-ttu-id="93f38-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f38-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93f38-108">Permission type</span></span>      | <span data-ttu-id="93f38-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93f38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f38-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93f38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93f38-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f38-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93f38-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93f38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93f38-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93f38-113">Not supported.</span></span>    |
|<span data-ttu-id="93f38-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93f38-114">Application</span></span> | <span data-ttu-id="93f38-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f38-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="93f38-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93f38-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93f38-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="93f38-117">Optional query parameters</span></span>

<span data-ttu-id="93f38-118">Diese Methode unterstützt die $filter, $select und $expand [OData-Abfrageparameter](/graph/query-parameters) , um die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="93f38-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93f38-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93f38-119">Request headers</span></span>

| <span data-ttu-id="93f38-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="93f38-120">Header</span></span>       | <span data-ttu-id="93f38-121">Wert</span><span class="sxs-lookup"><span data-stu-id="93f38-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93f38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93f38-122">Authorization</span></span>  | <span data-ttu-id="93f38-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93f38-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93f38-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93f38-125">Request body</span></span>

<span data-ttu-id="93f38-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93f38-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93f38-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="93f38-127">Response</span></span>

<span data-ttu-id="93f38-128">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [teamsApp](../resources/teamsapp.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="93f38-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93f38-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93f38-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="93f38-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93f38-130">Request</span></span>

<span data-ttu-id="93f38-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93f38-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="93f38-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="93f38-132">Response</span></span>

<span data-ttu-id="93f38-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93f38-133">The following is an example of the response.</span></span>
><span data-ttu-id="93f38-134">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="93f38-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93f38-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="93f38-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="93f38-136">Beispiel: Aufrufen der Namen der installierten apps</span><span class="sxs-lookup"><span data-stu-id="93f38-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="93f38-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93f38-137">Request</span></span>

<span data-ttu-id="93f38-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93f38-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="93f38-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="93f38-139">Response</span></span>

<span data-ttu-id="93f38-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93f38-140">The following is an example of the response.</span></span>

><span data-ttu-id="93f38-141">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="93f38-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93f38-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="93f38-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
