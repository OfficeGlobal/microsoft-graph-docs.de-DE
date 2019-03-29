---
title: Erstellen von „macOSOfficeSuiteApp“
description: Diese Methode erstellt ein neues Objekt des Typs macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4da48d554a5d92fb387290b515e60eb3c719677c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960720"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="f5309-103">Erstellen von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="f5309-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="f5309-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5309-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5309-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f5309-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5309-106">Diese Methode erstellt ein neues Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5309-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f5309-107">Prerequisites</span></span>
<span data-ttu-id="f5309-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5309-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5309-110">Permission type</span></span>|<span data-ttu-id="f5309-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5309-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5309-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5309-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5309-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5309-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f5309-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5309-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5309-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5309-115">Not supported.</span></span>|
|<span data-ttu-id="f5309-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5309-116">Application</span></span>|<span data-ttu-id="f5309-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5309-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5309-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5309-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f5309-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5309-119">Request headers</span></span>
|<span data-ttu-id="f5309-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f5309-120">Header</span></span>|<span data-ttu-id="f5309-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f5309-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5309-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5309-122">Authorization</span></span>|<span data-ttu-id="f5309-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f5309-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5309-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f5309-124">Accept</span></span>|<span data-ttu-id="f5309-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5309-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5309-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5309-126">Request body</span></span>
<span data-ttu-id="f5309-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „macOSOfficeSuiteApp“ an.</span><span class="sxs-lookup"><span data-stu-id="f5309-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="f5309-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSOfficeSuiteApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="f5309-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="f5309-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f5309-129">Property</span></span>|<span data-ttu-id="f5309-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f5309-130">Type</span></span>|<span data-ttu-id="f5309-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5309-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5309-132">id</span><span class="sxs-lookup"><span data-stu-id="f5309-132">id</span></span>|<span data-ttu-id="f5309-133">String</span><span class="sxs-lookup"><span data-stu-id="f5309-133">String</span></span>|<span data-ttu-id="f5309-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f5309-134">Key of the entity.</span></span> <span data-ttu-id="f5309-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f5309-136">displayName</span></span>|<span data-ttu-id="f5309-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5309-137">String</span></span>|<span data-ttu-id="f5309-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f5309-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-140">description</span><span class="sxs-lookup"><span data-stu-id="f5309-140">description</span></span>|<span data-ttu-id="f5309-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5309-141">String</span></span>|<span data-ttu-id="f5309-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-142">The description of the app.</span></span> <span data-ttu-id="f5309-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f5309-144">publisher</span></span>|<span data-ttu-id="f5309-145">String</span><span class="sxs-lookup"><span data-stu-id="f5309-145">String</span></span>|<span data-ttu-id="f5309-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-146">The publisher of the app.</span></span> <span data-ttu-id="f5309-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f5309-148">largeIcon</span></span>|[<span data-ttu-id="f5309-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f5309-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f5309-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f5309-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f5309-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5309-152">createdDateTime</span></span>|<span data-ttu-id="f5309-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5309-153">DateTimeOffset</span></span>|<span data-ttu-id="f5309-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-154">The date and time the app was created.</span></span> <span data-ttu-id="f5309-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5309-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f5309-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5309-157">DateTimeOffset</span></span>|<span data-ttu-id="f5309-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f5309-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f5309-160">isFeatured</span></span>|<span data-ttu-id="f5309-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5309-161">Boolean</span></span>|<span data-ttu-id="f5309-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f5309-163">privacyInformationUrl</span></span>|<span data-ttu-id="f5309-164">String</span><span class="sxs-lookup"><span data-stu-id="f5309-164">String</span></span>|<span data-ttu-id="f5309-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="f5309-165">The privacy statement Url.</span></span> <span data-ttu-id="f5309-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f5309-167">informationUrl</span></span>|<span data-ttu-id="f5309-168">String</span><span class="sxs-lookup"><span data-stu-id="f5309-168">String</span></span>|<span data-ttu-id="f5309-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="f5309-169">The more information Url.</span></span> <span data-ttu-id="f5309-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-171">owner</span><span class="sxs-lookup"><span data-stu-id="f5309-171">owner</span></span>|<span data-ttu-id="f5309-172">String</span><span class="sxs-lookup"><span data-stu-id="f5309-172">String</span></span>|<span data-ttu-id="f5309-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-173">The owner of the app.</span></span> <span data-ttu-id="f5309-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-175">developer</span><span class="sxs-lookup"><span data-stu-id="f5309-175">developer</span></span>|<span data-ttu-id="f5309-176">String</span><span class="sxs-lookup"><span data-stu-id="f5309-176">String</span></span>|<span data-ttu-id="f5309-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="f5309-177">The developer of the app.</span></span> <span data-ttu-id="f5309-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-179">notes</span><span class="sxs-lookup"><span data-stu-id="f5309-179">notes</span></span>|<span data-ttu-id="f5309-180">String</span><span class="sxs-lookup"><span data-stu-id="f5309-180">String</span></span>|<span data-ttu-id="f5309-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="f5309-181">Notes for the app.</span></span> <span data-ttu-id="f5309-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f5309-183">uploadState</span></span>|<span data-ttu-id="f5309-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f5309-184">Int32</span></span>|<span data-ttu-id="f5309-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="f5309-185">The upload state.</span></span> <span data-ttu-id="f5309-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f5309-187">publishingState</span></span>|[<span data-ttu-id="f5309-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f5309-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f5309-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="f5309-189">The publishing state for the app.</span></span> <span data-ttu-id="f5309-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="f5309-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f5309-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="f5309-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f5309-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="f5309-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f5309-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f5309-193">isAssigned</span></span>|<span data-ttu-id="f5309-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5309-194">Boolean</span></span>|<span data-ttu-id="f5309-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="f5309-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f5309-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f5309-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="f5309-197">roleScopeTagIds</span></span>|<span data-ttu-id="f5309-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f5309-198">String collection</span></span>|<span data-ttu-id="f5309-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="f5309-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f5309-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f5309-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f5309-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5309-201">Response</span></span>
<span data-ttu-id="f5309-202">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f5309-202">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5309-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5309-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5309-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5309-204">Request</span></span>
<span data-ttu-id="f5309-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5309-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5309-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5309-206">Response</span></span>
<span data-ttu-id="f5309-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5309-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




