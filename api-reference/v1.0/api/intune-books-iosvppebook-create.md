---
title: iosVppEBook erstellen
description: Erstellt neue Objekte des Typs iosVppEBook.
ms.openlocfilehash: e9a6802a25b76f62a6fc3960648b2265c3ea0de4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017999"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="cb335-103">iosVppEBook erstellen</span><span class="sxs-lookup"><span data-stu-id="cb335-103">Create iosVppEBook</span></span>

> <span data-ttu-id="cb335-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cb335-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb335-105">Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb335-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cb335-106">Prerequisites</span></span>
<span data-ttu-id="cb335-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb335-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb335-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb335-109">Permission type</span></span>|<span data-ttu-id="cb335-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb335-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb335-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb335-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb335-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb335-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb335-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb335-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb335-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb335-114">Not supported.</span></span>|
|<span data-ttu-id="cb335-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb335-115">Application</span></span>|<span data-ttu-id="cb335-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb335-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb335-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb335-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="cb335-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb335-118">Request headers</span></span>
|<span data-ttu-id="cb335-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cb335-119">Header</span></span>|<span data-ttu-id="cb335-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cb335-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb335-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb335-121">Authorization</span></span>|<span data-ttu-id="cb335-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cb335-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb335-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cb335-123">Accept</span></span>|<span data-ttu-id="cb335-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb335-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb335-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb335-125">Request body</span></span>
<span data-ttu-id="cb335-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppEBook-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cb335-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="cb335-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosVppEBook erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cb335-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="cb335-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb335-128">Property</span></span>|<span data-ttu-id="cb335-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cb335-129">Type</span></span>|<span data-ttu-id="cb335-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb335-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb335-131">id</span><span class="sxs-lookup"><span data-stu-id="cb335-131">id</span></span>|<span data-ttu-id="cb335-132">String</span><span class="sxs-lookup"><span data-stu-id="cb335-132">String</span></span>|<span data-ttu-id="cb335-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="cb335-133">Key of the entity.</span></span> <span data-ttu-id="cb335-134">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cb335-135">displayName</span></span>|<span data-ttu-id="cb335-136">String</span><span class="sxs-lookup"><span data-stu-id="cb335-136">String</span></span>|<span data-ttu-id="cb335-137">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="cb335-137">Name of the eBook.</span></span> <span data-ttu-id="cb335-138">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-139">description</span><span class="sxs-lookup"><span data-stu-id="cb335-139">description</span></span>|<span data-ttu-id="cb335-140">String</span><span class="sxs-lookup"><span data-stu-id="cb335-140">String</span></span>|<span data-ttu-id="cb335-141">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="cb335-141">Description.</span></span> <span data-ttu-id="cb335-142">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-143">publisher</span><span class="sxs-lookup"><span data-stu-id="cb335-143">publisher</span></span>|<span data-ttu-id="cb335-144">String</span><span class="sxs-lookup"><span data-stu-id="cb335-144">String</span></span>|<span data-ttu-id="cb335-145">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="cb335-145">Publisher.</span></span> <span data-ttu-id="cb335-146">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb335-147">publishedDateTime</span></span>|<span data-ttu-id="cb335-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb335-148">DateTimeOffset</span></span>|<span data-ttu-id="cb335-149">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="cb335-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="cb335-150">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="cb335-151">largeCover</span></span>|[<span data-ttu-id="cb335-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb335-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cb335-153">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="cb335-153">Book cover.</span></span> <span data-ttu-id="cb335-154">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb335-155">createdDateTime</span></span>|<span data-ttu-id="cb335-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb335-156">DateTimeOffset</span></span>|<span data-ttu-id="cb335-157">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="cb335-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="cb335-158">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb335-159">lastModifiedDateTime</span></span>|<span data-ttu-id="cb335-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb335-160">DateTimeOffset</span></span>|<span data-ttu-id="cb335-161">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="cb335-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="cb335-162">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb335-163">informationUrl</span></span>|<span data-ttu-id="cb335-164">String</span><span class="sxs-lookup"><span data-stu-id="cb335-164">String</span></span>|<span data-ttu-id="cb335-165">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="cb335-165">The more information Url.</span></span> <span data-ttu-id="cb335-166">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb335-167">privacyInformationUrl</span></span>|<span data-ttu-id="cb335-168">String</span><span class="sxs-lookup"><span data-stu-id="cb335-168">String</span></span>|<span data-ttu-id="cb335-169">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="cb335-169">The privacy statement Url.</span></span> <span data-ttu-id="cb335-170">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cb335-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cb335-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="cb335-171">vppTokenId</span></span>|<span data-ttu-id="cb335-172">Guid</span><span class="sxs-lookup"><span data-stu-id="cb335-172">Guid</span></span>|<span data-ttu-id="cb335-173">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="cb335-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="cb335-174">appleId</span><span class="sxs-lookup"><span data-stu-id="cb335-174">appleId</span></span>|<span data-ttu-id="cb335-175">String</span><span class="sxs-lookup"><span data-stu-id="cb335-175">String</span></span>|<span data-ttu-id="cb335-176">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="cb335-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="cb335-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="cb335-177">vppOrganizationName</span></span>|<span data-ttu-id="cb335-178">String</span><span class="sxs-lookup"><span data-stu-id="cb335-178">String</span></span>|<span data-ttu-id="cb335-179">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="cb335-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="cb335-180">genres</span><span class="sxs-lookup"><span data-stu-id="cb335-180">genres</span></span>|<span data-ttu-id="cb335-181">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="cb335-181">String collection</span></span>|<span data-ttu-id="cb335-182">Genres</span><span class="sxs-lookup"><span data-stu-id="cb335-182">Genres.</span></span>|
|<span data-ttu-id="cb335-183">language</span><span class="sxs-lookup"><span data-stu-id="cb335-183">language</span></span>|<span data-ttu-id="cb335-184">String</span><span class="sxs-lookup"><span data-stu-id="cb335-184">String</span></span>|<span data-ttu-id="cb335-185">Sprache</span><span class="sxs-lookup"><span data-stu-id="cb335-185">Language.</span></span>|
|<span data-ttu-id="cb335-186">seller</span><span class="sxs-lookup"><span data-stu-id="cb335-186">seller</span></span>|<span data-ttu-id="cb335-187">String</span><span class="sxs-lookup"><span data-stu-id="cb335-187">String</span></span>|<span data-ttu-id="cb335-188">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="cb335-188">Seller.</span></span>|
|<span data-ttu-id="cb335-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cb335-189">totalLicenseCount</span></span>|<span data-ttu-id="cb335-190">Int32</span><span class="sxs-lookup"><span data-stu-id="cb335-190">Int32</span></span>|<span data-ttu-id="cb335-191">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="cb335-191">Total license count.</span></span>|
|<span data-ttu-id="cb335-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cb335-192">usedLicenseCount</span></span>|<span data-ttu-id="cb335-193">Int32</span><span class="sxs-lookup"><span data-stu-id="cb335-193">Int32</span></span>|<span data-ttu-id="cb335-194">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="cb335-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="cb335-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb335-195">Response</span></span>
<span data-ttu-id="cb335-196">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb335-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb335-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb335-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb335-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb335-198">Request</span></span>
<span data-ttu-id="cb335-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb335-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
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

### <a name="response"></a><span data-ttu-id="cb335-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb335-200">Response</span></span>
<span data-ttu-id="cb335-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb335-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



