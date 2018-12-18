---
title: Abrufen eines Elements
description: Verwenden Sie diese API, um ein bestimmtes Element (Benutzer oder Gruppe) in eine administrative Einheit abzurufen.
author: lleonard-msft
ms.openlocfilehash: 9e0e8bedc349511c59e304cacfc713d54a0f8335
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328392"
---
# <a name="get-a-member"></a><span data-ttu-id="dd49c-103">Abrufen eines Elements</span><span class="sxs-lookup"><span data-stu-id="dd49c-103">Get a member</span></span>

> <span data-ttu-id="dd49c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd49c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd49c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd49c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd49c-106">Verwenden Sie diese API, um ein bestimmtes Element (Benutzer oder Gruppe) in eine administrative Einheit abzurufen.</span><span class="sxs-lookup"><span data-stu-id="dd49c-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd49c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd49c-107">Permissions</span></span>
<span data-ttu-id="dd49c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd49c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd49c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd49c-110">Permission type</span></span>      | <span data-ttu-id="dd49c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd49c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd49c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd49c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd49c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd49c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd49c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd49c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd49c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd49c-115">Not supported.</span></span>    |
|<span data-ttu-id="dd49c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd49c-116">Application</span></span> | <span data-ttu-id="dd49c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd49c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd49c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd49c-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd49c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd49c-119">Request headers</span></span>
| <span data-ttu-id="dd49c-120">Name</span><span class="sxs-lookup"><span data-stu-id="dd49c-120">Name</span></span>      |<span data-ttu-id="dd49c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd49c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd49c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd49c-122">Authorization</span></span>  | <span data-ttu-id="dd49c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd49c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd49c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd49c-125">Request body</span></span>
<span data-ttu-id="dd49c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd49c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd49c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd49c-127">Response</span></span>

<span data-ttu-id="dd49c-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und einen [Benutzer](../resources/user.md) oder eine [Gruppe](../resources/group.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dd49c-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd49c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd49c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd49c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd49c-130">Request</span></span>
<span data-ttu-id="dd49c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd49c-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="dd49c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd49c-132">Response</span></span>
<span data-ttu-id="dd49c-133">Hier ist ein Beispiel für die Respone.</span><span class="sxs-lookup"><span data-stu-id="dd49c-133">Here is an example of the respone.</span></span> <span data-ttu-id="dd49c-134">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="dd49c-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dd49c-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd49c-135">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```