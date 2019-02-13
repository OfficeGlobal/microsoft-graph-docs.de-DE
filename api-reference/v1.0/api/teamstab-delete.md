---
title: Registerkarte von Kanal löschen
description: 'Entfernt (löst) einer Registerkarte aus der angegebenen Kanal innerhalb eines Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a5cb2334c250c63d0644c8fab3f97d35c481a515
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967305"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="c496c-103">Registerkarte von Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="c496c-103">Delete tab from channel</span></span>



<span data-ttu-id="c496c-104">Entfernt (löst) einer Registerkarte aus den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c496c-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c496c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c496c-105">Permissions</span></span>
<span data-ttu-id="c496c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c496c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c496c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c496c-108">Permission type</span></span>      | <span data-ttu-id="c496c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c496c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c496c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c496c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c496c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c496c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c496c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c496c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c496c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c496c-113">Not supported.</span></span>    |
|<span data-ttu-id="c496c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c496c-114">Application</span></span> | <span data-ttu-id="c496c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c496c-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="c496c-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="c496c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c496c-117">Globale Administratoren und Microsoft Teams-Dienstadministratoren können auf Teams zugreifen, in denen sie kein Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="c496c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c496c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c496c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c496c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c496c-119">Request headers</span></span>
| <span data-ttu-id="c496c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c496c-120">Header</span></span>       | <span data-ttu-id="c496c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c496c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c496c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c496c-122">Authorization</span></span>  | <span data-ttu-id="c496c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c496c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c496c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c496c-125">Request body</span></span>
<span data-ttu-id="c496c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c496c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c496c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c496c-127">Response</span></span>

<span data-ttu-id="c496c-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c496c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c496c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c496c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c496c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c496c-131">Request</span></span>
<span data-ttu-id="c496c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c496c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="c496c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c496c-133">Response</span></span>
<span data-ttu-id="c496c-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c496c-134">The following is an example of the response.</span></span> <span data-ttu-id="c496c-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="c496c-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c496c-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c496c-136">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
