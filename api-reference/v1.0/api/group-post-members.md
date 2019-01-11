---
title: Mitglied hinzufügen
description: Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.
localization_priority: Priority
ms.openlocfilehash: 89f4bd5060e167e1920e5f64d70127c1fed41ad6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867522"
---
# <a name="add-member"></a><span data-ttu-id="9c7e6-103">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="9c7e6-103">Add member</span></span>
<span data-ttu-id="9c7e6-104">Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="9c7e6-105">Sie können Benutzer oder andere Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-105">You can add users or other groups.</span></span> <span data-ttu-id="9c7e6-106">Wichtig: Sie können nur Benutzer zu Office 365-Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c7e6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c7e6-107">Permissions</span></span>
<span data-ttu-id="9c7e6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c7e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c7e6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c7e6-110">Permission type</span></span>      | <span data-ttu-id="9c7e6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c7e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c7e6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c7e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c7e6-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c7e6-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c7e6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c7e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c7e6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c7e6-115">Not supported.</span></span>    |
|<span data-ttu-id="9c7e6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c7e6-116">Application</span></span> | <span data-ttu-id="9c7e6-117">Group.ReadWrite.All und Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c7e6-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c7e6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c7e6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9c7e6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c7e6-119">Request headers</span></span>
| <span data-ttu-id="9c7e6-120">Name</span><span class="sxs-lookup"><span data-stu-id="9c7e6-120">Name</span></span>       | <span data-ttu-id="9c7e6-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9c7e6-121">Type</span></span> | <span data-ttu-id="9c7e6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c7e6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c7e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c7e6-123">Authorization</span></span>  | <span data-ttu-id="9c7e6-124">string</span><span class="sxs-lookup"><span data-stu-id="9c7e6-124">string</span></span>  | <span data-ttu-id="9c7e6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c7e6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c7e6-127">Request body</span></span>
<span data-ttu-id="9c7e6-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9c7e6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c7e6-129">Response</span></span>
<span data-ttu-id="9c7e6-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c7e6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c7e6-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9c7e6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c7e6-133">Request</span></span>
<span data-ttu-id="9c7e6-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="9c7e6-135">Geben Sie im Anforderungstext eine JSON-Darstellung des `id` des [directoryObject](../resources/directoryobject.md)-, [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="9c7e6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c7e6-136">Response</span></span>
<span data-ttu-id="9c7e6-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-137">The following is an example of the response.</span></span>
><span data-ttu-id="9c7e6-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9c7e6-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9c7e6-139">All the properties will be returned from an actual call.</span></span>
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
