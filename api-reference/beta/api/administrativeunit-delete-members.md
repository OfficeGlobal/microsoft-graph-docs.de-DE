---
title: Mitglied entfernen
description: Verwenden Sie diese API zum Entfernen eines Mitglieds (Benutzer oder Gruppe) über eine administrative Einheit.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 09cb727c60e102786948311f10df48f9230a9dd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865200"
---
# <a name="remove-a-member"></a><span data-ttu-id="76799-103">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="76799-103">Remove a member</span></span>

> <span data-ttu-id="76799-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="76799-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76799-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76799-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76799-106">Verwenden Sie diese API zum Entfernen eines Mitglieds (Benutzer oder Gruppe) über eine administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="76799-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="76799-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="76799-107">Permissions</span></span>
<span data-ttu-id="76799-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76799-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="76799-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76799-110">Permission type</span></span>      | <span data-ttu-id="76799-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76799-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76799-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76799-112">Delegated (work or school account)</span></span> | <span data-ttu-id="76799-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76799-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="76799-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76799-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76799-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76799-115">Not supported.</span></span>    |
|<span data-ttu-id="76799-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76799-116">Application</span></span> | <span data-ttu-id="76799-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76799-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76799-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76799-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="76799-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76799-119">Request headers</span></span>
| <span data-ttu-id="76799-120">Name</span><span class="sxs-lookup"><span data-stu-id="76799-120">Name</span></span>      |<span data-ttu-id="76799-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76799-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76799-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76799-122">Authorization</span></span>  | <span data-ttu-id="76799-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="76799-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76799-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76799-125">Request body</span></span>
<span data-ttu-id="76799-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="76799-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76799-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="76799-127">Response</span></span>

<span data-ttu-id="76799-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76799-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76799-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76799-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76799-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76799-131">Request</span></span>
<span data-ttu-id="76799-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76799-132">Here is an example of the request.</span></span> <span data-ttu-id="76799-133">Im folgenden Beispiel id1 stellt den Bezeichner für die administrative Einheit Ziel und id2 stellt den eindeutigen Bezeichner für die Member Benutzer oder eine Gruppe aus der gerichteter administrative Einheit entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="76799-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="76799-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="76799-134">Response</span></span>
<span data-ttu-id="76799-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="76799-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
