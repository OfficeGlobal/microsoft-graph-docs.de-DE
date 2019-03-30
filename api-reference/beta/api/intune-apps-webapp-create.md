---
title: webApp erstellen
description: Erstellen eines neuen webApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c1a326bb09d50100310140bef88998947a9eeee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986166"
---
# <a name="create-webapp"></a><span data-ttu-id="e9857-103">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="e9857-103">Create webApp</span></span>

> <span data-ttu-id="e9857-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9857-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9857-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9857-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9857-106">Erstellen eines neuen [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e9857-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9857-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e9857-107">Prerequisites</span></span>
<span data-ttu-id="e9857-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9857-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e9857-110">Permission type</span></span>|<span data-ttu-id="e9857-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e9857-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9857-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e9857-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9857-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9857-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e9857-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e9857-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9857-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9857-115">Not supported.</span></span>|
|<span data-ttu-id="e9857-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e9857-116">Application</span></span>|<span data-ttu-id="e9857-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9857-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9857-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9857-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e9857-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e9857-119">Request headers</span></span>
|<span data-ttu-id="e9857-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e9857-120">Header</span></span>|<span data-ttu-id="e9857-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e9857-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9857-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9857-122">Authorization</span></span>|<span data-ttu-id="e9857-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e9857-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9857-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e9857-124">Accept</span></span>|<span data-ttu-id="e9857-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9857-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9857-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e9857-126">Request body</span></span>
<span data-ttu-id="e9857-127">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e9857-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="e9857-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e9857-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="e9857-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9857-129">Property</span></span>|<span data-ttu-id="e9857-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e9857-130">Type</span></span>|<span data-ttu-id="e9857-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9857-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9857-132">id</span><span class="sxs-lookup"><span data-stu-id="e9857-132">id</span></span>|<span data-ttu-id="e9857-133">String</span><span class="sxs-lookup"><span data-stu-id="e9857-133">String</span></span>|<span data-ttu-id="e9857-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e9857-134">Key of the entity.</span></span> <span data-ttu-id="e9857-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e9857-136">displayName</span></span>|<span data-ttu-id="e9857-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9857-137">String</span></span>|<span data-ttu-id="e9857-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e9857-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-140">description</span><span class="sxs-lookup"><span data-stu-id="e9857-140">description</span></span>|<span data-ttu-id="e9857-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9857-141">String</span></span>|<span data-ttu-id="e9857-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-142">The description of the app.</span></span> <span data-ttu-id="e9857-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e9857-144">publisher</span></span>|<span data-ttu-id="e9857-145">String</span><span class="sxs-lookup"><span data-stu-id="e9857-145">String</span></span>|<span data-ttu-id="e9857-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-146">The publisher of the app.</span></span> <span data-ttu-id="e9857-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e9857-148">largeIcon</span></span>|[<span data-ttu-id="e9857-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e9857-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e9857-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e9857-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e9857-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9857-152">createdDateTime</span></span>|<span data-ttu-id="e9857-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9857-153">DateTimeOffset</span></span>|<span data-ttu-id="e9857-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-154">The date and time the app was created.</span></span> <span data-ttu-id="e9857-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9857-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e9857-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9857-157">DateTimeOffset</span></span>|<span data-ttu-id="e9857-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e9857-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e9857-160">isFeatured</span></span>|<span data-ttu-id="e9857-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e9857-161">Boolean</span></span>|<span data-ttu-id="e9857-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e9857-163">privacyInformationUrl</span></span>|<span data-ttu-id="e9857-164">String</span><span class="sxs-lookup"><span data-stu-id="e9857-164">String</span></span>|<span data-ttu-id="e9857-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="e9857-165">The privacy statement Url.</span></span> <span data-ttu-id="e9857-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e9857-167">informationUrl</span></span>|<span data-ttu-id="e9857-168">String</span><span class="sxs-lookup"><span data-stu-id="e9857-168">String</span></span>|<span data-ttu-id="e9857-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e9857-169">The more information Url.</span></span> <span data-ttu-id="e9857-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-171">owner</span><span class="sxs-lookup"><span data-stu-id="e9857-171">owner</span></span>|<span data-ttu-id="e9857-172">String</span><span class="sxs-lookup"><span data-stu-id="e9857-172">String</span></span>|<span data-ttu-id="e9857-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-173">The owner of the app.</span></span> <span data-ttu-id="e9857-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-175">developer</span><span class="sxs-lookup"><span data-stu-id="e9857-175">developer</span></span>|<span data-ttu-id="e9857-176">String</span><span class="sxs-lookup"><span data-stu-id="e9857-176">String</span></span>|<span data-ttu-id="e9857-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e9857-177">The developer of the app.</span></span> <span data-ttu-id="e9857-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-179">notes</span><span class="sxs-lookup"><span data-stu-id="e9857-179">notes</span></span>|<span data-ttu-id="e9857-180">String</span><span class="sxs-lookup"><span data-stu-id="e9857-180">String</span></span>|<span data-ttu-id="e9857-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="e9857-181">Notes for the app.</span></span> <span data-ttu-id="e9857-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e9857-183">uploadState</span></span>|<span data-ttu-id="e9857-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e9857-184">Int32</span></span>|<span data-ttu-id="e9857-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="e9857-185">The upload state.</span></span> <span data-ttu-id="e9857-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e9857-187">publishingState</span></span>|[<span data-ttu-id="e9857-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e9857-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e9857-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="e9857-189">The publishing state for the app.</span></span> <span data-ttu-id="e9857-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e9857-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e9857-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e9857-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e9857-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e9857-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e9857-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e9857-193">isAssigned</span></span>|<span data-ttu-id="e9857-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9857-194">Boolean</span></span>|<span data-ttu-id="e9857-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="e9857-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e9857-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="e9857-197">roleScopeTagIds</span></span>|<span data-ttu-id="e9857-198">String collection</span><span class="sxs-lookup"><span data-stu-id="e9857-198">String collection</span></span>|<span data-ttu-id="e9857-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="e9857-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e9857-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e9857-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e9857-201">appUrl</span><span class="sxs-lookup"><span data-stu-id="e9857-201">appUrl</span></span>|<span data-ttu-id="e9857-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9857-202">String</span></span>|<span data-ttu-id="e9857-203">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="e9857-203">The web app URL.</span></span>|
|<span data-ttu-id="e9857-204">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="e9857-204">useManagedBrowser</span></span>|<span data-ttu-id="e9857-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9857-205">Boolean</span></span>|<span data-ttu-id="e9857-206">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e9857-206">Whether or not to use managed browser.</span></span> <span data-ttu-id="e9857-207">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="e9857-207">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="e9857-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9857-208">Response</span></span>
<span data-ttu-id="e9857-209">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e9857-209">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9857-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9857-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9857-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9857-211">Request</span></span>
<span data-ttu-id="e9857-212">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e9857-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 752

{
  "@odata.type": "#microsoft.graph.webApp",
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
  ],
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="e9857-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9857-213">Response</span></span>
<span data-ttu-id="e9857-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e9857-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 924

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  ],
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




