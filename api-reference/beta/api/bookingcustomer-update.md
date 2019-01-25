---
title: Bookingcustomer aktualisieren
description: Aktualisieren Sie die Eigenschaften eines BookingCustomer-Objekts.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 90de81666335c1825e1d134f9b898ee4b6561664
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525311"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="96e23-103">Bookingcustomer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="96e23-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e23-104">Aktualisieren Sie die Eigenschaften eines [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="96e23-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="96e23-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96e23-105">Permissions</span></span>
<span data-ttu-id="96e23-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e23-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96e23-108">Permission type</span></span>      | <span data-ttu-id="96e23-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96e23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96e23-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96e23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96e23-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="96e23-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="96e23-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96e23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96e23-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96e23-113">Not supported.</span></span>   |
|<span data-ttu-id="96e23-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96e23-114">Application</span></span> | <span data-ttu-id="96e23-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96e23-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="96e23-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96e23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="96e23-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96e23-117">Optional request headers</span></span>
| <span data-ttu-id="96e23-118">Name</span><span class="sxs-lookup"><span data-stu-id="96e23-118">Name</span></span>       | <span data-ttu-id="96e23-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96e23-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="96e23-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e23-120">Authorization</span></span>  | <span data-ttu-id="96e23-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="96e23-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e23-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96e23-122">Request body</span></span>
<span data-ttu-id="96e23-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="96e23-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="96e23-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96e23-126">Property</span></span>     | <span data-ttu-id="96e23-127">Typ</span><span class="sxs-lookup"><span data-stu-id="96e23-127">Type</span></span>   |<span data-ttu-id="96e23-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96e23-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96e23-129">displayName</span><span class="sxs-lookup"><span data-stu-id="96e23-129">displayName</span></span>|<span data-ttu-id="96e23-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96e23-130">String</span></span>|<span data-ttu-id="96e23-131">Der Name des Kunden.</span><span class="sxs-lookup"><span data-stu-id="96e23-131">The name of the customer.</span></span>|
|<span data-ttu-id="96e23-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="96e23-132">emailAddress</span></span>|<span data-ttu-id="96e23-133">String</span><span class="sxs-lookup"><span data-stu-id="96e23-133">String</span></span>|<span data-ttu-id="96e23-134">Die SMTP-Adresse des Kunden.</span><span class="sxs-lookup"><span data-stu-id="96e23-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="96e23-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="96e23-135">Response</span></span>
<span data-ttu-id="96e23-136">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [BookingCustomer](../resources/bookingcustomer.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="96e23-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96e23-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96e23-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96e23-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96e23-138">Request</span></span>
<span data-ttu-id="96e23-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96e23-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="96e23-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="96e23-140">Response</span></span>
<span data-ttu-id="96e23-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96e23-141">The following is an example of the response.</span></span> <span data-ttu-id="96e23-142">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="96e23-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="96e23-143">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96e23-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
