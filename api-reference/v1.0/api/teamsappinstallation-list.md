---
title: Liste apps im team
description: Abrufen der Liste apps im angegebenen Team installiert.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3289f7abc80e20a11d38c9ab35a9961981b81dd1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985732"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="ab808-103">Liste apps im team</span><span class="sxs-lookup"><span data-stu-id="ab808-103">List apps in team</span></span>



<span data-ttu-id="ab808-104">Abrufen der Liste der in das angegebene [Team](../resources/team.md) [apps installiert](../resources/teamsappinstallation.md) .</span><span class="sxs-lookup"><span data-stu-id="ab808-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab808-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ab808-105">Permissions</span></span>

<span data-ttu-id="ab808-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab808-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab808-108">Permission type</span></span>      | <span data-ttu-id="ab808-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab808-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab808-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab808-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab808-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab808-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab808-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab808-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab808-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab808-113">Not supported.</span></span>    |
|<span data-ttu-id="ab808-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab808-114">Application</span></span> | <span data-ttu-id="ab808-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab808-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab808-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab808-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab808-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ab808-117">Optional query parameters</span></span>

<span data-ttu-id="ab808-118">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="ab808-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab808-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab808-119">Request headers</span></span>

| <span data-ttu-id="ab808-120">Header</span><span class="sxs-lookup"><span data-stu-id="ab808-120">Header</span></span>       | <span data-ttu-id="ab808-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ab808-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab808-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab808-122">Authorization</span></span>  | <span data-ttu-id="ab808-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ab808-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab808-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab808-125">Request body</span></span>

<span data-ttu-id="ab808-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ab808-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab808-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab808-127">Response</span></span>

<span data-ttu-id="ab808-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [TeamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ab808-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab808-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab808-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab808-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab808-130">Request</span></span>

<span data-ttu-id="ab808-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab808-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET /teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="ab808-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab808-132">Response</span></span>

<span data-ttu-id="ab808-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ab808-133">The following is an example of the response.</span></span>
><span data-ttu-id="ab808-134">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ab808-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ab808-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ab808-135">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="ab808-136">Beispiel: Abrufen der Namen der installierten apps</span><span class="sxs-lookup"><span data-stu-id="ab808-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="ab808-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab808-137">Request</span></span>

<span data-ttu-id="ab808-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab808-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="ab808-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab808-139">Response</span></span>

<span data-ttu-id="ab808-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ab808-140">The following is an example of the response.</span></span>

><span data-ttu-id="ab808-141">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ab808-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ab808-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ab808-142">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
