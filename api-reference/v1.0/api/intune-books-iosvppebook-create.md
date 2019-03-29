---
title: iosVppEBook erstellen
description: Erstellt neue Objekte des Typs iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6251e3ecda1597653ff2fed9575e7357e89f652f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965060"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="c80ce-103">iosVppEBook erstellen</span><span class="sxs-lookup"><span data-stu-id="c80ce-103">Create iosVppEBook</span></span>

> <span data-ttu-id="c80ce-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c80ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c80ce-105">Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c80ce-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c80ce-106">Prerequisites</span></span>
<span data-ttu-id="c80ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c80ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c80ce-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c80ce-109">Permission type</span></span>|<span data-ttu-id="c80ce-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c80ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c80ce-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c80ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c80ce-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c80ce-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c80ce-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c80ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c80ce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c80ce-114">Not supported.</span></span>|
|<span data-ttu-id="c80ce-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c80ce-115">Application</span></span>|<span data-ttu-id="c80ce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c80ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c80ce-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c80ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="c80ce-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c80ce-118">Request headers</span></span>
|<span data-ttu-id="c80ce-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c80ce-119">Header</span></span>|<span data-ttu-id="c80ce-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c80ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c80ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c80ce-121">Authorization</span></span>|<span data-ttu-id="c80ce-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c80ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c80ce-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c80ce-123">Accept</span></span>|<span data-ttu-id="c80ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c80ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c80ce-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c80ce-125">Request body</span></span>
<span data-ttu-id="c80ce-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppEBook-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c80ce-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="c80ce-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosVppEBook erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c80ce-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="c80ce-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c80ce-128">Property</span></span>|<span data-ttu-id="c80ce-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c80ce-129">Type</span></span>|<span data-ttu-id="c80ce-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c80ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c80ce-131">id</span><span class="sxs-lookup"><span data-stu-id="c80ce-131">id</span></span>|<span data-ttu-id="c80ce-132">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-132">String</span></span>|<span data-ttu-id="c80ce-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c80ce-133">Key of the entity.</span></span> <span data-ttu-id="c80ce-134">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c80ce-135">displayName</span></span>|<span data-ttu-id="c80ce-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c80ce-136">String</span></span>|<span data-ttu-id="c80ce-137">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c80ce-137">Name of the eBook.</span></span> <span data-ttu-id="c80ce-138">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-139">description</span><span class="sxs-lookup"><span data-stu-id="c80ce-139">description</span></span>|<span data-ttu-id="c80ce-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c80ce-140">String</span></span>|<span data-ttu-id="c80ce-141">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="c80ce-141">Description.</span></span> <span data-ttu-id="c80ce-142">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-143">publisher</span><span class="sxs-lookup"><span data-stu-id="c80ce-143">publisher</span></span>|<span data-ttu-id="c80ce-144">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-144">String</span></span>|<span data-ttu-id="c80ce-145">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="c80ce-145">Publisher.</span></span> <span data-ttu-id="c80ce-146">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c80ce-147">publishedDateTime</span></span>|<span data-ttu-id="c80ce-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c80ce-148">DateTimeOffset</span></span>|<span data-ttu-id="c80ce-149">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c80ce-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="c80ce-150">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="c80ce-151">largeCover</span></span>|[<span data-ttu-id="c80ce-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c80ce-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c80ce-153">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="c80ce-153">Book cover.</span></span> <span data-ttu-id="c80ce-154">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c80ce-155">createdDateTime</span></span>|<span data-ttu-id="c80ce-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c80ce-156">DateTimeOffset</span></span>|<span data-ttu-id="c80ce-157">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="c80ce-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="c80ce-158">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c80ce-159">lastModifiedDateTime</span></span>|<span data-ttu-id="c80ce-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c80ce-160">DateTimeOffset</span></span>|<span data-ttu-id="c80ce-161">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c80ce-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="c80ce-162">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c80ce-163">informationUrl</span></span>|<span data-ttu-id="c80ce-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c80ce-164">String</span></span>|<span data-ttu-id="c80ce-165">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c80ce-165">The more information Url.</span></span> <span data-ttu-id="c80ce-166">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c80ce-167">privacyInformationUrl</span></span>|<span data-ttu-id="c80ce-168">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-168">String</span></span>|<span data-ttu-id="c80ce-169">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c80ce-169">The privacy statement Url.</span></span> <span data-ttu-id="c80ce-170">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c80ce-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c80ce-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="c80ce-171">vppTokenId</span></span>|<span data-ttu-id="c80ce-172">Guid</span><span class="sxs-lookup"><span data-stu-id="c80ce-172">Guid</span></span>|<span data-ttu-id="c80ce-173">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="c80ce-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="c80ce-174">appleId</span><span class="sxs-lookup"><span data-stu-id="c80ce-174">appleId</span></span>|<span data-ttu-id="c80ce-175">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-175">String</span></span>|<span data-ttu-id="c80ce-176">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c80ce-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="c80ce-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="c80ce-177">vppOrganizationName</span></span>|<span data-ttu-id="c80ce-178">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-178">String</span></span>|<span data-ttu-id="c80ce-179">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="c80ce-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="c80ce-180">genres</span><span class="sxs-lookup"><span data-stu-id="c80ce-180">genres</span></span>|<span data-ttu-id="c80ce-181">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c80ce-181">String collection</span></span>|<span data-ttu-id="c80ce-182">Genres</span><span class="sxs-lookup"><span data-stu-id="c80ce-182">Genres.</span></span>|
|<span data-ttu-id="c80ce-183">language</span><span class="sxs-lookup"><span data-stu-id="c80ce-183">language</span></span>|<span data-ttu-id="c80ce-184">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-184">String</span></span>|<span data-ttu-id="c80ce-185">Sprache</span><span class="sxs-lookup"><span data-stu-id="c80ce-185">Language.</span></span>|
|<span data-ttu-id="c80ce-186">seller</span><span class="sxs-lookup"><span data-stu-id="c80ce-186">seller</span></span>|<span data-ttu-id="c80ce-187">String</span><span class="sxs-lookup"><span data-stu-id="c80ce-187">String</span></span>|<span data-ttu-id="c80ce-188">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="c80ce-188">Seller.</span></span>|
|<span data-ttu-id="c80ce-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c80ce-189">totalLicenseCount</span></span>|<span data-ttu-id="c80ce-190">Int32</span><span class="sxs-lookup"><span data-stu-id="c80ce-190">Int32</span></span>|<span data-ttu-id="c80ce-191">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="c80ce-191">Total license count.</span></span>|
|<span data-ttu-id="c80ce-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c80ce-192">usedLicenseCount</span></span>|<span data-ttu-id="c80ce-193">Int32</span><span class="sxs-lookup"><span data-stu-id="c80ce-193">Int32</span></span>|<span data-ttu-id="c80ce-194">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="c80ce-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="c80ce-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="c80ce-195">Response</span></span>
<span data-ttu-id="c80ce-196">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c80ce-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c80ce-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c80ce-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="c80ce-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c80ce-198">Request</span></span>
<span data-ttu-id="c80ce-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c80ce-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c80ce-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="c80ce-200">Response</span></span>
<span data-ttu-id="c80ce-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c80ce-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



