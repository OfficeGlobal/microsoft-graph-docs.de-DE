---
title: Verwenden der Microsoft Bookings-API in Microsoft Graph
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7fc58a4fe0fb616963fd91d83a401d4ad8e1c43e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529859"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="fbeb2-104">Verwenden der Microsoft Bookings-API in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fbeb2-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="fbeb2-105">Mit Microsoft Bookings können Kleinunternehmer mit geringem Aufwand Kundenbuchungen und -informationen verwalten.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-105">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="fbeb2-106">Ein Geschäftsinhaber kann ein oder mehrere Unternehmen erstellen, wobei jedes Unternehmen ein eigenes Angebot an Diensten beinhaltet.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-106">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="fbeb2-107">Der Geschäftsinhaber kann Mitarbeiter einrichten und Dienste angeben, die jeder Mitarbeiter ausführt.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-107">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="fbeb2-108">Ein Kunde kann einen Termin für einen bestimmten Dienst in diesem Unternehmen entweder online oder über eine mobile App buchen.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-108">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="fbeb2-109">Mit Bookings wird sichergestellt, dass der Termin für das Unternehmen, die Mitarbeiter und die jeweils involvierten Kunden auf dem neuesten Stand ist.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-109">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="fbeb2-110">Ein [bookingBusiness](bookingbusiness.md)-Objekt umfasst programmgesteuert in der Bookings-API die folgenden Objekte:</span><span class="sxs-lookup"><span data-stu-id="fbeb2-110">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="fbeb2-111">Ein oder mehrere [bookingStaffMember](bookingstaffmember.md)-Objekte</span><span class="sxs-lookup"><span data-stu-id="fbeb2-111">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="fbeb2-112">Ein oder mehrere [bookingservice](bookingservice.md)-Objekte</span><span class="sxs-lookup"><span data-stu-id="fbeb2-112">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="fbeb2-113">Mehrere [bookingAppointment](bookingappointment.md)-Instanzen</span><span class="sxs-lookup"><span data-stu-id="fbeb2-113">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="fbeb2-114">Mehrere [bookingCustomer](bookingcustomer.md)-Objekte</span><span class="sxs-lookup"><span data-stu-id="fbeb2-114">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="fbeb2-115">Verwenden der Bookings-REST-API</span><span class="sxs-lookup"><span data-stu-id="fbeb2-115">Using the Bookings REST API</span></span>

