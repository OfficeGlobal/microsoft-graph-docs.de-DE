---
title: Verwenden Sie die Microsoft-Buchungen API in Microsoft Graph
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Priority
ms.openlocfilehash: def9260654baafe1953d629265c4b76a2afd2748
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845535"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="8f968-104">Verwenden Sie die Microsoft-Buchungen API in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8f968-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 > <span data-ttu-id="8f968-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f968-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f968-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f968-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="8f968-107">Microsoft Bookings können Kleinunternehmen Besitzer Kunden Buchungen und Informationen mit minimalem Setup zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="8f968-107">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="8f968-108">Eigentümer eines Unternehmens kann eine oder mehrere Unternehmen mit jedem Business bietet eine Reihe von Diensten erstellen.</span><span class="sxs-lookup"><span data-stu-id="8f968-108">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="8f968-109">Der Besitzer kann Einrichten von Mitarbeitern, und geben Sie die Dienste, die jeder Mitarbeiter durchführt.</span><span class="sxs-lookup"><span data-stu-id="8f968-109">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="8f968-110">Ein Kunde kann einen Termin für einen bestimmten Dienst in dieses Unternehmen in einer app online oder mobilen Buch.</span><span class="sxs-lookup"><span data-stu-id="8f968-110">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="8f968-111">Buchungen stellt sicher, dass, die die Zeit des Termins für die Business, Mitarbeitern und Kunden beteiligten aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="8f968-111">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="8f968-112">Programmgesteuertes, umfasst eine [BookingBusiness](bookingbusiness.md) in der Buchungen API die folgenden Objekte:</span><span class="sxs-lookup"><span data-stu-id="8f968-112">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="8f968-113">Ein oder mehrere [BookingStaffMember](bookingstaffmember.md) -Objekte</span><span class="sxs-lookup"><span data-stu-id="8f968-113">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="8f968-114">Ein oder mehrere [BookingService](bookingservice.md) -Objekte</span><span class="sxs-lookup"><span data-stu-id="8f968-114">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="8f968-115">Eine Reihe von [BookingAppointment](bookingappointment.md) Instanzen</span><span class="sxs-lookup"><span data-stu-id="8f968-115">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="8f968-116">Eine Reihe von [BookingCustomer](bookingcustomer.md) -Objekten</span><span class="sxs-lookup"><span data-stu-id="8f968-116">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="8f968-117">Verwenden die Buchungen REST-API</span><span class="sxs-lookup"><span data-stu-id="8f968-117">Using the Bookings REST API</span></span>

<span data-ttu-id="8f968-118">Lernen Sie die folgenden Schritte vor dem Buchen Kundenterminen für ein Unternehmen beim ersten.</span><span class="sxs-lookup"><span data-stu-id="8f968-118">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="8f968-119">Stellen Sie sicher, dass Sie die entsprechenden [Zugriffstoken](/graph/auth-overview) für die entsprechenden Vorgänge angeben.</span><span class="sxs-lookup"><span data-stu-id="8f968-119">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="8f968-120">Stellen Sie sicher, dass das Unternehmen ein [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) -Abonnement verfügt.</span><span class="sxs-lookup"><span data-stu-id="8f968-120">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="8f968-121">Erstellen einer neuen **BookingBusiness** durch Senden einer POST-Operation auf die Entität.</span><span class="sxs-lookup"><span data-stu-id="8f968-121">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="8f968-122">Mindestens sollten Sie einen Namen für die neue Business angeben, die Kunden angezeigt werden:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f968-122">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="8f968-123">Verwenden Sie die **Id** -Eigenschaft des neuen **BookingBusiness** in der POST-Antwort zurückgegeben Business Einstellungen [Anpassen](../api/bookingbusiness-update.md) möchten, und fügen Sie Mitarbeiter und Dienste für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="8f968-123">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="8f968-124">Fügen Sie einzelne Mitarbeiter für das Unternehmen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f968-124">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
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
4. <span data-ttu-id="8f968-125">Definieren Sie jeden Dienst, der vom Unternehmen angeboten:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f968-125">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="8f968-126">Veröffentlichen der scheduling Seite für das Unternehmen zu Kunden und Unternehmer buchen Termine vornehmen zu lassen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f968-126">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="8f968-127">Im Allgemeinen so Listen Sie alle buchen Unternehmen in Office 365-Mandanten:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f968-127">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="8f968-128">Allgemeine Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="8f968-128">Common use cases</span></span> 

