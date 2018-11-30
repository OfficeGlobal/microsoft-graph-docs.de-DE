---
title: Erstellen von „iosVppApp“
description: Erstellen eines neuen iosVppApp-Objekts.
ms.openlocfilehash: cb7b0926145d2448195662cef817292fb41ac1e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017145"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="be203-103">Erstellen von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="be203-103">Create iosVppApp</span></span>

> <span data-ttu-id="be203-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be203-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be203-105">Erstellen eines neuen [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="be203-105">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be203-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="be203-106">Prerequisites</span></span>
<span data-ttu-id="be203-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be203-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be203-109">Permission type</span></span>|<span data-ttu-id="be203-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be203-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be203-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be203-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be203-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be203-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be203-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be203-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be203-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be203-114">Not supported.</span></span>|
|<span data-ttu-id="be203-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be203-115">Application</span></span>|<span data-ttu-id="be203-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be203-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be203-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be203-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="be203-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be203-118">Request headers</span></span>
|<span data-ttu-id="be203-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="be203-119">Header</span></span>|<span data-ttu-id="be203-120">Wert</span><span class="sxs-lookup"><span data-stu-id="be203-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be203-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be203-121">Authorization</span></span>|<span data-ttu-id="be203-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="be203-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be203-123">Accept</span><span class="sxs-lookup"><span data-stu-id="be203-123">Accept</span></span>|<span data-ttu-id="be203-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be203-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be203-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be203-125">Request body</span></span>
<span data-ttu-id="be203-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="be203-126">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="be203-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="be203-127">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="be203-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be203-128">Property</span></span>|<span data-ttu-id="be203-129">Typ</span><span class="sxs-lookup"><span data-stu-id="be203-129">Type</span></span>|<span data-ttu-id="be203-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be203-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be203-131">id</span><span class="sxs-lookup"><span data-stu-id="be203-131">id</span></span>|<span data-ttu-id="be203-132">String</span><span class="sxs-lookup"><span data-stu-id="be203-132">String</span></span>|<span data-ttu-id="be203-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="be203-133">Key of the entity.</span></span> <span data-ttu-id="be203-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-135">displayName</span><span class="sxs-lookup"><span data-stu-id="be203-135">displayName</span></span>|<span data-ttu-id="be203-136">String</span><span class="sxs-lookup"><span data-stu-id="be203-136">String</span></span>|<span data-ttu-id="be203-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="be203-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="be203-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-139">description</span><span class="sxs-lookup"><span data-stu-id="be203-139">description</span></span>|<span data-ttu-id="be203-140">String</span><span class="sxs-lookup"><span data-stu-id="be203-140">String</span></span>|<span data-ttu-id="be203-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="be203-141">The description of the app.</span></span> <span data-ttu-id="be203-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-143">publisher</span><span class="sxs-lookup"><span data-stu-id="be203-143">publisher</span></span>|<span data-ttu-id="be203-144">String</span><span class="sxs-lookup"><span data-stu-id="be203-144">String</span></span>|<span data-ttu-id="be203-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="be203-145">The publisher of the app.</span></span> <span data-ttu-id="be203-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="be203-147">largeIcon</span></span>|[<span data-ttu-id="be203-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="be203-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="be203-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="be203-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="be203-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be203-151">createdDateTime</span></span>|<span data-ttu-id="be203-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be203-152">DateTimeOffset</span></span>|<span data-ttu-id="be203-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="be203-153">The date and time the app was created.</span></span> <span data-ttu-id="be203-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be203-155">lastModifiedDateTime</span></span>|<span data-ttu-id="be203-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be203-156">DateTimeOffset</span></span>|<span data-ttu-id="be203-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="be203-157">The date and time the app was last modified.</span></span> <span data-ttu-id="be203-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="be203-159">isFeatured</span></span>|<span data-ttu-id="be203-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be203-160">Boolean</span></span>|<span data-ttu-id="be203-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="be203-162">privacyInformationUrl</span></span>|<span data-ttu-id="be203-163">String</span><span class="sxs-lookup"><span data-stu-id="be203-163">String</span></span>|<span data-ttu-id="be203-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="be203-164">The privacy statement Url.</span></span> <span data-ttu-id="be203-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="be203-166">informationUrl</span></span>|<span data-ttu-id="be203-167">String</span><span class="sxs-lookup"><span data-stu-id="be203-167">String</span></span>|<span data-ttu-id="be203-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="be203-168">The more information Url.</span></span> <span data-ttu-id="be203-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-170">owner</span><span class="sxs-lookup"><span data-stu-id="be203-170">owner</span></span>|<span data-ttu-id="be203-171">String</span><span class="sxs-lookup"><span data-stu-id="be203-171">String</span></span>|<span data-ttu-id="be203-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="be203-172">The owner of the app.</span></span> <span data-ttu-id="be203-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-174">developer</span><span class="sxs-lookup"><span data-stu-id="be203-174">developer</span></span>|<span data-ttu-id="be203-175">String</span><span class="sxs-lookup"><span data-stu-id="be203-175">String</span></span>|<span data-ttu-id="be203-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="be203-176">The developer of the app.</span></span> <span data-ttu-id="be203-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-178">notes</span><span class="sxs-lookup"><span data-stu-id="be203-178">notes</span></span>|<span data-ttu-id="be203-179">String</span><span class="sxs-lookup"><span data-stu-id="be203-179">String</span></span>|<span data-ttu-id="be203-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="be203-180">Notes for the app.</span></span> <span data-ttu-id="be203-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be203-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="be203-182">publishingState</span></span>|[<span data-ttu-id="be203-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="be203-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="be203-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="be203-184">The publishing state for the app.</span></span> <span data-ttu-id="be203-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="be203-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="be203-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be203-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="be203-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="be203-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="be203-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="be203-188">usedLicenseCount</span></span>|<span data-ttu-id="be203-189">Int32</span><span class="sxs-lookup"><span data-stu-id="be203-189">Int32</span></span>|<span data-ttu-id="be203-190">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="be203-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="be203-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="be203-191">totalLicenseCount</span></span>|<span data-ttu-id="be203-192">Int32</span><span class="sxs-lookup"><span data-stu-id="be203-192">Int32</span></span>|<span data-ttu-id="be203-193">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="be203-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="be203-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="be203-194">releaseDateTime</span></span>|<span data-ttu-id="be203-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be203-195">DateTimeOffset</span></span>|<span data-ttu-id="be203-196">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="be203-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="be203-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="be203-197">appStoreUrl</span></span>|<span data-ttu-id="be203-198">String</span><span class="sxs-lookup"><span data-stu-id="be203-198">String</span></span>|<span data-ttu-id="be203-199">Store-URL</span><span class="sxs-lookup"><span data-stu-id="be203-199">The store URL.</span></span>|
|<span data-ttu-id="be203-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="be203-200">licensingType</span></span>|[<span data-ttu-id="be203-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="be203-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="be203-202">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="be203-202">The supported License Type.</span></span>|
|<span data-ttu-id="be203-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="be203-203">applicableDeviceType</span></span>|[<span data-ttu-id="be203-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="be203-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="be203-205">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="be203-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="be203-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="be203-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="be203-207">String</span><span class="sxs-lookup"><span data-stu-id="be203-207">String</span></span>|<span data-ttu-id="be203-208">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="be203-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="be203-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="be203-209">vppTokenAccountType</span></span>|[<span data-ttu-id="be203-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="be203-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="be203-211">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="be203-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="be203-212">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="be203-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="be203-213">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="be203-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="be203-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="be203-214">vppTokenAppleId</span></span>|<span data-ttu-id="be203-215">String</span><span class="sxs-lookup"><span data-stu-id="be203-215">String</span></span>|<span data-ttu-id="be203-216">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="be203-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="be203-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="be203-217">bundleId</span></span>|<span data-ttu-id="be203-218">String</span><span class="sxs-lookup"><span data-stu-id="be203-218">String</span></span>|<span data-ttu-id="be203-219">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="be203-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="be203-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="be203-220">Response</span></span>
<span data-ttu-id="be203-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be203-221">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be203-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be203-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="be203-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be203-223">Request</span></span>
<span data-ttu-id="be203-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be203-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="be203-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="be203-225">Response</span></span>
<span data-ttu-id="be203-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be203-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



