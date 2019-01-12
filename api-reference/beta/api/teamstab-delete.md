---
title: Registerkarte von Kanal löschen
description: 'Entfernt (löst) einer Registerkarte aus der angegebenen Kanal innerhalb eines Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2103d63e6919e40b868071a44fb3f0a99e95049b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945174"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="dc59b-103">Registerkarte von Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="dc59b-103">Delete tab from channel</span></span>

> <span data-ttu-id="dc59b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dc59b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc59b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dc59b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc59b-106">Entfernt (löst) einer Registerkarte aus den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="dc59b-106">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="dc59b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dc59b-107">Permissions</span></span>
<span data-ttu-id="dc59b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc59b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc59b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc59b-110">Permission type</span></span>      | <span data-ttu-id="dc59b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc59b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc59b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc59b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc59b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc59b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc59b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc59b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc59b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc59b-115">Not supported.</span></span>    |
|<span data-ttu-id="dc59b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc59b-116">Application</span></span> | <span data-ttu-id="dc59b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc59b-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="dc59b-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="dc59b-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dc59b-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="dc59b-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dc59b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc59b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc59b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc59b-121">Request headers</span></span>
| <span data-ttu-id="dc59b-122">Header</span><span class="sxs-lookup"><span data-stu-id="dc59b-122">Header</span></span>       | <span data-ttu-id="dc59b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="dc59b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc59b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc59b-124">Authorization</span></span>  | <span data-ttu-id="dc59b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc59b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc59b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc59b-127">Request body</span></span>
<span data-ttu-id="dc59b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dc59b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc59b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc59b-129">Response</span></span>

<span data-ttu-id="dc59b-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc59b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc59b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc59b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dc59b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc59b-133">Request</span></span>
<span data-ttu-id="dc59b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc59b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="dc59b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc59b-135">Response</span></span>
<span data-ttu-id="dc59b-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dc59b-136">The following is an example of the response.</span></span> <span data-ttu-id="dc59b-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="dc59b-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dc59b-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc59b-138">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
