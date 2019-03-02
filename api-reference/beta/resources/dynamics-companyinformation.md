---
title: companyInformation-Ressourcentyp
description: Unternehmensinformationen in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365913"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="851d2-103">companyInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="851d2-103">companyInformation resource type</span></span>
<span data-ttu-id="851d2-104">Stellt die für das aktuelle Unternehmen in Dynamics 365 Business Central angegebenen Informationen wie Name, Adresse, e-Mail-Adresse und Websiteadresse dar.</span><span class="sxs-lookup"><span data-stu-id="851d2-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="851d2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="851d2-105">Methods</span></span>

| <span data-ttu-id="851d2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="851d2-106">Method</span></span>         | <span data-ttu-id="851d2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="851d2-107">Return Type</span></span>  |<span data-ttu-id="851d2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="851d2-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="851d2-109">CompanyInformation abrufen</span><span class="sxs-lookup"><span data-stu-id="851d2-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="851d2-110">companyInformation</span><span class="sxs-lookup"><span data-stu-id="851d2-110">companyInformation</span></span>|<span data-ttu-id="851d2-111">Ruft Unternehmensinformationen ab.</span><span class="sxs-lookup"><span data-stu-id="851d2-111">Gets a company information.</span></span>|
|[<span data-ttu-id="851d2-112">Patch-companyInformation</span><span class="sxs-lookup"><span data-stu-id="851d2-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="851d2-113">companyInformation</span><span class="sxs-lookup"><span data-stu-id="851d2-113">companyInformation</span></span>|<span data-ttu-id="851d2-114">Aktualisiert Unternehmensinformationen.</span><span class="sxs-lookup"><span data-stu-id="851d2-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="851d2-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="851d2-115">Properties</span></span>
| <span data-ttu-id="851d2-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="851d2-116">Property</span></span>     | <span data-ttu-id="851d2-117">Typ</span><span class="sxs-lookup"><span data-stu-id="851d2-117">Type</span></span>      |<span data-ttu-id="851d2-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="851d2-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="851d2-119">id</span><span class="sxs-lookup"><span data-stu-id="851d2-119">id</span></span>            |<span data-ttu-id="851d2-120">GUID</span><span class="sxs-lookup"><span data-stu-id="851d2-120">GUID</span></span>|<span data-ttu-id="851d2-121">Die eindeutige ID des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-121">The unique ID of the company.</span></span> <span data-ttu-id="851d2-122">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="851d2-122">Non-editable.</span></span>|
|<span data-ttu-id="851d2-123">displayName</span><span class="sxs-lookup"><span data-stu-id="851d2-123">displayName</span></span>   |<span data-ttu-id="851d2-124">string</span><span class="sxs-lookup"><span data-stu-id="851d2-124">string</span></span>   |<span data-ttu-id="851d2-125">Der Anzeigename des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-125">The company's display name.</span></span>           |
|<span data-ttu-id="851d2-126">address</span><span class="sxs-lookup"><span data-stu-id="851d2-126">address</span></span>       |[<span data-ttu-id="851d2-127">Navigations. PostalAddress</span><span class="sxs-lookup"><span data-stu-id="851d2-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="851d2-128">Die Adresse des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-128">The company's address.</span></span> <span data-ttu-id="851d2-129">Zeigen Sie den komplexen Typ für zusätzliche Details an.</span><span class="sxs-lookup"><span data-stu-id="851d2-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="851d2-130">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="851d2-130">phoneNumber</span></span>   |<span data-ttu-id="851d2-131">string</span><span class="sxs-lookup"><span data-stu-id="851d2-131">string</span></span>   |<span data-ttu-id="851d2-132">Die Telefonnummer des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="851d2-133">faxNumber</span><span class="sxs-lookup"><span data-stu-id="851d2-133">faxNumber</span></span>     |<span data-ttu-id="851d2-134">string</span><span class="sxs-lookup"><span data-stu-id="851d2-134">string</span></span>   |<span data-ttu-id="851d2-135">Die Faxnummer des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-135">The company's fax number.</span></span>             |
|<span data-ttu-id="851d2-136">email</span><span class="sxs-lookup"><span data-stu-id="851d2-136">email</span></span>         |<span data-ttu-id="851d2-137">string</span><span class="sxs-lookup"><span data-stu-id="851d2-137">string</span></span>   |<span data-ttu-id="851d2-138">Die e-Mail-Adresse des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-138">The company's email address.</span></span>          |
|<span data-ttu-id="851d2-139">Website</span><span class="sxs-lookup"><span data-stu-id="851d2-139">website</span></span>       |<span data-ttu-id="851d2-140">string</span><span class="sxs-lookup"><span data-stu-id="851d2-140">string</span></span>   |<span data-ttu-id="851d2-141">Die Websiteadresse des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-141">The company's website address.</span></span>        |
|<span data-ttu-id="851d2-142">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="851d2-142">taxRegistrationNumber</span></span>|<span data-ttu-id="851d2-143">string</span><span class="sxs-lookup"><span data-stu-id="851d2-143">string</span></span>|<span data-ttu-id="851d2-144">Die Steuernummer des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="851d2-145">currencyCode</span><span class="sxs-lookup"><span data-stu-id="851d2-145">currencyCode</span></span>  |<span data-ttu-id="851d2-146">string</span><span class="sxs-lookup"><span data-stu-id="851d2-146">string</span></span>   |<span data-ttu-id="851d2-147">Die Währung, in der das Unternehmen tätig ist.</span><span class="sxs-lookup"><span data-stu-id="851d2-147">The currency the company does business in.</span></span> <span data-ttu-id="851d2-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="851d2-148">Read-Only.</span></span>|
|<span data-ttu-id="851d2-149">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="851d2-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="851d2-150">date</span><span class="sxs-lookup"><span data-stu-id="851d2-150">date</span></span>|<span data-ttu-id="851d2-151">Das aktuelle Geschäftsjahr-Anfangsdatum des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="851d2-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="851d2-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="851d2-152">Read-Only.</span></span>|
|<span data-ttu-id="851d2-153">Industrie</span><span class="sxs-lookup"><span data-stu-id="851d2-153">industry</span></span>      |<span data-ttu-id="851d2-154">string</span><span class="sxs-lookup"><span data-stu-id="851d2-154">string</span></span>   |<span data-ttu-id="851d2-155">Die Branche, zu der das Unternehmen gehört.</span><span class="sxs-lookup"><span data-stu-id="851d2-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="851d2-156">Bild</span><span class="sxs-lookup"><span data-stu-id="851d2-156">picture</span></span>       |<span data-ttu-id="851d2-157">stream</span><span class="sxs-lookup"><span data-stu-id="851d2-157">stream</span></span>   |<span data-ttu-id="851d2-158">Das Firmen Logo.</span><span class="sxs-lookup"><span data-stu-id="851d2-158">The company logo.</span></span> <span data-ttu-id="851d2-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="851d2-159">Read-Only.</span></span>          |
|<span data-ttu-id="851d2-160">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="851d2-160">businessProfileId</span></span>|<span data-ttu-id="851d2-161">string</span><span class="sxs-lookup"><span data-stu-id="851d2-161">string</span></span>|<span data-ttu-id="851d2-162">Die Geschäftsprofil-ID, die mit dem Financials-Unternehmen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="851d2-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="851d2-163">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="851d2-163">Read-Only.</span></span>|
|<span data-ttu-id="851d2-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="851d2-164">lastModifiedDateTime</span></span>|<span data-ttu-id="851d2-165">DateTime</span><span class="sxs-lookup"><span data-stu-id="851d2-165">datetime</span></span>|<span data-ttu-id="851d2-166">Die letzte Uhrzeit, zu der das Unternehmen geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="851d2-166">The last datetime the company was modified.</span></span> <span data-ttu-id="851d2-167">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="851d2-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="851d2-168">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="851d2-168">Relationships</span></span>
<span data-ttu-id="851d2-169">Keine</span><span class="sxs-lookup"><span data-stu-id="851d2-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="851d2-170">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="851d2-170">JSON representation</span></span>

<span data-ttu-id="851d2-171">Es folgt eine JSON-Darstellung des companyInformation</span><span class="sxs-lookup"><span data-stu-id="851d2-171">Here is a JSON representation of the companyInformation</span></span>
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```

