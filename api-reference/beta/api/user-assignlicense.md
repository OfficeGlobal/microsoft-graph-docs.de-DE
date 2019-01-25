---
title: assignLicense
description: Hinzufügen oder Entfernen von Lizenzen für den Benutzer aktivieren oder Deaktivieren der Verwendung von Microsoft-Cloud-angeboten. Beispielsweise eine Organisation kann ein Office 365 Enterprise E3-Abonnement mit 100 Lizenzen verfügen, und diese Anforderung weist eine der Lizenzen, die für einen bestimmten Benutzer. Sie können auch aktivieren und Deaktivieren von bestimmten Pläne ein Abonnement zugeordnet. Weitere Informationen zu Abonnements und Lizenzen finden Sie unter Technet-Artikel.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d15202d24148b2f75bd857500117a4f97b61fe51
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510498"
---
# <a name="assignlicense"></a><span data-ttu-id="18278-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="18278-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18278-107">Hinzufügen oder Entfernen von Lizenzen für den Benutzer aktivieren oder Deaktivieren der Verwendung von Microsoft-Cloud-angeboten.</span><span class="sxs-lookup"><span data-stu-id="18278-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="18278-108">Beispielsweise eine Organisation kann ein Office 365 Enterprise E3-Abonnement mit 100 Lizenzen verfügen, und diese Anforderung weist eine der Lizenzen, die für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="18278-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="18278-109">Sie können auch aktivieren und Deaktivieren von bestimmten Pläne ein Abonnement zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="18278-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="18278-110">Weitere Informationen zu Abonnements und Lizenzen finden Sie unter in diesem [Technet-Artikel](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="18278-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="18278-111">Wenn die im Verzeichnis Abonnements erhalten möchten, führen Sie eine [GET-Anforderung SubscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="18278-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="18278-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18278-112">Permissions</span></span>
<span data-ttu-id="18278-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18278-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18278-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18278-115">Permission type</span></span>      | <span data-ttu-id="18278-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18278-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18278-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18278-117">Delegated (work or school account)</span></span> | <span data-ttu-id="18278-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18278-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="18278-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18278-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18278-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18278-120">Not supported.</span></span>    |
|<span data-ttu-id="18278-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18278-121">Application</span></span> | <span data-ttu-id="18278-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18278-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18278-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18278-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="18278-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18278-124">Request headers</span></span>
| <span data-ttu-id="18278-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="18278-125">Header</span></span>       | <span data-ttu-id="18278-126">Wert</span><span class="sxs-lookup"><span data-stu-id="18278-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18278-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="18278-127">Authorization</span></span>  | <span data-ttu-id="18278-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18278-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18278-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18278-130">Content-Type</span></span>  | <span data-ttu-id="18278-131">application/json</span><span class="sxs-lookup"><span data-stu-id="18278-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18278-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18278-132">Request body</span></span>
<span data-ttu-id="18278-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="18278-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18278-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="18278-134">Parameter</span></span>    | <span data-ttu-id="18278-135">Typ</span><span class="sxs-lookup"><span data-stu-id="18278-135">Type</span></span>   |<span data-ttu-id="18278-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18278-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18278-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="18278-137">addLicenses</span></span>|<span data-ttu-id="18278-138">[assignedLicense](../resources/assignedlicense.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="18278-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="18278-139">Eine Auflistung von [AssignedLicense](../resources/assignedlicense.md) -Objekten, die die hinzuzufügenden Lizenzen angeben.</span><span class="sxs-lookup"><span data-stu-id="18278-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="18278-140">Sie können eine Lizenz zugeordnet sind, indem die **DisabledPlans** -Eigenschaft für ein Objekt [AssignedLicense](../resources/assignedlicense.md) ServicePlans deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="18278-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="18278-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="18278-141">removeLicenses</span></span>|<span data-ttu-id="18278-142">Guid</span><span class="sxs-lookup"><span data-stu-id="18278-142">Guid</span></span>|<span data-ttu-id="18278-143">Eine Auflistung von SkuIds, die die zu entfernenden Lizenzen zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="18278-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="18278-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="18278-144">Response</span></span>

<span data-ttu-id="18278-145">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine aktualisierte [Benutzer](../resources/user.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18278-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18278-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18278-146">Example</span></span>
<span data-ttu-id="18278-147">Lizenzen für den Benutzer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="18278-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="18278-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18278-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a><span data-ttu-id="18278-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18278-149">Example</span></span>
<span data-ttu-id="18278-150">Entfernen Sie Lizenzen vom Benutzer.</span><span class="sxs-lookup"><span data-stu-id="18278-150">Remove licenses from the user.</span></span>

#####<a name="request"></a><span data-ttu-id="18278-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18278-151">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="18278-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="18278-152">Response</span></span>
<span data-ttu-id="18278-153">In beiden Beispielen wird die Antwort das aktualisierte Benutzerobjekt.</span><span class="sxs-lookup"><span data-stu-id="18278-153">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="18278-154">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="18278-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="18278-155">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18278-155">All of the properties will be returned from an actual call.</span></span>
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
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
