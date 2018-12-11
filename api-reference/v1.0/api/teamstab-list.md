---
title: Liste der Registerkarten im Kanal
description: 'Rufen Sie die Liste der Registerkarten in den angegebenen Kanal innerhalb eines Teams ab. '
ms.openlocfilehash: 4efbe8508fc125d87268adfb05c23b99ab2c3d4b
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222373"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="8fac6-103">Liste der Registerkarten im Kanal</span><span class="sxs-lookup"><span data-stu-id="8fac6-103">List tabs in channel</span></span>



<span data-ttu-id="8fac6-104">Rufen Sie die Liste der [Registerkarten](../resources/teamstab.md) in den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md)ab.</span><span class="sxs-lookup"><span data-stu-id="8fac6-104">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8fac6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8fac6-105">Permissions</span></span>
<span data-ttu-id="8fac6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fac6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fac6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fac6-108">Permission type</span></span>      | <span data-ttu-id="8fac6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fac6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fac6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fac6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fac6-111">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fac6-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="8fac6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fac6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fac6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fac6-113">Not supported.</span></span>    |
| <span data-ttu-id="8fac6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fac6-114">Application</span></span>                            | <span data-ttu-id="8fac6-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fac6-115">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="8fac6-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8fac6-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8fac6-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="8fac6-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8fac6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fac6-118">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fac6-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8fac6-119">Optional query parameters</span></span>

<span data-ttu-id="8fac6-120">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="8fac6-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fac6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fac6-121">Request headers</span></span>
| <span data-ttu-id="8fac6-122">Header</span><span class="sxs-lookup"><span data-stu-id="8fac6-122">Header</span></span>       | <span data-ttu-id="8fac6-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8fac6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fac6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fac6-124">Authorization</span></span>  | <span data-ttu-id="8fac6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fac6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fac6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fac6-127">Request body</span></span>
<span data-ttu-id="8fac6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8fac6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fac6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fac6-129">Response</span></span>
<span data-ttu-id="8fac6-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Registerkarten](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="8fac6-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fac6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fac6-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8fac6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fac6-132">Request</span></span>
<span data-ttu-id="8fac6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fac6-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="8fac6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fac6-134">Response</span></span>
<span data-ttu-id="8fac6-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8fac6-135">The following is an example of the response.</span></span>
><span data-ttu-id="8fac6-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8fac6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
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
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
