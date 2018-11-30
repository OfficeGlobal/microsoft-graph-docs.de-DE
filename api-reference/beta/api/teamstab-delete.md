---
title: Registerkarte von Kanal löschen
description: 'Entfernt (löst) einer Registerkarte aus der angegebenen Kanal innerhalb eines Teams. '
ms.openlocfilehash: 975f046b3da279ddcda2f3f13be89ee7c45b21a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065023"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="54eaa-103">Registerkarte von Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="54eaa-103">Delete tab from channel</span></span>

> <span data-ttu-id="54eaa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54eaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54eaa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54eaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54eaa-106">Entfernt (löst) einer Registerkarte aus den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="54eaa-106">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="54eaa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="54eaa-107">Permissions</span></span>
<span data-ttu-id="54eaa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54eaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54eaa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54eaa-110">Permission type</span></span>      | <span data-ttu-id="54eaa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54eaa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54eaa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54eaa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54eaa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54eaa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="54eaa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54eaa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54eaa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54eaa-115">Not supported.</span></span>    |
|<span data-ttu-id="54eaa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54eaa-116">Application</span></span> | <span data-ttu-id="54eaa-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54eaa-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54eaa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54eaa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="54eaa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54eaa-119">Request headers</span></span>
| <span data-ttu-id="54eaa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="54eaa-120">Header</span></span>       | <span data-ttu-id="54eaa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="54eaa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54eaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54eaa-122">Authorization</span></span>  | <span data-ttu-id="54eaa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="54eaa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54eaa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54eaa-125">Request body</span></span>
<span data-ttu-id="54eaa-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="54eaa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54eaa-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="54eaa-127">Response</span></span>

<span data-ttu-id="54eaa-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54eaa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54eaa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54eaa-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="54eaa-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54eaa-131">Request</span></span>
<span data-ttu-id="54eaa-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54eaa-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="54eaa-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="54eaa-133">Response</span></span>
<span data-ttu-id="54eaa-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="54eaa-134">The following is an example of the response.</span></span> <span data-ttu-id="54eaa-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="54eaa-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="54eaa-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54eaa-136">All of the properties will be returned from an actual call.</span></span>
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
