---
title: iosVppEBook erstellen
description: Erstellt neue Objekte des Typs iosVppEBook.
ms.openlocfilehash: 403093fa69cff503022ba6104f27a1f8ccd96849
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064071"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="f3b87-103">iosVppEBook erstellen</span><span class="sxs-lookup"><span data-stu-id="f3b87-103">Create iosVppEBook</span></span>

> <span data-ttu-id="f3b87-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3b87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3b87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3b87-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3b87-107">Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3b87-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3b87-108">Prerequisites</span></span>
<span data-ttu-id="f3b87-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3b87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3b87-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3b87-111">Permission type</span></span>|<span data-ttu-id="f3b87-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3b87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3b87-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3b87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3b87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3b87-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3b87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3b87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3b87-116">Not supported.</span></span>|
|<span data-ttu-id="f3b87-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3b87-117">Application</span></span>|<span data-ttu-id="f3b87-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3b87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3b87-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3b87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="f3b87-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3b87-120">Request headers</span></span>
|<span data-ttu-id="f3b87-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3b87-121">Header</span></span>|<span data-ttu-id="f3b87-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f3b87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3b87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3b87-123">Authorization</span></span>|<span data-ttu-id="f3b87-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3b87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3b87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3b87-125">Accept</span></span>|<span data-ttu-id="f3b87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3b87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3b87-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3b87-127">Request body</span></span>
<span data-ttu-id="f3b87-128">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppEBook-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f3b87-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="f3b87-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosVppEBook erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f3b87-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="f3b87-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3b87-130">Property</span></span>|<span data-ttu-id="f3b87-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f3b87-131">Type</span></span>|<span data-ttu-id="f3b87-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3b87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b87-133">id</span><span class="sxs-lookup"><span data-stu-id="f3b87-133">id</span></span>|<span data-ttu-id="f3b87-134">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-134">String</span></span>|<span data-ttu-id="f3b87-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="f3b87-135">Key of the entity.</span></span> <span data-ttu-id="f3b87-136">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f3b87-137">displayName</span></span>|<span data-ttu-id="f3b87-138">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-138">String</span></span>|<span data-ttu-id="f3b87-139">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="f3b87-139">Name of the eBook.</span></span> <span data-ttu-id="f3b87-140">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-141">description</span><span class="sxs-lookup"><span data-stu-id="f3b87-141">description</span></span>|<span data-ttu-id="f3b87-142">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-142">String</span></span>|<span data-ttu-id="f3b87-143">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="f3b87-143">Description.</span></span> <span data-ttu-id="f3b87-144">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f3b87-145">publisher</span></span>|<span data-ttu-id="f3b87-146">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-146">String</span></span>|<span data-ttu-id="f3b87-147">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="f3b87-147">Publisher.</span></span> <span data-ttu-id="f3b87-148">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3b87-149">publishedDateTime</span></span>|<span data-ttu-id="f3b87-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3b87-150">DateTimeOffset</span></span>|<span data-ttu-id="f3b87-151">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="f3b87-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="f3b87-152">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="f3b87-153">largeCover</span></span>|[<span data-ttu-id="f3b87-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3b87-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3b87-155">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="f3b87-155">Book cover.</span></span> <span data-ttu-id="f3b87-156">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3b87-157">createdDateTime</span></span>|<span data-ttu-id="f3b87-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3b87-158">DateTimeOffset</span></span>|<span data-ttu-id="f3b87-159">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="f3b87-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="f3b87-160">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3b87-161">lastModifiedDateTime</span></span>|<span data-ttu-id="f3b87-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3b87-162">DateTimeOffset</span></span>|<span data-ttu-id="f3b87-163">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="f3b87-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="f3b87-164">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3b87-165">informationUrl</span></span>|<span data-ttu-id="f3b87-166">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-166">String</span></span>|<span data-ttu-id="f3b87-167">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="f3b87-167">The more information Url.</span></span> <span data-ttu-id="f3b87-168">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3b87-169">privacyInformationUrl</span></span>|<span data-ttu-id="f3b87-170">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-170">String</span></span>|<span data-ttu-id="f3b87-171">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="f3b87-171">The privacy statement Url.</span></span> <span data-ttu-id="f3b87-172">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f3b87-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3b87-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f3b87-173">vppTokenId</span></span>|<span data-ttu-id="f3b87-174">Guid</span><span class="sxs-lookup"><span data-stu-id="f3b87-174">Guid</span></span>|<span data-ttu-id="f3b87-175">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="f3b87-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="f3b87-176">appleId</span><span class="sxs-lookup"><span data-stu-id="f3b87-176">appleId</span></span>|<span data-ttu-id="f3b87-177">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-177">String</span></span>|<span data-ttu-id="f3b87-178">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="f3b87-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="f3b87-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f3b87-179">vppOrganizationName</span></span>|<span data-ttu-id="f3b87-180">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-180">String</span></span>|<span data-ttu-id="f3b87-181">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="f3b87-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="f3b87-182">genres</span><span class="sxs-lookup"><span data-stu-id="f3b87-182">genres</span></span>|<span data-ttu-id="f3b87-183">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3b87-183">String collection</span></span>|<span data-ttu-id="f3b87-184">Genres</span><span class="sxs-lookup"><span data-stu-id="f3b87-184">Genres.</span></span>|
|<span data-ttu-id="f3b87-185">language</span><span class="sxs-lookup"><span data-stu-id="f3b87-185">language</span></span>|<span data-ttu-id="f3b87-186">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-186">String</span></span>|<span data-ttu-id="f3b87-187">Sprache</span><span class="sxs-lookup"><span data-stu-id="f3b87-187">Language.</span></span>|
|<span data-ttu-id="f3b87-188">seller</span><span class="sxs-lookup"><span data-stu-id="f3b87-188">seller</span></span>|<span data-ttu-id="f3b87-189">String</span><span class="sxs-lookup"><span data-stu-id="f3b87-189">String</span></span>|<span data-ttu-id="f3b87-190">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="f3b87-190">Seller.</span></span>|
|<span data-ttu-id="f3b87-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3b87-191">totalLicenseCount</span></span>|<span data-ttu-id="f3b87-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b87-192">Int32</span></span>|<span data-ttu-id="f3b87-193">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="f3b87-193">Total license count.</span></span>|
|<span data-ttu-id="f3b87-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3b87-194">usedLicenseCount</span></span>|<span data-ttu-id="f3b87-195">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b87-195">Int32</span></span>|<span data-ttu-id="f3b87-196">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="f3b87-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="f3b87-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3b87-197">Response</span></span>
<span data-ttu-id="f3b87-198">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3b87-198">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3b87-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3b87-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3b87-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3b87-200">Request</span></span>
<span data-ttu-id="f3b87-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3b87-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 856

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

### <a name="response"></a><span data-ttu-id="f3b87-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3b87-202">Response</span></span>
<span data-ttu-id="f3b87-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3b87-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





