---
title: iosVppEBook erstellen
description: Erstellt neue Objekte des Typs iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf780e1bc3bcb15392a6f2a1b164ef3c94ab1cc2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165219"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="c8d63-103">iosVppEBook erstellen</span><span class="sxs-lookup"><span data-stu-id="c8d63-103">Create iosVppEBook</span></span>

> <span data-ttu-id="c8d63-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8d63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8d63-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c8d63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8d63-106">Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-106">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8d63-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8d63-107">Prerequisites</span></span>
<span data-ttu-id="c8d63-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8d63-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8d63-110">Permission type</span></span>|<span data-ttu-id="c8d63-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8d63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8d63-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8d63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8d63-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d63-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8d63-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8d63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8d63-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8d63-115">Not supported.</span></span>|
|<span data-ttu-id="c8d63-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8d63-116">Application</span></span>|<span data-ttu-id="c8d63-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8d63-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8d63-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8d63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="c8d63-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8d63-119">Request headers</span></span>
|<span data-ttu-id="c8d63-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c8d63-120">Header</span></span>|<span data-ttu-id="c8d63-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c8d63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8d63-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8d63-122">Authorization</span></span>|<span data-ttu-id="c8d63-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8d63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8d63-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8d63-124">Accept</span></span>|<span data-ttu-id="c8d63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8d63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8d63-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8d63-126">Request body</span></span>
<span data-ttu-id="c8d63-127">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppEBook-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c8d63-127">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="c8d63-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosVppEBook erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c8d63-128">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="c8d63-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8d63-129">Property</span></span>|<span data-ttu-id="c8d63-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c8d63-130">Type</span></span>|<span data-ttu-id="c8d63-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8d63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8d63-132">id</span><span class="sxs-lookup"><span data-stu-id="c8d63-132">id</span></span>|<span data-ttu-id="c8d63-133">string</span><span class="sxs-lookup"><span data-stu-id="c8d63-133">String</span></span>|<span data-ttu-id="c8d63-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c8d63-134">Key of the entity.</span></span> <span data-ttu-id="c8d63-135">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c8d63-136">displayName</span></span>|<span data-ttu-id="c8d63-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-137">String</span></span>|<span data-ttu-id="c8d63-138">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c8d63-138">Name of the eBook.</span></span> <span data-ttu-id="c8d63-139">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-140">description</span><span class="sxs-lookup"><span data-stu-id="c8d63-140">description</span></span>|<span data-ttu-id="c8d63-141">String</span><span class="sxs-lookup"><span data-stu-id="c8d63-141">String</span></span>|<span data-ttu-id="c8d63-142">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="c8d63-142">Description.</span></span> <span data-ttu-id="c8d63-143">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c8d63-144">publisher</span></span>|<span data-ttu-id="c8d63-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-145">String</span></span>|<span data-ttu-id="c8d63-146">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="c8d63-146">Publisher.</span></span> <span data-ttu-id="c8d63-147">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8d63-148">publishedDateTime</span></span>|<span data-ttu-id="c8d63-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8d63-149">DateTimeOffset</span></span>|<span data-ttu-id="c8d63-150">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c8d63-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="c8d63-151">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="c8d63-152">largeCover</span></span>|[<span data-ttu-id="c8d63-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c8d63-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c8d63-154">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="c8d63-154">Book cover.</span></span> <span data-ttu-id="c8d63-155">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8d63-156">createdDateTime</span></span>|<span data-ttu-id="c8d63-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8d63-157">DateTimeOffset</span></span>|<span data-ttu-id="c8d63-158">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="c8d63-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="c8d63-159">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8d63-160">lastModifiedDateTime</span></span>|<span data-ttu-id="c8d63-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8d63-161">DateTimeOffset</span></span>|<span data-ttu-id="c8d63-162">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c8d63-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="c8d63-163">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c8d63-164">informationUrl</span></span>|<span data-ttu-id="c8d63-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-165">String</span></span>|<span data-ttu-id="c8d63-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c8d63-166">The more information Url.</span></span> <span data-ttu-id="c8d63-167">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c8d63-168">privacyInformationUrl</span></span>|<span data-ttu-id="c8d63-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-169">String</span></span>|<span data-ttu-id="c8d63-170">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c8d63-170">The privacy statement Url.</span></span> <span data-ttu-id="c8d63-171">Der Wert wird geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c8d63-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c8d63-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="c8d63-172">vppTokenId</span></span>|<span data-ttu-id="c8d63-173">Guid</span><span class="sxs-lookup"><span data-stu-id="c8d63-173">Guid</span></span>|<span data-ttu-id="c8d63-174">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="c8d63-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="c8d63-175">appleId</span><span class="sxs-lookup"><span data-stu-id="c8d63-175">appleId</span></span>|<span data-ttu-id="c8d63-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-176">String</span></span>|<span data-ttu-id="c8d63-177">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c8d63-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="c8d63-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="c8d63-178">vppOrganizationName</span></span>|<span data-ttu-id="c8d63-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-179">String</span></span>|<span data-ttu-id="c8d63-180">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="c8d63-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="c8d63-181">genres</span><span class="sxs-lookup"><span data-stu-id="c8d63-181">genres</span></span>|<span data-ttu-id="c8d63-182">String collection</span><span class="sxs-lookup"><span data-stu-id="c8d63-182">String collection</span></span>|<span data-ttu-id="c8d63-183">Genres</span><span class="sxs-lookup"><span data-stu-id="c8d63-183">Genres.</span></span>|
|<span data-ttu-id="c8d63-184">language</span><span class="sxs-lookup"><span data-stu-id="c8d63-184">language</span></span>|<span data-ttu-id="c8d63-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-185">String</span></span>|<span data-ttu-id="c8d63-186">Sprache</span><span class="sxs-lookup"><span data-stu-id="c8d63-186">Language.</span></span>|
|<span data-ttu-id="c8d63-187">seller</span><span class="sxs-lookup"><span data-stu-id="c8d63-187">seller</span></span>|<span data-ttu-id="c8d63-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d63-188">String</span></span>|<span data-ttu-id="c8d63-189">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="c8d63-189">Seller.</span></span>|
|<span data-ttu-id="c8d63-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c8d63-190">totalLicenseCount</span></span>|<span data-ttu-id="c8d63-191">Int32</span><span class="sxs-lookup"><span data-stu-id="c8d63-191">Int32</span></span>|<span data-ttu-id="c8d63-192">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="c8d63-192">Total license count.</span></span>|
|<span data-ttu-id="c8d63-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c8d63-193">usedLicenseCount</span></span>|<span data-ttu-id="c8d63-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c8d63-194">Int32</span></span>|<span data-ttu-id="c8d63-195">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="c8d63-195">Used license count.</span></span>|
|<span data-ttu-id="c8d63-196">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c8d63-196">roleScopeTagIds</span></span>|<span data-ttu-id="c8d63-197">String collection</span><span class="sxs-lookup"><span data-stu-id="c8d63-197">String collection</span></span>|<span data-ttu-id="c8d63-198">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c8d63-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c8d63-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8d63-199">Response</span></span>
<span data-ttu-id="c8d63-200">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8d63-200">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8d63-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8d63-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8d63-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8d63-202">Request</span></span>
<span data-ttu-id="c8d63-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8d63-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 854

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c8d63-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8d63-204">Response</span></span>
<span data-ttu-id="c8d63-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8d63-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




