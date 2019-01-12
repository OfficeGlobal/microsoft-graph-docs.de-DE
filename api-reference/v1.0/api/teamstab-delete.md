---
title: Registerkarte von Kanal löschen
description: 'Entfernt (löst) einer Registerkarte aus der angegebenen Kanal innerhalb eines Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 672077e4b1ac383ca6e6bb415ff25639fb03dc08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917433"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="2b374-103">Registerkarte von Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="2b374-103">Delete tab from channel</span></span>



<span data-ttu-id="2b374-104">Entfernt (löst) einer Registerkarte aus den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2b374-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2b374-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b374-105">Permissions</span></span>
<span data-ttu-id="2b374-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b374-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b374-108">Permission type</span></span>      | <span data-ttu-id="2b374-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b374-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b374-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b374-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b374-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b374-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b374-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b374-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b374-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b374-113">Not supported.</span></span>    |
|<span data-ttu-id="2b374-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b374-114">Application</span></span> | <span data-ttu-id="2b374-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b374-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="2b374-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="2b374-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2b374-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="2b374-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b374-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b374-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b374-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b374-119">Request headers</span></span>
| <span data-ttu-id="2b374-120">Header</span><span class="sxs-lookup"><span data-stu-id="2b374-120">Header</span></span>       | <span data-ttu-id="2b374-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2b374-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b374-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b374-122">Authorization</span></span>  | <span data-ttu-id="2b374-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b374-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b374-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b374-125">Request body</span></span>
<span data-ttu-id="2b374-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2b374-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b374-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b374-127">Response</span></span>

<span data-ttu-id="2b374-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b374-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b374-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b374-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2b374-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b374-131">Request</span></span>
<span data-ttu-id="2b374-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b374-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="2b374-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b374-133">Response</span></span>
<span data-ttu-id="2b374-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b374-134">The following is an example of the response.</span></span> <span data-ttu-id="2b374-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="2b374-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2b374-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b374-136">All of the properties will be returned from an actual call.</span></span>
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
