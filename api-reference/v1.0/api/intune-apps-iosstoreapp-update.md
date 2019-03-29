---
title: iosStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines iosStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4ad218975d5d4b6ac23e294a3321635ff415d69
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979557"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="f6ed1-103">iosStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f6ed1-103">Update iosStoreApp</span></span>

> <span data-ttu-id="f6ed1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6ed1-105">Aktualisieren der Eigenschaften eines [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-105">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6ed1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6ed1-106">Prerequisites</span></span>
<span data-ttu-id="f6ed1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ed1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6ed1-109">Permission type</span></span>|<span data-ttu-id="f6ed1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6ed1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6ed1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6ed1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6ed1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ed1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6ed1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6ed1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6ed1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6ed1-114">Not supported.</span></span>|
|<span data-ttu-id="f6ed1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6ed1-115">Application</span></span>|<span data-ttu-id="f6ed1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6ed1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6ed1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6ed1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f6ed1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6ed1-118">Request headers</span></span>
|<span data-ttu-id="f6ed1-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6ed1-119">Header</span></span>|<span data-ttu-id="f6ed1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f6ed1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6ed1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6ed1-121">Authorization</span></span>|<span data-ttu-id="f6ed1-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6ed1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6ed1-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6ed1-123">Accept</span></span>|<span data-ttu-id="f6ed1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f6ed1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6ed1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6ed1-125">Request body</span></span>
<span data-ttu-id="f6ed1-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-126">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="f6ed1-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosStoreApp](../resources/intune-apps-iosstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-127">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="f6ed1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6ed1-128">Property</span></span>|<span data-ttu-id="f6ed1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f6ed1-129">Type</span></span>|<span data-ttu-id="f6ed1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6ed1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6ed1-131">id</span><span class="sxs-lookup"><span data-stu-id="f6ed1-131">id</span></span>|<span data-ttu-id="f6ed1-132">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-132">String</span></span>|<span data-ttu-id="f6ed1-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f6ed1-133">Key of the entity.</span></span> <span data-ttu-id="f6ed1-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f6ed1-135">displayName</span></span>|<span data-ttu-id="f6ed1-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6ed1-136">String</span></span>|<span data-ttu-id="f6ed1-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f6ed1-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-139">description</span><span class="sxs-lookup"><span data-stu-id="f6ed1-139">description</span></span>|<span data-ttu-id="f6ed1-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6ed1-140">String</span></span>|<span data-ttu-id="f6ed1-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-141">The description of the app.</span></span> <span data-ttu-id="f6ed1-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f6ed1-143">publisher</span></span>|<span data-ttu-id="f6ed1-144">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-144">String</span></span>|<span data-ttu-id="f6ed1-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-145">The publisher of the app.</span></span> <span data-ttu-id="f6ed1-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f6ed1-147">largeIcon</span></span>|[<span data-ttu-id="f6ed1-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f6ed1-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f6ed1-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f6ed1-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ed1-151">createdDateTime</span></span>|<span data-ttu-id="f6ed1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ed1-152">DateTimeOffset</span></span>|<span data-ttu-id="f6ed1-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-153">The date and time the app was created.</span></span> <span data-ttu-id="f6ed1-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ed1-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f6ed1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ed1-156">DateTimeOffset</span></span>|<span data-ttu-id="f6ed1-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f6ed1-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f6ed1-159">isFeatured</span></span>|<span data-ttu-id="f6ed1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6ed1-160">Boolean</span></span>|<span data-ttu-id="f6ed1-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f6ed1-162">privacyInformationUrl</span></span>|<span data-ttu-id="f6ed1-163">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-163">String</span></span>|<span data-ttu-id="f6ed1-164">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="f6ed1-164">The privacy statement Url.</span></span> <span data-ttu-id="f6ed1-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f6ed1-166">informationUrl</span></span>|<span data-ttu-id="f6ed1-167">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-167">String</span></span>|<span data-ttu-id="f6ed1-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-168">The more information Url.</span></span> <span data-ttu-id="f6ed1-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-170">owner</span><span class="sxs-lookup"><span data-stu-id="f6ed1-170">owner</span></span>|<span data-ttu-id="f6ed1-171">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-171">String</span></span>|<span data-ttu-id="f6ed1-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-172">The owner of the app.</span></span> <span data-ttu-id="f6ed1-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-174">developer</span><span class="sxs-lookup"><span data-stu-id="f6ed1-174">developer</span></span>|<span data-ttu-id="f6ed1-175">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-175">String</span></span>|<span data-ttu-id="f6ed1-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-176">The developer of the app.</span></span> <span data-ttu-id="f6ed1-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-178">notes</span><span class="sxs-lookup"><span data-stu-id="f6ed1-178">notes</span></span>|<span data-ttu-id="f6ed1-179">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-179">String</span></span>|<span data-ttu-id="f6ed1-180">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-180">Notes for the app.</span></span> <span data-ttu-id="f6ed1-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ed1-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ed1-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f6ed1-182">publishingState</span></span>|[<span data-ttu-id="f6ed1-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f6ed1-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f6ed1-184">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-184">The publishing state for the app.</span></span> <span data-ttu-id="f6ed1-185">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f6ed1-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f6ed1-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f6ed1-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="f6ed1-188">bundleId</span></span>|<span data-ttu-id="f6ed1-189">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-189">String</span></span>|<span data-ttu-id="f6ed1-190">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="f6ed1-190">The Identity Name.</span></span>|
|<span data-ttu-id="f6ed1-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f6ed1-191">appStoreUrl</span></span>|<span data-ttu-id="f6ed1-192">String</span><span class="sxs-lookup"><span data-stu-id="f6ed1-192">String</span></span>|<span data-ttu-id="f6ed1-193">URL des Apple-App-Stores</span><span class="sxs-lookup"><span data-stu-id="f6ed1-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="f6ed1-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f6ed1-194">applicableDeviceType</span></span>|[<span data-ttu-id="f6ed1-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f6ed1-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f6ed1-196">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f6ed1-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f6ed1-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f6ed1-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f6ed1-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f6ed1-199">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f6ed1-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6ed1-200">Response</span></span>
<span data-ttu-id="f6ed1-201">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-201">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6ed1-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6ed1-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6ed1-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6ed1-203">Request</span></span>
<span data-ttu-id="f6ed1-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1006

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "publishingState": "processing",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f6ed1-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6ed1-205">Response</span></span>
<span data-ttu-id="f6ed1-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6ed1-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1178

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "publishingState": "processing",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```