<span data-ttu-id="8f968-129">Die folgende Tabelle enthält die allgemeine Vorgänge für ein Unternehmen in der Buchungen-API.</span><span class="sxs-lookup"><span data-stu-id="8f968-129">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="8f968-130">Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="8f968-130">Use cases</span></span>        | <span data-ttu-id="8f968-131">REST-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="8f968-131">REST resources</span></span> | <span data-ttu-id="8f968-132">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8f968-132">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="8f968-133">Erstellen, abrufen, aktualisieren oder Löschen eines Unternehmens</span><span class="sxs-lookup"><span data-stu-id="8f968-133">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="8f968-134">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8f968-134">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="8f968-135">Methoden des bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8f968-135">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="8f968-136">Aktualisieren der scheduling-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="8f968-136">Update the scheduling policy</span></span> | [<span data-ttu-id="8f968-137">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="8f968-137">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="8f968-138">Aktualisieren einer bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8f968-138">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="8f968-139">Hinzufügen, abrufen, aktualisieren oder Löschen von Mitarbeitern</span><span class="sxs-lookup"><span data-stu-id="8f968-139">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="8f968-140">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8f968-140">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="8f968-141">Methoden des bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8f968-141">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="8f968-142">Hinzufügen, abrufen, aktualisieren oder Löschen von Diensten</span><span class="sxs-lookup"><span data-stu-id="8f968-142">Add, get, update, or delete services</span></span> | [<span data-ttu-id="8f968-143">bookingService</span><span class="sxs-lookup"><span data-stu-id="8f968-143">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="8f968-144">Methoden des bookingService</span><span class="sxs-lookup"><span data-stu-id="8f968-144">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="8f968-145">Veröffentlichen oder Aufheben der Veröffentlichung der Seite scheduling</span><span class="sxs-lookup"><span data-stu-id="8f968-145">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="8f968-146">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8f968-146">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="8f968-147">Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="8f968-147">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="8f968-148">Aufheben der Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="8f968-148">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="8f968-149">Erstellen, abrufen, aktualisieren, löschen oder Abbrechen eines Termins</span><span class="sxs-lookup"><span data-stu-id="8f968-149">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="8f968-150">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="8f968-150">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="8f968-151">Methoden des bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="8f968-151">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="8f968-152">Abrufen von Terminen in einen bestimmten Datumsbereich</span><span class="sxs-lookup"><span data-stu-id="8f968-152">Get appointments in a date range</span></span> | [<span data-ttu-id="8f968-153">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8f968-153">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="8f968-154">Liste Buchungen calendarView</span><span class="sxs-lookup"><span data-stu-id="8f968-154">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="8f968-155">Währung abrufen</span><span class="sxs-lookup"><span data-stu-id="8f968-155">Get currency</span></span> | [<span data-ttu-id="8f968-156">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="8f968-156">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="8f968-157">Methoden des bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="8f968-157">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="8f968-158">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8f968-158">See also</span></span>

- <span data-ttu-id="8f968-159">Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.</span><span class="sxs-lookup"><span data-stu-id="8f968-159">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="8f968-160">Finden Sie unter [wie einige unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).</span><span class="sxs-lookup"><span data-stu-id="8f968-160">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="8f968-161">Erfahren Sie, wie [Berechtigungen](/graph/permissions-reference) in Microsoft Graph entscheiden.</span><span class="sxs-lookup"><span data-stu-id="8f968-161">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
