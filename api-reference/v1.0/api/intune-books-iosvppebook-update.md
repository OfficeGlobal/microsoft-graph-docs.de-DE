---
title: Aktualisieren von „iosVppEBook“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac75fef4b902c77f36f3a8559b40bad252a5336a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836092"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="67419-103">Aktualisieren von „iosVppEBook“</span><span class="sxs-lookup"><span data-stu-id="67419-103">Update iosVppEBook</span></span>

> <span data-ttu-id="67419-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="67419-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67419-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67419-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="67419-106">Prerequisites</span></span>
<span data-ttu-id="67419-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67419-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67419-109">Permission type</span></span>|<span data-ttu-id="67419-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67419-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67419-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67419-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67419-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67419-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67419-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67419-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67419-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67419-114">Not supported.</span></span>|
|<span data-ttu-id="67419-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67419-115">Application</span></span>|<span data-ttu-id="67419-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67419-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67419-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67419-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="67419-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67419-118">Request headers</span></span>
|<span data-ttu-id="67419-119">Header</span><span class="sxs-lookup"><span data-stu-id="67419-119">Header</span></span>|<span data-ttu-id="67419-120">Wert</span><span class="sxs-lookup"><span data-stu-id="67419-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67419-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67419-121">Authorization</span></span>|<span data-ttu-id="67419-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="67419-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67419-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="67419-123">Accept</span></span>|<span data-ttu-id="67419-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67419-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67419-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67419-125">Request body</span></span>
<span data-ttu-id="67419-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) an.</span><span class="sxs-lookup"><span data-stu-id="67419-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="67419-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="67419-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="67419-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67419-128">Property</span></span>|<span data-ttu-id="67419-129">Typ</span><span class="sxs-lookup"><span data-stu-id="67419-129">Type</span></span>|<span data-ttu-id="67419-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67419-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67419-131">id</span><span class="sxs-lookup"><span data-stu-id="67419-131">id</span></span>|<span data-ttu-id="67419-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-132">String</span></span>|<span data-ttu-id="67419-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="67419-133">Key of the entity.</span></span> <span data-ttu-id="67419-134">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-135">displayName</span><span class="sxs-lookup"><span data-stu-id="67419-135">displayName</span></span>|<span data-ttu-id="67419-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-136">String</span></span>|<span data-ttu-id="67419-137">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="67419-137">Name of the eBook.</span></span> <span data-ttu-id="67419-138">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-139">description</span><span class="sxs-lookup"><span data-stu-id="67419-139">description</span></span>|<span data-ttu-id="67419-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-140">String</span></span>|<span data-ttu-id="67419-141">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="67419-141">Description.</span></span> <span data-ttu-id="67419-142">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-143">publisher</span><span class="sxs-lookup"><span data-stu-id="67419-143">publisher</span></span>|<span data-ttu-id="67419-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-144">String</span></span>|<span data-ttu-id="67419-145">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="67419-145">Publisher.</span></span> <span data-ttu-id="67419-146">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="67419-147">publishedDateTime</span></span>|<span data-ttu-id="67419-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67419-148">DateTimeOffset</span></span>|<span data-ttu-id="67419-149">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="67419-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="67419-150">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="67419-151">largeCover</span></span>|[<span data-ttu-id="67419-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="67419-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="67419-153">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="67419-153">Book cover.</span></span> <span data-ttu-id="67419-154">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67419-155">createdDateTime</span></span>|<span data-ttu-id="67419-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67419-156">DateTimeOffset</span></span>|<span data-ttu-id="67419-157">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="67419-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="67419-158">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67419-159">lastModifiedDateTime</span></span>|<span data-ttu-id="67419-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67419-160">DateTimeOffset</span></span>|<span data-ttu-id="67419-161">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="67419-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="67419-162">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="67419-163">informationUrl</span></span>|<span data-ttu-id="67419-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-164">String</span></span>|<span data-ttu-id="67419-165">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="67419-165">The more information Url.</span></span> <span data-ttu-id="67419-166">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="67419-167">privacyInformationUrl</span></span>|<span data-ttu-id="67419-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-168">String</span></span>|<span data-ttu-id="67419-169">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="67419-169">The privacy statement Url.</span></span> <span data-ttu-id="67419-170">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="67419-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67419-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="67419-171">vppTokenId</span></span>|<span data-ttu-id="67419-172">Guid</span><span class="sxs-lookup"><span data-stu-id="67419-172">Guid</span></span>|<span data-ttu-id="67419-173">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="67419-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="67419-174">appleId</span><span class="sxs-lookup"><span data-stu-id="67419-174">appleId</span></span>|<span data-ttu-id="67419-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-175">String</span></span>|<span data-ttu-id="67419-176">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="67419-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="67419-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="67419-177">vppOrganizationName</span></span>|<span data-ttu-id="67419-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-178">String</span></span>|<span data-ttu-id="67419-179">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="67419-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="67419-180">genres</span><span class="sxs-lookup"><span data-stu-id="67419-180">genres</span></span>|<span data-ttu-id="67419-181">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="67419-181">String collection</span></span>|<span data-ttu-id="67419-182">Genres</span><span class="sxs-lookup"><span data-stu-id="67419-182">Genres.</span></span>|
|<span data-ttu-id="67419-183">language</span><span class="sxs-lookup"><span data-stu-id="67419-183">language</span></span>|<span data-ttu-id="67419-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-184">String</span></span>|<span data-ttu-id="67419-185">Sprache</span><span class="sxs-lookup"><span data-stu-id="67419-185">Language.</span></span>|
|<span data-ttu-id="67419-186">seller</span><span class="sxs-lookup"><span data-stu-id="67419-186">seller</span></span>|<span data-ttu-id="67419-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67419-187">String</span></span>|<span data-ttu-id="67419-188">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="67419-188">Seller.</span></span>|
|<span data-ttu-id="67419-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67419-189">totalLicenseCount</span></span>|<span data-ttu-id="67419-190">Int32</span><span class="sxs-lookup"><span data-stu-id="67419-190">Int32</span></span>|<span data-ttu-id="67419-191">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="67419-191">Total license count.</span></span>|
|<span data-ttu-id="67419-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67419-192">usedLicenseCount</span></span>|<span data-ttu-id="67419-193">Int32</span><span class="sxs-lookup"><span data-stu-id="67419-193">Int32</span></span>|<span data-ttu-id="67419-194">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="67419-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="67419-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="67419-195">Response</span></span>
<span data-ttu-id="67419-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="67419-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67419-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67419-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="67419-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67419-198">Request</span></span>
<span data-ttu-id="67419-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67419-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="67419-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="67419-200">Response</span></span>
<span data-ttu-id="67419-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67419-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```



