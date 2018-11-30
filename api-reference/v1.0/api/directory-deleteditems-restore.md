---
title: Gelöschtes Element wiederherstellen
description: 'Stellt ein kürzlich gelöschtes Element aus den gelöschten Elementen wieder her. '
ms.openlocfilehash: 3fa47d269cefaf54994b57f8f06a92a8ac8fc4b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018400"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="3eb6c-103">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="3eb6c-103">Restore deleted item</span></span>

<span data-ttu-id="3eb6c-104">Stellt ein kürzlich gelöschtes Element aus den [gelöschten Elementen](../resources/directory.md) wieder her.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="3eb6c-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="3eb6c-106">Wenn ein Element versehentlich gelöscht wurde, können es vollständig wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="3eb6c-107">Ein kürzlich gelöschtes Element bleibt bis zu 30 Tage verfügbar.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="3eb6c-108">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eb6c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3eb6c-109">Permissions</span></span>
<span data-ttu-id="3eb6c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="3eb6c-112">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="3eb6c-112">For users:</span></span>

|<span data-ttu-id="3eb6c-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3eb6c-113">Permission type</span></span>      | <span data-ttu-id="3eb6c-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3eb6c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eb6c-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3eb6c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3eb6c-116">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3eb6c-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3eb6c-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3eb6c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eb6c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eb6c-118">Not supported.</span></span> |
|<span data-ttu-id="3eb6c-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3eb6c-119">Application</span></span> | <span data-ttu-id="3eb6c-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb6c-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="3eb6c-121">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="3eb6c-121">For groups:</span></span>

|<span data-ttu-id="3eb6c-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3eb6c-122">Permission type</span></span>      | <span data-ttu-id="3eb6c-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3eb6c-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eb6c-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3eb6c-124">Delegated (work or school account)</span></span> | <span data-ttu-id="3eb6c-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3eb6c-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3eb6c-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3eb6c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eb6c-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eb6c-127">Not supported.</span></span>    |
|<span data-ttu-id="3eb6c-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3eb6c-128">Application</span></span> | <span data-ttu-id="3eb6c-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb6c-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eb6c-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eb6c-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="3eb6c-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3eb6c-131">Request headers</span></span>
| <span data-ttu-id="3eb6c-132">Name</span><span class="sxs-lookup"><span data-stu-id="3eb6c-132">Name</span></span>       | <span data-ttu-id="3eb6c-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3eb6c-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3eb6c-134">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3eb6c-134">Authorization</span></span>  | <span data-ttu-id="3eb6c-135">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="3eb6c-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="3eb6c-136">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3eb6c-136">Accept</span></span> | <span data-ttu-id="3eb6c-137">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb6c-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eb6c-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3eb6c-138">Request body</span></span>
<span data-ttu-id="3eb6c-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eb6c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eb6c-140">Response</span></span>

<span data-ttu-id="3eb6c-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb6c-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3eb6c-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3eb6c-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eb6c-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="3eb6c-144">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3eb6c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eb6c-145">Response</span></span>
<span data-ttu-id="3eb6c-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3eb6c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->