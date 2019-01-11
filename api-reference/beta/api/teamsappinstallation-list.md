---
title: Liste apps im team
description: Abrufen der Liste apps im angegebenen Team installiert.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 9b1589a7497ef466f996edde4353198d0d59b535
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854404"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="7db2c-103">Liste apps im team</span><span class="sxs-lookup"><span data-stu-id="7db2c-103">List apps in team</span></span>

> <span data-ttu-id="7db2c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7db2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7db2c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7db2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7db2c-106">Abrufen der Liste der in das angegebene [Team](../resources/team.md) [apps installiert](../resources/teamsappinstallation.md) .</span><span class="sxs-lookup"><span data-stu-id="7db2c-106">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7db2c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7db2c-107">Permissions</span></span>

<span data-ttu-id="7db2c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7db2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7db2c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7db2c-110">Permission type</span></span>      | <span data-ttu-id="7db2c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7db2c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7db2c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7db2c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7db2c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7db2c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7db2c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7db2c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7db2c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7db2c-115">Not supported.</span></span>    |
|<span data-ttu-id="7db2c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7db2c-116">Application</span></span> | <span data-ttu-id="7db2c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7db2c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7db2c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7db2c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7db2c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7db2c-119">Optional query parameters</span></span>

<span data-ttu-id="7db2c-120">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="7db2c-120">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7db2c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7db2c-121">Request headers</span></span>

| <span data-ttu-id="7db2c-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7db2c-122">Header</span></span>       | <span data-ttu-id="7db2c-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7db2c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7db2c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7db2c-124">Authorization</span></span>  | <span data-ttu-id="7db2c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7db2c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7db2c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7db2c-127">Request body</span></span>

<span data-ttu-id="7db2c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7db2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7db2c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7db2c-129">Response</span></span>

<span data-ttu-id="7db2c-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [TeamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7db2c-130">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7db2c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7db2c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7db2c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7db2c-132">Request</span></span>

<span data-ttu-id="7db2c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7db2c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="7db2c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7db2c-134">Response</span></span>

<span data-ttu-id="7db2c-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7db2c-135">The following is an example of the response.</span></span>
><span data-ttu-id="7db2c-136">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7db2c-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7db2c-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7db2c-137">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="7db2c-138">Beispiel: Abrufen der Namen der installierten apps</span><span class="sxs-lookup"><span data-stu-id="7db2c-138">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="7db2c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7db2c-139">Request</span></span>

<span data-ttu-id="7db2c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7db2c-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="7db2c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7db2c-141">Response</span></span>

<span data-ttu-id="7db2c-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7db2c-142">The following is an example of the response.</span></span>

><span data-ttu-id="7db2c-143">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7db2c-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7db2c-144">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7db2c-144">All the properties will be returned from an actual call.</span></span>
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
