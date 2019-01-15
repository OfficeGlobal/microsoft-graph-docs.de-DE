---
title: Registerkarte von Kanal löschen
description: 'Entfernt (löst) einer Registerkarte aus der angegebenen Kanal innerhalb eines Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9b66bf69645c9a76ea11375984cf8c56e0dff6bd
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016695"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="c8df8-103">Registerkarte von Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="c8df8-103">Delete tab from channel</span></span>



<span data-ttu-id="c8df8-104">Entfernt (löst) einer Registerkarte aus den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c8df8-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c8df8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8df8-105">Permissions</span></span>
<span data-ttu-id="c8df8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8df8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8df8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8df8-108">Permission type</span></span>      | <span data-ttu-id="c8df8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8df8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8df8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8df8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8df8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8df8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c8df8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8df8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8df8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8df8-113">Not supported.</span></span>    |
|<span data-ttu-id="c8df8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8df8-114">Application</span></span> | <span data-ttu-id="c8df8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8df8-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="c8df8-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="c8df8-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c8df8-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="c8df8-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c8df8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8df8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c8df8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8df8-119">Request headers</span></span>
| <span data-ttu-id="c8df8-120">Header</span><span class="sxs-lookup"><span data-stu-id="c8df8-120">Header</span></span>       | <span data-ttu-id="c8df8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c8df8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8df8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8df8-122">Authorization</span></span>  | <span data-ttu-id="c8df8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8df8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8df8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8df8-125">Request body</span></span>
<span data-ttu-id="c8df8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8df8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8df8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8df8-127">Response</span></span>

<span data-ttu-id="c8df8-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8df8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8df8-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8df8-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c8df8-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8df8-131">Request</span></span>
<span data-ttu-id="c8df8-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8df8-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="c8df8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8df8-133">Response</span></span>
<span data-ttu-id="c8df8-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8df8-134">The following is an example of the response.</span></span> <span data-ttu-id="c8df8-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="c8df8-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c8df8-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8df8-136">All of the properties will be returned from an actual call.</span></span>
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
