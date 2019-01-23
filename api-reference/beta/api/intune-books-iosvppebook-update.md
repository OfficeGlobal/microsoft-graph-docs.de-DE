---
title: Aktualisieren von „iosVppEBook“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBook.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7279b8da1ffe159dba56f4a5a10345243703da1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393746"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="3a6b2-103">Aktualisieren von „iosVppEBook“</span><span class="sxs-lookup"><span data-stu-id="3a6b2-103">Update iosVppEBook</span></span>

> <span data-ttu-id="3a6b2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a6b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a6b2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a6b2-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a6b2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3a6b2-108">Prerequisites</span></span>
<span data-ttu-id="3a6b2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a6b2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a6b2-111">Permission type</span></span>|<span data-ttu-id="3a6b2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a6b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a6b2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a6b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a6b2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a6b2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a6b2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a6b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a6b2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a6b2-116">Not supported.</span></span>|
|<span data-ttu-id="3a6b2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a6b2-117">Application</span></span>|<span data-ttu-id="3a6b2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a6b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a6b2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a6b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="3a6b2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a6b2-120">Request headers</span></span>
|<span data-ttu-id="3a6b2-121">Header</span><span class="sxs-lookup"><span data-stu-id="3a6b2-121">Header</span></span>|<span data-ttu-id="3a6b2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3a6b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a6b2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3a6b2-123">Authorization</span></span>|<span data-ttu-id="3a6b2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3a6b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a6b2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3a6b2-125">Accept</span></span>|<span data-ttu-id="3a6b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a6b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a6b2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a6b2-127">Request body</span></span>
<span data-ttu-id="3a6b2-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) an.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="3a6b2-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="3a6b2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a6b2-130">Property</span></span>|<span data-ttu-id="3a6b2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3a6b2-131">Type</span></span>|<span data-ttu-id="3a6b2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a6b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a6b2-133">id</span><span class="sxs-lookup"><span data-stu-id="3a6b2-133">id</span></span>|<span data-ttu-id="3a6b2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-134">String</span></span>|<span data-ttu-id="3a6b2-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-135">Key of the entity.</span></span> <span data-ttu-id="3a6b2-136">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3a6b2-137">displayName</span></span>|<span data-ttu-id="3a6b2-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-138">String</span></span>|<span data-ttu-id="3a6b2-139">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-139">Name of the eBook.</span></span> <span data-ttu-id="3a6b2-140">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-141">description</span><span class="sxs-lookup"><span data-stu-id="3a6b2-141">description</span></span>|<span data-ttu-id="3a6b2-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-142">String</span></span>|<span data-ttu-id="3a6b2-143">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-143">Description.</span></span> <span data-ttu-id="3a6b2-144">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3a6b2-145">publisher</span></span>|<span data-ttu-id="3a6b2-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-146">String</span></span>|<span data-ttu-id="3a6b2-147">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-147">Publisher.</span></span> <span data-ttu-id="3a6b2-148">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a6b2-149">publishedDateTime</span></span>|<span data-ttu-id="3a6b2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a6b2-150">DateTimeOffset</span></span>|<span data-ttu-id="3a6b2-151">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="3a6b2-152">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="3a6b2-153">largeCover</span></span>|[<span data-ttu-id="3a6b2-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3a6b2-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3a6b2-155">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-155">Book cover.</span></span> <span data-ttu-id="3a6b2-156">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a6b2-157">createdDateTime</span></span>|<span data-ttu-id="3a6b2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a6b2-158">DateTimeOffset</span></span>|<span data-ttu-id="3a6b2-159">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="3a6b2-160">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a6b2-161">lastModifiedDateTime</span></span>|<span data-ttu-id="3a6b2-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a6b2-162">DateTimeOffset</span></span>|<span data-ttu-id="3a6b2-163">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="3a6b2-164">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3a6b2-165">informationUrl</span></span>|<span data-ttu-id="3a6b2-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-166">String</span></span>|<span data-ttu-id="3a6b2-167">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-167">The more information Url.</span></span> <span data-ttu-id="3a6b2-168">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3a6b2-169">privacyInformationUrl</span></span>|<span data-ttu-id="3a6b2-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-170">String</span></span>|<span data-ttu-id="3a6b2-171">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-171">The privacy statement Url.</span></span> <span data-ttu-id="3a6b2-172">Geerbt von [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3a6b2-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3a6b2-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="3a6b2-173">vppTokenId</span></span>|<span data-ttu-id="3a6b2-174">Guid</span><span class="sxs-lookup"><span data-stu-id="3a6b2-174">Guid</span></span>|<span data-ttu-id="3a6b2-175">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="3a6b2-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="3a6b2-176">appleId</span><span class="sxs-lookup"><span data-stu-id="3a6b2-176">appleId</span></span>|<span data-ttu-id="3a6b2-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-177">String</span></span>|<span data-ttu-id="3a6b2-178">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="3a6b2-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="3a6b2-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3a6b2-179">vppOrganizationName</span></span>|<span data-ttu-id="3a6b2-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-180">String</span></span>|<span data-ttu-id="3a6b2-181">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="3a6b2-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="3a6b2-182">genres</span><span class="sxs-lookup"><span data-stu-id="3a6b2-182">genres</span></span>|<span data-ttu-id="3a6b2-183">String collection</span><span class="sxs-lookup"><span data-stu-id="3a6b2-183">String collection</span></span>|<span data-ttu-id="3a6b2-184">Genres</span><span class="sxs-lookup"><span data-stu-id="3a6b2-184">Genres.</span></span>|
|<span data-ttu-id="3a6b2-185">language</span><span class="sxs-lookup"><span data-stu-id="3a6b2-185">language</span></span>|<span data-ttu-id="3a6b2-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-186">String</span></span>|<span data-ttu-id="3a6b2-187">Sprache</span><span class="sxs-lookup"><span data-stu-id="3a6b2-187">Language.</span></span>|
|<span data-ttu-id="3a6b2-188">seller</span><span class="sxs-lookup"><span data-stu-id="3a6b2-188">seller</span></span>|<span data-ttu-id="3a6b2-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a6b2-189">String</span></span>|<span data-ttu-id="3a6b2-190">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="3a6b2-190">Seller.</span></span>|
|<span data-ttu-id="3a6b2-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3a6b2-191">totalLicenseCount</span></span>|<span data-ttu-id="3a6b2-192">Int32</span><span class="sxs-lookup"><span data-stu-id="3a6b2-192">Int32</span></span>|<span data-ttu-id="3a6b2-193">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="3a6b2-193">Total license count.</span></span>|
|<span data-ttu-id="3a6b2-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3a6b2-194">usedLicenseCount</span></span>|<span data-ttu-id="3a6b2-195">Int32</span><span class="sxs-lookup"><span data-stu-id="3a6b2-195">Int32</span></span>|<span data-ttu-id="3a6b2-196">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="3a6b2-196">Used license count.</span></span>|
|<span data-ttu-id="3a6b2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a6b2-197">roleScopeTagIds</span></span>|<span data-ttu-id="3a6b2-198">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3a6b2-198">String collection</span></span>|<span data-ttu-id="3a6b2-199">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3a6b2-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a6b2-200">Response</span></span>
<span data-ttu-id="3a6b2-201">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-201">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a6b2-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a6b2-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a6b2-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a6b2-203">Request</span></span>
<span data-ttu-id="3a6b2-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="3a6b2-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a6b2-205">Response</span></span>
<span data-ttu-id="3a6b2-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a6b2-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




