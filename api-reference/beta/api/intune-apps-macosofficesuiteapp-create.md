---
title: Erstellen von „macOSOfficeSuiteApp“
description: Diese Methode erstellt ein neues Objekt des Typs macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6712f23e27793356e5305444bc8996441beaf56
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140852"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="ee190-103">Erstellen von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="ee190-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="ee190-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee190-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee190-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ee190-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee190-106">Diese Methode erstellt ein neues Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee190-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ee190-107">Prerequisites</span></span>
<span data-ttu-id="ee190-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee190-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee190-110">Permission type</span></span>|<span data-ttu-id="ee190-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee190-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee190-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee190-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee190-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee190-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee190-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee190-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee190-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee190-115">Not supported.</span></span>|
|<span data-ttu-id="ee190-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee190-116">Application</span></span>|<span data-ttu-id="ee190-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee190-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee190-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee190-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ee190-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee190-119">Request headers</span></span>
|<span data-ttu-id="ee190-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ee190-120">Header</span></span>|<span data-ttu-id="ee190-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ee190-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee190-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee190-122">Authorization</span></span>|<span data-ttu-id="ee190-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ee190-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee190-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ee190-124">Accept</span></span>|<span data-ttu-id="ee190-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee190-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee190-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee190-126">Request body</span></span>
<span data-ttu-id="ee190-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „macOSOfficeSuiteApp“ an.</span><span class="sxs-lookup"><span data-stu-id="ee190-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="ee190-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSOfficeSuiteApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ee190-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="ee190-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee190-129">Property</span></span>|<span data-ttu-id="ee190-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ee190-130">Type</span></span>|<span data-ttu-id="ee190-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee190-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee190-132">id</span><span class="sxs-lookup"><span data-stu-id="ee190-132">id</span></span>|<span data-ttu-id="ee190-133">string</span><span class="sxs-lookup"><span data-stu-id="ee190-133">String</span></span>|<span data-ttu-id="ee190-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ee190-134">Key of the entity.</span></span> <span data-ttu-id="ee190-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ee190-136">displayName</span></span>|<span data-ttu-id="ee190-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee190-137">String</span></span>|<span data-ttu-id="ee190-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ee190-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-140">description</span><span class="sxs-lookup"><span data-stu-id="ee190-140">description</span></span>|<span data-ttu-id="ee190-141">String</span><span class="sxs-lookup"><span data-stu-id="ee190-141">String</span></span>|<span data-ttu-id="ee190-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-142">The description of the app.</span></span> <span data-ttu-id="ee190-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-144">publisher</span><span class="sxs-lookup"><span data-stu-id="ee190-144">publisher</span></span>|<span data-ttu-id="ee190-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee190-145">String</span></span>|<span data-ttu-id="ee190-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-146">The publisher of the app.</span></span> <span data-ttu-id="ee190-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ee190-148">largeIcon</span></span>|[<span data-ttu-id="ee190-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ee190-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ee190-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ee190-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ee190-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee190-152">createdDateTime</span></span>|<span data-ttu-id="ee190-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee190-153">DateTimeOffset</span></span>|<span data-ttu-id="ee190-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-154">The date and time the app was created.</span></span> <span data-ttu-id="ee190-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee190-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ee190-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee190-157">DateTimeOffset</span></span>|<span data-ttu-id="ee190-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ee190-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ee190-160">isFeatured</span></span>|<span data-ttu-id="ee190-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee190-161">Boolean</span></span>|<span data-ttu-id="ee190-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ee190-163">privacyInformationUrl</span></span>|<span data-ttu-id="ee190-164">String</span><span class="sxs-lookup"><span data-stu-id="ee190-164">String</span></span>|<span data-ttu-id="ee190-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="ee190-165">The privacy statement Url.</span></span> <span data-ttu-id="ee190-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ee190-167">informationUrl</span></span>|<span data-ttu-id="ee190-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee190-168">String</span></span>|<span data-ttu-id="ee190-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="ee190-169">The more information Url.</span></span> <span data-ttu-id="ee190-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-171">owner</span><span class="sxs-lookup"><span data-stu-id="ee190-171">owner</span></span>|<span data-ttu-id="ee190-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee190-172">String</span></span>|<span data-ttu-id="ee190-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-173">The owner of the app.</span></span> <span data-ttu-id="ee190-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-175">developer</span><span class="sxs-lookup"><span data-stu-id="ee190-175">developer</span></span>|<span data-ttu-id="ee190-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee190-176">String</span></span>|<span data-ttu-id="ee190-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-177">The developer of the app.</span></span> <span data-ttu-id="ee190-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-179">notes</span><span class="sxs-lookup"><span data-stu-id="ee190-179">notes</span></span>|<span data-ttu-id="ee190-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee190-180">String</span></span>|<span data-ttu-id="ee190-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="ee190-181">Notes for the app.</span></span> <span data-ttu-id="ee190-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="ee190-183">uploadState</span></span>|<span data-ttu-id="ee190-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ee190-184">Int32</span></span>|<span data-ttu-id="ee190-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="ee190-185">The upload state.</span></span> <span data-ttu-id="ee190-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="ee190-187">publishingState</span></span>|[<span data-ttu-id="ee190-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ee190-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ee190-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="ee190-189">The publishing state for the app.</span></span> <span data-ttu-id="ee190-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="ee190-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ee190-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="ee190-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ee190-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="ee190-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ee190-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ee190-193">isAssigned</span></span>|<span data-ttu-id="ee190-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee190-194">Boolean</span></span>|<span data-ttu-id="ee190-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="ee190-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ee190-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ee190-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ee190-197">roleScopeTagIds</span></span>|<span data-ttu-id="ee190-198">String collection</span><span class="sxs-lookup"><span data-stu-id="ee190-198">String collection</span></span>|<span data-ttu-id="ee190-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="ee190-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ee190-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee190-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ee190-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee190-201">Response</span></span>
<span data-ttu-id="ee190-202">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ee190-202">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee190-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee190-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee190-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee190-204">Request</span></span>
<span data-ttu-id="ee190-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee190-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 691

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ee190-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee190-206">Response</span></span>
<span data-ttu-id="ee190-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee190-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




