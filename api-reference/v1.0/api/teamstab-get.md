---
title: Erste Registerkarte
description: 'Abrufen der Eigenschaften und Beziehungen zwischen der angegebenen Registerkarte. '
author: nkramer
ms.openlocfilehash: 30c98258585db9443e2481db5a9fb8c304b8d72b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339585"
---
# <a name="get-tab"></a><span data-ttu-id="9f453-103">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="9f453-103">Get tab</span></span>



<span data-ttu-id="9f453-104">Abrufen der Eigenschaften und Beziehungen zwischen der angegebenen [Registerkarte](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="9f453-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9f453-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f453-105">Permissions</span></span>
<span data-ttu-id="9f453-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f453-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f453-108">Permission type</span></span>      | <span data-ttu-id="9f453-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f453-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f453-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f453-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f453-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f453-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f453-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f453-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f453-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f453-113">Not supported.</span></span>    |
|<span data-ttu-id="9f453-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f453-114">Application</span></span> | <span data-ttu-id="9f453-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f453-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="9f453-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="9f453-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9f453-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="9f453-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f453-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f453-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f453-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9f453-119">Optional query parameters</span></span>

<span data-ttu-id="9f453-120">Diese Methode unterstützt die $select und $den [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="9f453-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f453-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f453-121">Request headers</span></span>
| <span data-ttu-id="9f453-122">Header</span><span class="sxs-lookup"><span data-stu-id="9f453-122">Header</span></span>       | <span data-ttu-id="9f453-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9f453-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f453-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f453-124">Authorization</span></span>  | <span data-ttu-id="9f453-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f453-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f453-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f453-127">Request body</span></span>
<span data-ttu-id="9f453-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f453-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f453-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f453-129">Response</span></span>

<span data-ttu-id="9f453-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Tab](../resources/teamstab.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f453-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f453-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f453-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9f453-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f453-132">Request</span></span>
<span data-ttu-id="9f453-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f453-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="9f453-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f453-134">Response</span></span>
<span data-ttu-id="9f453-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f453-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9f453-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9f453-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
