---
title: iosVppEBook erstellen
description: Erstellt neue Objekte des Typs iosVppEBook.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 121f686e5709bcfe59ffab7151afcb9e5f48c127
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409755"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="c5d38-103">iosVppEBook erstellen</span><span class="sxs-lookup"><span data-stu-id="c5d38-103">Create iosVppEBook</span></span>

> <span data-ttu-id="c5d38-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c5d38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5d38-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5d38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5d38-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5d38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5d38-107">Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5d38-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5d38-108">Prerequisites</span></span>
<span data-ttu-id="c5d38-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5d38-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5d38-111">Permission type</span></span>|<span data-ttu-id="c5d38-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5d38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5d38-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5d38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5d38-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d38-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5d38-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5d38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5d38-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5d38-116">Not supported.</span></span>|
|<span data-ttu-id="c5d38-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5d38-117">Application</span></span>|<span data-ttu-id="c5d38-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5d38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5d38-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5d38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="c5d38-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5d38-120">Request headers</span></span>
|<span data-ttu-id="c5d38-121">Header</span><span class="sxs-lookup"><span data-stu-id="c5d38-121">Header</span></span>|<span data-ttu-id="c5d38-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c5d38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5d38-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c5d38-123">Authorization</span></span>|<span data-ttu-id="c5d38-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5d38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5d38-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5d38-125">Accept</span></span>|<span data-ttu-id="c5d38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d38-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5d38-127">Request body</span></span>
<span data-ttu-id="c5d38-128">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppEBook-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c5d38-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="c5d38-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosVppEBook erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c5d38-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="c5d38-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5d38-130">Property</span></span>|<span data-ttu-id="c5d38-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c5d38-131">Type</span></span>|<span data-ttu-id="c5d38-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5d38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d38-133">id</span><span class="sxs-lookup"><span data-stu-id="c5d38-133">id</span></span>|<span data-ttu-id="c5d38-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-134">String</span></span>|<span data-ttu-id="c5d38-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c5d38-135">Key of the entity.</span></span> <span data-ttu-id="c5d38-136">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d38-137">displayName</span></span>|<span data-ttu-id="c5d38-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-138">String</span></span>|<span data-ttu-id="c5d38-139">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c5d38-139">Name of the eBook.</span></span> <span data-ttu-id="c5d38-140">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-141">description</span><span class="sxs-lookup"><span data-stu-id="c5d38-141">description</span></span>|<span data-ttu-id="c5d38-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-142">String</span></span>|<span data-ttu-id="c5d38-143">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="c5d38-143">Description.</span></span> <span data-ttu-id="c5d38-144">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c5d38-145">publisher</span></span>|<span data-ttu-id="c5d38-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-146">String</span></span>|<span data-ttu-id="c5d38-147">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="c5d38-147">Publisher.</span></span> <span data-ttu-id="c5d38-148">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5d38-149">publishedDateTime</span></span>|<span data-ttu-id="c5d38-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5d38-150">DateTimeOffset</span></span>|<span data-ttu-id="c5d38-151">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c5d38-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="c5d38-152">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="c5d38-153">largeCover</span></span>|[<span data-ttu-id="c5d38-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c5d38-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c5d38-155">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="c5d38-155">Book cover.</span></span> <span data-ttu-id="c5d38-156">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5d38-157">createdDateTime</span></span>|<span data-ttu-id="c5d38-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5d38-158">DateTimeOffset</span></span>|<span data-ttu-id="c5d38-159">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="c5d38-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="c5d38-160">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5d38-161">lastModifiedDateTime</span></span>|<span data-ttu-id="c5d38-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5d38-162">DateTimeOffset</span></span>|<span data-ttu-id="c5d38-163">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="c5d38-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="c5d38-164">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c5d38-165">informationUrl</span></span>|<span data-ttu-id="c5d38-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-166">String</span></span>|<span data-ttu-id="c5d38-167">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c5d38-167">The more information Url.</span></span> <span data-ttu-id="c5d38-168">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c5d38-169">privacyInformationUrl</span></span>|<span data-ttu-id="c5d38-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-170">String</span></span>|<span data-ttu-id="c5d38-171">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c5d38-171">The privacy statement Url.</span></span> <span data-ttu-id="c5d38-172">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c5d38-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="c5d38-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="c5d38-173">vppTokenId</span></span>|<span data-ttu-id="c5d38-174">Guid</span><span class="sxs-lookup"><span data-stu-id="c5d38-174">Guid</span></span>|<span data-ttu-id="c5d38-175">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="c5d38-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="c5d38-176">appleId</span><span class="sxs-lookup"><span data-stu-id="c5d38-176">appleId</span></span>|<span data-ttu-id="c5d38-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-177">String</span></span>|<span data-ttu-id="c5d38-178">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c5d38-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="c5d38-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="c5d38-179">vppOrganizationName</span></span>|<span data-ttu-id="c5d38-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-180">String</span></span>|<span data-ttu-id="c5d38-181">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="c5d38-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="c5d38-182">genres</span><span class="sxs-lookup"><span data-stu-id="c5d38-182">genres</span></span>|<span data-ttu-id="c5d38-183">String collection</span><span class="sxs-lookup"><span data-stu-id="c5d38-183">String collection</span></span>|<span data-ttu-id="c5d38-184">Genres</span><span class="sxs-lookup"><span data-stu-id="c5d38-184">Genres.</span></span>|
|<span data-ttu-id="c5d38-185">language</span><span class="sxs-lookup"><span data-stu-id="c5d38-185">language</span></span>|<span data-ttu-id="c5d38-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-186">String</span></span>|<span data-ttu-id="c5d38-187">Sprache</span><span class="sxs-lookup"><span data-stu-id="c5d38-187">Language.</span></span>|
|<span data-ttu-id="c5d38-188">seller</span><span class="sxs-lookup"><span data-stu-id="c5d38-188">seller</span></span>|<span data-ttu-id="c5d38-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5d38-189">String</span></span>|<span data-ttu-id="c5d38-190">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="c5d38-190">Seller.</span></span>|
|<span data-ttu-id="c5d38-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c5d38-191">totalLicenseCount</span></span>|<span data-ttu-id="c5d38-192">Int32</span><span class="sxs-lookup"><span data-stu-id="c5d38-192">Int32</span></span>|<span data-ttu-id="c5d38-193">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="c5d38-193">Total license count.</span></span>|
|<span data-ttu-id="c5d38-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c5d38-194">usedLicenseCount</span></span>|<span data-ttu-id="c5d38-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c5d38-195">Int32</span></span>|<span data-ttu-id="c5d38-196">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="c5d38-196">Used license count.</span></span>|
|<span data-ttu-id="c5d38-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5d38-197">roleScopeTagIds</span></span>|<span data-ttu-id="c5d38-198">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c5d38-198">String collection</span></span>|<span data-ttu-id="c5d38-199">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c5d38-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c5d38-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5d38-200">Response</span></span>
<span data-ttu-id="c5d38-201">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5d38-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d38-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5d38-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5d38-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5d38-203">Request</span></span>
<span data-ttu-id="c5d38-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5d38-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5d38-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5d38-205">Response</span></span>
<span data-ttu-id="c5d38-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5d38-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




