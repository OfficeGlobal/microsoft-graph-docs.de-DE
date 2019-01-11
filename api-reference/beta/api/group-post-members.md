---
title: Mitglied hinzufügen
description: Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.
localization_priority: Normal
ms.openlocfilehash: 74ad07ea9012385f896ba4c6c6aa18f44758e5bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832865"
---
# <a name="add-member"></a><span data-ttu-id="07d39-103">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="07d39-103">Add member</span></span>

> <span data-ttu-id="07d39-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07d39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07d39-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07d39-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07d39-106">Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="07d39-106">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="07d39-107">Sie können Benutzer oder andere Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="07d39-107">You can add users or other groups.</span></span> <span data-ttu-id="07d39-108">Wichtig: Sie können nur Benutzer zu Office 365-Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="07d39-108">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="07d39-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07d39-109">Permissions</span></span>
<span data-ttu-id="07d39-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d39-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d39-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07d39-112">Permission type</span></span>      | <span data-ttu-id="07d39-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07d39-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d39-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07d39-114">Delegated (work or school account)</span></span> | <span data-ttu-id="07d39-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07d39-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07d39-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07d39-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d39-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07d39-117">Not supported.</span></span>    |
|<span data-ttu-id="07d39-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07d39-118">Application</span></span> | <span data-ttu-id="07d39-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d39-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07d39-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07d39-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="07d39-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07d39-121">Request headers</span></span>
| <span data-ttu-id="07d39-122">Name</span><span class="sxs-lookup"><span data-stu-id="07d39-122">Name</span></span>       | <span data-ttu-id="07d39-123">Typ</span><span class="sxs-lookup"><span data-stu-id="07d39-123">Type</span></span> | <span data-ttu-id="07d39-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07d39-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07d39-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d39-125">Authorization</span></span>  | <span data-ttu-id="07d39-126">string</span><span class="sxs-lookup"><span data-stu-id="07d39-126">string</span></span>  | <span data-ttu-id="07d39-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07d39-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07d39-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07d39-129">Request body</span></span>
<span data-ttu-id="07d39-130">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="07d39-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="07d39-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="07d39-131">Response</span></span>
<span data-ttu-id="07d39-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07d39-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d39-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07d39-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="07d39-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07d39-135">Request</span></span>
<span data-ttu-id="07d39-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07d39-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="07d39-137">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der die `id` des Objekts [DirectoryObject](../resources/directoryobject.md), [Benutzer](../resources/user.md)oder [Gruppe](../resources/group.md) hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="07d39-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="07d39-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="07d39-138">Response</span></span>
<span data-ttu-id="07d39-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07d39-139">The following is an example of the response.</span></span>
><span data-ttu-id="07d39-140">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="07d39-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07d39-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="07d39-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
