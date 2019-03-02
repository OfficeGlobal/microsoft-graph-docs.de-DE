---
title: Employees-Ressourcentyp
description: Ein Employee-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366655"
---
# <a name="employees-resource-type"></a><span data-ttu-id="0e852-103">Employees-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0e852-103">employees resource type</span></span>
<span data-ttu-id="0e852-104">Stellt einen Mitarbeiter in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="0e852-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0e852-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="0e852-105">Methods</span></span>

| <span data-ttu-id="0e852-106">Methode</span><span class="sxs-lookup"><span data-stu-id="0e852-106">Method</span></span>                                              | <span data-ttu-id="0e852-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0e852-107">Return Type</span></span>|<span data-ttu-id="0e852-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e852-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="0e852-109">Mitarbeiter abrufen</span><span class="sxs-lookup"><span data-stu-id="0e852-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="0e852-110">Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="0e852-110">employees</span></span>  |<span data-ttu-id="0e852-111">Rufen Sie ein Employee-Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="0e852-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="0e852-112">Post Angestellte</span><span class="sxs-lookup"><span data-stu-id="0e852-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="0e852-113">Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="0e852-113">employees</span></span>  |<span data-ttu-id="0e852-114">Erstellen eines Employee-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e852-114">Create an employee object.</span></span>|
|[<span data-ttu-id="0e852-115">Patch-Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="0e852-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="0e852-116">Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="0e852-116">employees</span></span>  |<span data-ttu-id="0e852-117">Aktualisieren eines Employee-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e852-117">Update an employee object.</span></span>|
|[<span data-ttu-id="0e852-118">Mitarbeiter löschen</span><span class="sxs-lookup"><span data-stu-id="0e852-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="0e852-119">Keine</span><span class="sxs-lookup"><span data-stu-id="0e852-119">none</span></span>       |<span data-ttu-id="0e852-120">Löschen eines Employee-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e852-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e852-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e852-121">Properties</span></span>
| <span data-ttu-id="0e852-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e852-122">Property</span></span>           | <span data-ttu-id="0e852-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0e852-123">Type</span></span>   |<span data-ttu-id="0e852-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e852-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="0e852-125">id</span><span class="sxs-lookup"><span data-stu-id="0e852-125">id</span></span>                  |<span data-ttu-id="0e852-126">GUID</span><span class="sxs-lookup"><span data-stu-id="0e852-126">GUID</span></span>    |<span data-ttu-id="0e852-127">Die Mitarbeiter-ID.</span><span class="sxs-lookup"><span data-stu-id="0e852-127">The employee ID.</span></span> <span data-ttu-id="0e852-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="0e852-128">Non-editable.</span></span>                         |
|<span data-ttu-id="0e852-129">number</span><span class="sxs-lookup"><span data-stu-id="0e852-129">number</span></span>              |<span data-ttu-id="0e852-130">string</span><span class="sxs-lookup"><span data-stu-id="0e852-130">string</span></span>  |<span data-ttu-id="0e852-131">Die Mitarbeiternummer.</span><span class="sxs-lookup"><span data-stu-id="0e852-131">The employee number.</span></span> <span data-ttu-id="0e852-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0e852-132">Read-Only.</span></span>                        |
|<span data-ttu-id="0e852-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0e852-133">displayName</span></span>         |<span data-ttu-id="0e852-134">String</span><span class="sxs-lookup"><span data-stu-id="0e852-134">string</span></span>  |<span data-ttu-id="0e852-135">Der angegebene Name und Nachname des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="0e852-135">The employee givenName + surname.</span></span> <span data-ttu-id="0e852-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0e852-136">Read-Only.</span></span>           |
|<span data-ttu-id="0e852-137">givenName</span><span class="sxs-lookup"><span data-stu-id="0e852-137">givenName</span></span>           |<span data-ttu-id="0e852-138">string</span><span class="sxs-lookup"><span data-stu-id="0e852-138">string</span></span>  |<span data-ttu-id="0e852-139">Der angegebene Name des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="0e852-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="0e852-140">middleName</span><span class="sxs-lookup"><span data-stu-id="0e852-140">middleName</span></span>          |<span data-ttu-id="0e852-141">string</span><span class="sxs-lookup"><span data-stu-id="0e852-141">string</span></span>  |<span data-ttu-id="0e852-142">Der Vorname des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="0e852-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="0e852-143">surname</span><span class="sxs-lookup"><span data-stu-id="0e852-143">surname</span></span>             |<span data-ttu-id="0e852-144">string</span><span class="sxs-lookup"><span data-stu-id="0e852-144">string</span></span>  |<span data-ttu-id="0e852-145">Der Nachname des Mitarbeiters</span><span class="sxs-lookup"><span data-stu-id="0e852-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="0e852-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0e852-146">jobTitle</span></span>            |<span data-ttu-id="0e852-147">string</span><span class="sxs-lookup"><span data-stu-id="0e852-147">string</span></span>  |<span data-ttu-id="0e852-148">Der vollständige Name des Mitarbeiters</span><span class="sxs-lookup"><span data-stu-id="0e852-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="0e852-149">address</span><span class="sxs-lookup"><span data-stu-id="0e852-149">address</span></span>             |[<span data-ttu-id="0e852-150">Navigations. PostalAddress</span><span class="sxs-lookup"><span data-stu-id="0e852-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="0e852-151">Gibt die Adresse des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-151">Specifies the employee's address.</span></span> <span data-ttu-id="0e852-152">Diese Adresse wird in allen Ressourcen Dokumenten des Mitarbeiters angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0e852-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="0e852-153">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0e852-153">phoneNumber</span></span>         |<span data-ttu-id="0e852-154">string</span><span class="sxs-lookup"><span data-stu-id="0e852-154">string</span></span>  |<span data-ttu-id="0e852-155">Gibt die Telefonnummer des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="0e852-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0e852-156">mobilePhone</span></span>         |<span data-ttu-id="0e852-157">string</span><span class="sxs-lookup"><span data-stu-id="0e852-157">string</span></span>  |<span data-ttu-id="0e852-158">Gibt die Mobiltelefonnummer des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="0e852-159">email</span><span class="sxs-lookup"><span data-stu-id="0e852-159">email</span></span>               |<span data-ttu-id="0e852-160">string</span><span class="sxs-lookup"><span data-stu-id="0e852-160">string</span></span>  |<span data-ttu-id="0e852-161">Gibt die e-Mail-Adresse des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="0e852-162">personalEmail</span><span class="sxs-lookup"><span data-stu-id="0e852-162">personalEmail</span></span>       |<span data-ttu-id="0e852-163">string</span><span class="sxs-lookup"><span data-stu-id="0e852-163">string</span></span>  |<span data-ttu-id="0e852-164">Gibt die persönliche e-Mail-Adresse des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="0e852-165">employmentDate</span><span class="sxs-lookup"><span data-stu-id="0e852-165">employmentDate</span></span>      |<span data-ttu-id="0e852-166">date</span><span class="sxs-lookup"><span data-stu-id="0e852-166">date</span></span>    |<span data-ttu-id="0e852-167">Gibt das Datum an, an dem der Mitarbeiter begonnen hat, für das Unternehmen zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="0e852-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="0e852-168">terminationDate</span><span class="sxs-lookup"><span data-stu-id="0e852-168">terminationDate</span></span>     |<span data-ttu-id="0e852-169">date</span><span class="sxs-lookup"><span data-stu-id="0e852-169">date</span></span>    |<span data-ttu-id="0e852-170">Gibt das Datum an, an dem der Mitarbeiter beendet wurde, beispielsweise aufgrund eines Ausfalls oder einer Kündigung.</span><span class="sxs-lookup"><span data-stu-id="0e852-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="0e852-171">status</span><span class="sxs-lookup"><span data-stu-id="0e852-171">status</span></span>              |<span data-ttu-id="0e852-172">string</span><span class="sxs-lookup"><span data-stu-id="0e852-172">string</span></span>  |<span data-ttu-id="0e852-173">Gibt den Status des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-173">Specifies the employee's status.</span></span> <span data-ttu-id="0e852-174">Mögliche Werte sind aktiv, inaktiv oder terminiert</span><span class="sxs-lookup"><span data-stu-id="0e852-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="0e852-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="0e852-175">birthDate</span></span>           |<span data-ttu-id="0e852-176">date</span><span class="sxs-lookup"><span data-stu-id="0e852-176">date</span></span>    |<span data-ttu-id="0e852-177">Gibt das Geburtsdatum des Mitarbeiters an.</span><span class="sxs-lookup"><span data-stu-id="0e852-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="0e852-178">Bild</span><span class="sxs-lookup"><span data-stu-id="0e852-178">picture</span></span>             |<span data-ttu-id="0e852-179">stream</span><span class="sxs-lookup"><span data-stu-id="0e852-179">stream</span></span>  |<span data-ttu-id="0e852-180">Das Bild des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="0e852-180">The employee picture.</span></span> <span data-ttu-id="0e852-181">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0e852-181">Read-Only.</span></span>                       |
|<span data-ttu-id="0e852-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e852-182">lastModifiedDateTime</span></span>|<span data-ttu-id="0e852-183">DateTime</span><span class="sxs-lookup"><span data-stu-id="0e852-183">datetime</span></span>|<span data-ttu-id="0e852-184">Die letzte DateTime, die der Mitarbeiter geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0e852-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="0e852-185">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0e852-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="0e852-186">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0e852-186">Relationships</span></span>
<span data-ttu-id="0e852-187">Keine</span><span class="sxs-lookup"><span data-stu-id="0e852-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e852-188">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e852-188">JSON representation</span></span>

<span data-ttu-id="0e852-189">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e852-189">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

