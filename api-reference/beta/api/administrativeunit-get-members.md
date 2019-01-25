---
title: Abrufen eines Elements
description: Verwenden Sie diese API, um ein bestimmtes Element (Benutzer oder Gruppe) in eine administrative Einheit abzurufen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67067d0e465aab61449a42cd833f9e6ce07fcd12
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526795"
---
# <a name="get-a-member"></a><span data-ttu-id="8edf2-103">Abrufen eines Elements</span><span class="sxs-lookup"><span data-stu-id="8edf2-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8edf2-104">Verwenden Sie diese API, um ein bestimmtes Element (Benutzer oder Gruppe) in eine administrative Einheit abzurufen.</span><span class="sxs-lookup"><span data-stu-id="8edf2-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="8edf2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8edf2-105">Permissions</span></span>
<span data-ttu-id="8edf2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8edf2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8edf2-108">Permission type</span></span>      | <span data-ttu-id="8edf2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8edf2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8edf2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8edf2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8edf2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8edf2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8edf2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8edf2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8edf2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8edf2-113">Not supported.</span></span>    |
|<span data-ttu-id="8edf2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8edf2-114">Application</span></span> | <span data-ttu-id="8edf2-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8edf2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8edf2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8edf2-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8edf2-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8edf2-117">Request headers</span></span>
| <span data-ttu-id="8edf2-118">Name</span><span class="sxs-lookup"><span data-stu-id="8edf2-118">Name</span></span>      |<span data-ttu-id="8edf2-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8edf2-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8edf2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8edf2-120">Authorization</span></span>  | <span data-ttu-id="8edf2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8edf2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8edf2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8edf2-123">Request body</span></span>
<span data-ttu-id="8edf2-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8edf2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8edf2-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8edf2-125">Response</span></span>

<span data-ttu-id="8edf2-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und einen [Benutzer](../resources/user.md) oder eine [Gruppe](../resources/group.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8edf2-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8edf2-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8edf2-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8edf2-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8edf2-128">Request</span></span>
<span data-ttu-id="8edf2-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8edf2-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="8edf2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8edf2-130">Response</span></span>
<span data-ttu-id="8edf2-131">Hier ist ein Beispiel für die Respone.</span><span class="sxs-lookup"><span data-stu-id="8edf2-131">Here is an example of the respone.</span></span> <span data-ttu-id="8edf2-132">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="8edf2-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8edf2-133">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8edf2-133">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
