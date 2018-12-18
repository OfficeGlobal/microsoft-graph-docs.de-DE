---
title: Ein Mitglied hinzufügen
description: Verwenden Sie diese API zum Hinzufügen eines Mitglieds (Benutzer oder Gruppe), um eine administrative Einheit.
author: lleonard-msft
ms.openlocfilehash: be47dbf06c5f59c0a4aaaea4f8c8b4aa8c3ce902
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339228"
---
# <a name="add-a-member"></a><span data-ttu-id="e5b91-103">Ein Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e5b91-103">Add a member</span></span>

> <span data-ttu-id="e5b91-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5b91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5b91-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5b91-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5b91-106">Verwenden Sie diese API zum Hinzufügen eines Mitglieds (Benutzer oder Gruppe), um eine administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="e5b91-106">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="e5b91-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e5b91-107">Permissions</span></span>
<span data-ttu-id="e5b91-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5b91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e5b91-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5b91-110">Permission type</span></span>      | <span data-ttu-id="e5b91-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5b91-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5b91-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5b91-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5b91-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5b91-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5b91-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5b91-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b91-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5b91-115">Not supported.</span></span>    |
|<span data-ttu-id="e5b91-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5b91-116">Application</span></span> | <span data-ttu-id="e5b91-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5b91-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5b91-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5b91-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e5b91-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5b91-119">Request headers</span></span>
| <span data-ttu-id="e5b91-120">Name</span><span class="sxs-lookup"><span data-stu-id="e5b91-120">Name</span></span>      |<span data-ttu-id="e5b91-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5b91-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5b91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b91-122">Authorization</span></span>  | <span data-ttu-id="e5b91-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e5b91-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5b91-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5b91-125">Request body</span></span>
<span data-ttu-id="e5b91-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [Benutzers](../resources/user.md), [Gruppe](../resources/group.md) oder [DirectoryObject](../resources/directoryobject.md) hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="e5b91-126">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e5b91-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5b91-127">Response</span></span>

<span data-ttu-id="e5b91-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5b91-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b91-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5b91-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5b91-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5b91-131">Request</span></span>
<span data-ttu-id="e5b91-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5b91-132">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="e5b91-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der die `id` des Objekts [Benutzer](../resources/user.md) oder eine [Gruppe](../resources/group.md) hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="e5b91-133">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="e5b91-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5b91-134">Response</span></span>
<span data-ttu-id="e5b91-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e5b91-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
