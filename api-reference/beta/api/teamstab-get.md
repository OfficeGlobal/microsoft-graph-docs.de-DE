---
title: Erste Registerkarte
description: 'Abrufen der Eigenschaften und Beziehungen zwischen der angegebenen Registerkarte. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: f08853cb1969427bfbabac8bd5e6e446b1142ffe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864946"
---
# <a name="get-tab"></a><span data-ttu-id="83199-103">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="83199-103">Get tab</span></span>

> <span data-ttu-id="83199-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83199-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83199-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83199-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83199-106">Abrufen der Eigenschaften und Beziehungen zwischen der angegebenen [Registerkarte](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="83199-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="83199-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="83199-107">Permissions</span></span>
<span data-ttu-id="83199-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83199-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83199-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83199-110">Permission type</span></span>      | <span data-ttu-id="83199-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83199-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83199-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83199-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83199-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83199-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83199-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83199-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83199-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83199-115">Not supported.</span></span>    |
|<span data-ttu-id="83199-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83199-116">Application</span></span> | <span data-ttu-id="83199-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83199-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="83199-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="83199-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="83199-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="83199-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="83199-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83199-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83199-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="83199-121">Optional query parameters</span></span>

<span data-ttu-id="83199-122">Diese Methode unterstützt die $select und $den [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="83199-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83199-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83199-123">Request headers</span></span>
| <span data-ttu-id="83199-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83199-124">Header</span></span>       | <span data-ttu-id="83199-125">Wert</span><span class="sxs-lookup"><span data-stu-id="83199-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83199-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="83199-126">Authorization</span></span>  | <span data-ttu-id="83199-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="83199-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83199-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83199-129">Request body</span></span>
<span data-ttu-id="83199-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="83199-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83199-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="83199-131">Response</span></span>

<span data-ttu-id="83199-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Tab](../resources/teamstab.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="83199-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83199-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83199-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="83199-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83199-134">Request</span></span>
<span data-ttu-id="83199-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83199-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="83199-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="83199-136">Response</span></span>
<span data-ttu-id="83199-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="83199-137">The following is an example of the response.</span></span> 

><span data-ttu-id="83199-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="83199-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
