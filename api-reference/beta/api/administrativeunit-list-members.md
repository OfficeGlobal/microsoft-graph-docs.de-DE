---
title: Mitglieder auflisten
description: Verwenden Sie diese API zum Abrufen der Mitglieder Liste (Benutzer und Gruppen) in eine administrative Einheit.
author: lleonard-msft
ms.openlocfilehash: d373c8353928d8e8d5d8b398aa09e62d457ba665
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311662"
---
# <a name="list-members"></a><span data-ttu-id="a29d5-103">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="a29d5-103">List members</span></span>

> <span data-ttu-id="a29d5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a29d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a29d5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a29d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a29d5-106">Verwenden Sie diese API zum Abrufen der Mitglieder Liste (Benutzer und Gruppen) in eine administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="a29d5-106">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="a29d5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a29d5-107">Permissions</span></span>
<span data-ttu-id="a29d5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a29d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a29d5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a29d5-110">Permission type</span></span>      | <span data-ttu-id="a29d5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a29d5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a29d5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a29d5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a29d5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a29d5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a29d5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a29d5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a29d5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a29d5-115">Not supported.</span></span>    |
|<span data-ttu-id="a29d5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a29d5-116">Application</span></span> | <span data-ttu-id="a29d5-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a29d5-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a29d5-118">Hinweis: Zum Auflisten der Mitglieder einer ausgeblendeten Mitgliedschaften in eine administrative Einheit ist die Berechtigung Member.Read.Hidden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a29d5-118">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="a29d5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a29d5-119">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a29d5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a29d5-120">Request headers</span></span>
| <span data-ttu-id="a29d5-121">Name</span><span class="sxs-lookup"><span data-stu-id="a29d5-121">Name</span></span>      |<span data-ttu-id="a29d5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a29d5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a29d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a29d5-123">Authorization</span></span>  | <span data-ttu-id="a29d5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a29d5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a29d5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a29d5-126">Request body</span></span>
<span data-ttu-id="a29d5-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a29d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a29d5-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a29d5-128">Response</span></span>

<span data-ttu-id="a29d5-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von [Benutzer](../resources/user.md) und/oder [Gruppe](../resources/group.md) von Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a29d5-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="a29d5-130">Stattdessen, wenn Sie ablegen `$ref` am Ende der Anforderung, die Antwort enthält eine Auflistung von `@odata.id` Links/URLs an die Mitglieder.</span><span class="sxs-lookup"><span data-stu-id="a29d5-130">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="a29d5-131">Beispiele</span><span class="sxs-lookup"><span data-stu-id="a29d5-131">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="a29d5-132">Liste diemember-Objekte</span><span class="sxs-lookup"><span data-stu-id="a29d5-132">List member objects</span></span>
<span data-ttu-id="a29d5-133">Die folgende Anforderung Listet die Mitglieder der administrativen Einheit, eine Auflistung von Benutzern und/oder Gruppen zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="a29d5-133">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="a29d5-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a29d5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a><span data-ttu-id="a29d5-137">Elementverweise Liste</span><span class="sxs-lookup"><span data-stu-id="a29d5-137">List member references</span></span>
<span data-ttu-id="a29d5-138">Die folgende Anforderung wird Auflisten der Memberverweise die administrative Einheit, eine Auflistung von zurückgeben `@odata.id` Verweise auf die Elemente.</span><span class="sxs-lookup"><span data-stu-id="a29d5-138">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="a29d5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a29d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
