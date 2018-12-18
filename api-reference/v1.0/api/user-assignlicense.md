---
title: assignLicense
description: Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.
author: dkershaw10
ms.openlocfilehash: 26c65c0597d5c066af1388087aef07e181076e7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326397"
---
# <a name="assignlicense"></a><span data-ttu-id="0e7c3-104">assignLicense</span><span class="sxs-lookup"><span data-stu-id="0e7c3-104">assignLicense</span></span>
<span data-ttu-id="0e7c3-p102">Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-p102">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e7c3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e7c3-107">Permissions</span></span>
<span data-ttu-id="0e7c3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e7c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e7c3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e7c3-110">Permission type</span></span>      | <span data-ttu-id="0e7c3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e7c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e7c3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e7c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e7c3-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e7c3-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e7c3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e7c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e7c3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e7c3-115">Not supported.</span></span>    |
|<span data-ttu-id="0e7c3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e7c3-116">Application</span></span> | <span data-ttu-id="0e7c3-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e7c3-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e7c3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e7c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="0e7c3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e7c3-119">Request headers</span></span>
| <span data-ttu-id="0e7c3-120">Header</span><span class="sxs-lookup"><span data-stu-id="0e7c3-120">Header</span></span>       | <span data-ttu-id="0e7c3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0e7c3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e7c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e7c3-122">Authorization</span></span>  | <span data-ttu-id="0e7c3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0e7c3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e7c3-125">Content-Type</span></span>  | <span data-ttu-id="0e7c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e7c3-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e7c3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e7c3-127">Request body</span></span>
<span data-ttu-id="0e7c3-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e7c3-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="0e7c3-129">Parameter</span></span>    | <span data-ttu-id="0e7c3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0e7c3-130">Type</span></span>   |<span data-ttu-id="0e7c3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e7c3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e7c3-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="0e7c3-132">addLicenses</span></span>|<span data-ttu-id="0e7c3-133">AssignedLicense-Auflistung</span><span class="sxs-lookup"><span data-stu-id="0e7c3-133">AssignedLicense collection</span></span>|<span data-ttu-id="0e7c3-p105">Eine Sammlung von [assignedLicense](../resources/assignedlicense.md)-Objekten, die die hinzuzufügenden Lizenzen angeben. Sie können Pläne deaktivieren, die einer Lizenz zugeordnet sind, indem Sie die **disabledPlans**-Eigenschaft für ein [assignedLicense](../resources/assignedlicense.md)-Objekt festlegen.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="0e7c3-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="0e7c3-136">removeLicenses</span></span>|<span data-ttu-id="0e7c3-137">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0e7c3-137">Guid collection</span></span>|<span data-ttu-id="0e7c3-138">Eine Auflistung von GUIDs, die die zu entfernenden Lizenzen identifizieren.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="0e7c3-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e7c3-139">Response</span></span>

<span data-ttu-id="0e7c3-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e7c3-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e7c3-141">Example</span></span>
<span data-ttu-id="0e7c3-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e7c3-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e7c3-143">Request</span></span>
<span data-ttu-id="0e7c3-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "guid"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="0e7c3-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e7c3-145">Response</span></span>
<span data-ttu-id="0e7c3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e7c3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "0118A350-71FC-4EC3-8F0C-6A1CB8867561"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-02T12:13:14Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
