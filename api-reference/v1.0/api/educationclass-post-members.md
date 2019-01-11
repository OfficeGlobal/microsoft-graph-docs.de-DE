---
title: Kursteilnehmer hinzufügen
description: Hinzufügen eines Mitglieds zu einer Klasse.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f69d29a1726545c6c0a85af2200294cfc1d6fe00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804522"
---
# <a name="add-a-student"></a><span data-ttu-id="97581-103">Kursteilnehmer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="97581-103">Add a student</span></span>

<span data-ttu-id="97581-104">Hinzufügen eines Mitglieds zu einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="97581-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="97581-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97581-105">Permissions</span></span>
<span data-ttu-id="97581-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97581-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97581-108">Permission type</span></span>      | <span data-ttu-id="97581-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97581-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97581-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97581-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="97581-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97581-111">Not supported.</span></span>  |
|<span data-ttu-id="97581-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97581-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="97581-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97581-113">Not supported.</span></span>  |
|<span data-ttu-id="97581-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97581-114">Application</span></span> | <span data-ttu-id="97581-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="97581-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="97581-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97581-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="97581-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97581-117">Request headers</span></span>
| <span data-ttu-id="97581-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97581-118">Header</span></span>       | <span data-ttu-id="97581-119">Wert</span><span class="sxs-lookup"><span data-stu-id="97581-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97581-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="97581-120">Authorization</span></span>  | <span data-ttu-id="97581-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97581-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97581-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97581-123">Content-Type</span></span>  | <span data-ttu-id="97581-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97581-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97581-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97581-125">Request body</span></span>
<span data-ttu-id="97581-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="97581-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="97581-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="97581-127">Response</span></span>
<span data-ttu-id="97581-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97581-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97581-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97581-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97581-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97581-130">Request</span></span>
<span data-ttu-id="97581-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97581-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="97581-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="97581-132">Response</span></span>
<span data-ttu-id="97581-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97581-133">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
