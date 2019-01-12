---
title: Mitglied entfernen
description: Verwenden Sie diese API zum Entfernen eines Mitglieds (Benutzer oder Gruppe) über eine administrative Einheit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e79dac5b7ae3a20675f6faaf9b209f8117ca2252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941527"
---
# <a name="remove-a-member"></a><span data-ttu-id="5922d-103">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="5922d-103">Remove a member</span></span>

> <span data-ttu-id="5922d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5922d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5922d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5922d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5922d-106">Verwenden Sie diese API zum Entfernen eines Mitglieds (Benutzer oder Gruppe) über eine administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="5922d-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="5922d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5922d-107">Permissions</span></span>
<span data-ttu-id="5922d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5922d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5922d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5922d-110">Permission type</span></span>      | <span data-ttu-id="5922d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5922d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5922d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5922d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5922d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5922d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5922d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5922d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5922d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5922d-115">Not supported.</span></span>    |
|<span data-ttu-id="5922d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5922d-116">Application</span></span> | <span data-ttu-id="5922d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5922d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5922d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5922d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5922d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5922d-119">Request headers</span></span>
| <span data-ttu-id="5922d-120">Name</span><span class="sxs-lookup"><span data-stu-id="5922d-120">Name</span></span>      |<span data-ttu-id="5922d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5922d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5922d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5922d-122">Authorization</span></span>  | <span data-ttu-id="5922d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5922d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5922d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5922d-125">Request body</span></span>
<span data-ttu-id="5922d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5922d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5922d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5922d-127">Response</span></span>

<span data-ttu-id="5922d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5922d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5922d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5922d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5922d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5922d-131">Request</span></span>
<span data-ttu-id="5922d-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5922d-132">Here is an example of the request.</span></span> <span data-ttu-id="5922d-133">Im folgenden Beispiel id1 stellt den Bezeichner für die administrative Einheit Ziel und id2 stellt den eindeutigen Bezeichner für die Member Benutzer oder eine Gruppe aus der gerichteter administrative Einheit entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="5922d-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="5922d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5922d-134">Response</span></span>
<span data-ttu-id="5922d-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5922d-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