<span data-ttu-id="fbeb2-116">Führen Sie die folgenden Schritte aus, bevor Sie zum ersten Mal Kundentermine für ein Unternehmen buchen.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-116">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="fbeb2-117">Stellen Sie sicher, dass Sie die entsprechenden [Zugriffstoken](/graph/auth-overview) für die entsprechenden Vorgänge bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-117">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="fbeb2-118">Stellen Sie sicher, dass das Unternehmen über ein [Office 365 Business Premium](https://products.office.com/de-DE/business/office-365-business-premium)-Abonnement verfügt.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-118">Make sure the business has an [Office 365 Business Premium](https://products.office.com/de-DE/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="fbeb2-119">Erstellen Sie ein neues **bookingBusiness**-Objekt, indem Sie einen POST-Vorgang an die Entitätenmenge senden.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-119">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="fbeb2-120">Sie sollten mindestens einen Namen für das neue Unternehmen angeben, das Kunden angezeigt wird: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="fbeb2-120">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="fbeb2-121">Verwenden Sie die **id**-Eigenschaft des neuen **bookingBusiness**-Objekts, das in der POST-Antwort zurückgegeben wurde, um mit dem [Anpassen](../api/bookingbusiness-update.md) der Unternehmenseinstellungen fortzufahren, und fügen Sie Mitarbeiter und Dienste für das Unternehmen hinzu.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-121">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="fbeb2-122">Fügen Sie einzelne Mitarbeiter für das Unternehmen hinzu: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="fbeb2-122">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. <span data-ttu-id="fbeb2-123">Definieren Sie jeden Dienst, der vom Unternehmen angeboten wird: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="fbeb2-123">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="fbeb2-124">Veröffentlichen Sie die Seite für die Terminvergabe für das Unternehmen, damit Kunden und Betreiber des Unternehmens Termine buchen können: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="fbeb2-124">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="fbeb2-125">So können Sie generell alle Unternehmen mit Bookings im Office 365-Mandanten auflisten: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="fbeb2-125">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="fbeb2-126">Allgemeine Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="fbeb2-126">Common use cases</span></span> 

<span data-ttu-id="fbeb2-127">Die folgende Tabelle enthält die allgemeinen Vorgänge für ein Unternehmen in der Bookings-API.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-127">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="fbeb2-128">Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="fbeb2-128">Use cases</span></span>        | <span data-ttu-id="fbeb2-129">REST-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="fbeb2-129">REST resources</span></span> | <span data-ttu-id="fbeb2-130">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fbeb2-130">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="fbeb2-131">Erstellen, Abrufen, Aktualisieren oder Löschen eines Unternehmens</span><span class="sxs-lookup"><span data-stu-id="fbeb2-131">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="fbeb2-132">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="fbeb2-132">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="fbeb2-133">Methoden von bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="fbeb2-133">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="fbeb2-134">Aktualisieren der Richtlinie für die Terminvergabe</span><span class="sxs-lookup"><span data-stu-id="fbeb2-134">Update the scheduling policy</span></span> | [<span data-ttu-id="fbeb2-135">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="fbeb2-135">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="fbeb2-136">Aktualisieren von bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="fbeb2-136">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="fbeb2-137">Hinzufügen, Abrufen, Aktualisieren oder Löschen von Mitarbeitern</span><span class="sxs-lookup"><span data-stu-id="fbeb2-137">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="fbeb2-138">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="fbeb2-138">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="fbeb2-139">Methoden von bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="fbeb2-139">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="fbeb2-140">Hinzufügen, Abrufen, Aktualisieren oder Löschen von Diensten</span><span class="sxs-lookup"><span data-stu-id="fbeb2-140">Add, get, update, or delete services</span></span> | [<span data-ttu-id="fbeb2-141">bookingService</span><span class="sxs-lookup"><span data-stu-id="fbeb2-141">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="fbeb2-142">Methoden von bookingService</span><span class="sxs-lookup"><span data-stu-id="fbeb2-142">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="fbeb2-143">Veröffentlichen oder Aufheben der Veröffentlichung der Seite für die Terminvergabe</span><span class="sxs-lookup"><span data-stu-id="fbeb2-143">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="fbeb2-144">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="fbeb2-144">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="fbeb2-145">publish</span><span class="sxs-lookup"><span data-stu-id="fbeb2-145">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="fbeb2-146">unpublish</span><span class="sxs-lookup"><span data-stu-id="fbeb2-146">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="fbeb2-147">Erstellen, Abrufen, Aktualisieren, Löschen oder Absagen von Terminen</span><span class="sxs-lookup"><span data-stu-id="fbeb2-147">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="fbeb2-148">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="fbeb2-148">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="fbeb2-149">Methoden von bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="fbeb2-149">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="fbeb2-150">Abrufen von Terminen in einem Datumsbereich</span><span class="sxs-lookup"><span data-stu-id="fbeb2-150">Get appointments in a date range</span></span> | [<span data-ttu-id="fbeb2-151">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="fbeb2-151">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="fbeb2-152">Auflisten von Bookings für calendarView</span><span class="sxs-lookup"><span data-stu-id="fbeb2-152">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="fbeb2-153">Abrufen der Währung</span><span class="sxs-lookup"><span data-stu-id="fbeb2-153">Get currency</span></span> | [<span data-ttu-id="fbeb2-154">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="fbeb2-154">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="fbeb2-155">Methoden von bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="fbeb2-155">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="fbeb2-156">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fbeb2-156">See also</span></span>

- <span data-ttu-id="fbeb2-157">Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="fbeb2-158">Sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).</span><span class="sxs-lookup"><span data-stu-id="fbeb2-158">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="fbeb2-159">Erfahren Sie, wie [Berechtigungen](/graph/permissions-reference) in Microsoft Graph ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="fbeb2-159">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/booking-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
