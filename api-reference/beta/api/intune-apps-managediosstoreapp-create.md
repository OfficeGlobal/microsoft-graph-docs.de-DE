---
title: managedIOSStoreApp erstellen
description: Erstellen eines neuen managedIOSStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f689bdcf8b9197314f688a9dc86c3fe1240597b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879303"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="376fd-103">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="376fd-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="376fd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="376fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="376fd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="376fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="376fd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="376fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="376fd-107">Erstellen eines neuen [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="376fd-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="376fd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="376fd-108">Prerequisites</span></span>
<span data-ttu-id="376fd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376fd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="376fd-111">Permission type</span></span>|<span data-ttu-id="376fd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="376fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376fd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="376fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="376fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="376fd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="376fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376fd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="376fd-116">Not supported.</span></span>|
|<span data-ttu-id="376fd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="376fd-117">Application</span></span>|<span data-ttu-id="376fd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="376fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="376fd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="376fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="376fd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="376fd-120">Request headers</span></span>
|<span data-ttu-id="376fd-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="376fd-121">Header</span></span>|<span data-ttu-id="376fd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="376fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="376fd-123">Authorization</span></span>|<span data-ttu-id="376fd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="376fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376fd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="376fd-125">Accept</span></span>|<span data-ttu-id="376fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="376fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376fd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="376fd-127">Request body</span></span>
<span data-ttu-id="376fd-128">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="376fd-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="376fd-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="376fd-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="376fd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="376fd-130">Property</span></span>|<span data-ttu-id="376fd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="376fd-131">Type</span></span>|<span data-ttu-id="376fd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="376fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376fd-133">id</span><span class="sxs-lookup"><span data-stu-id="376fd-133">id</span></span>|<span data-ttu-id="376fd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-134">String</span></span>|<span data-ttu-id="376fd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="376fd-135">Key of the entity.</span></span> <span data-ttu-id="376fd-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="376fd-137">displayName</span></span>|<span data-ttu-id="376fd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-138">String</span></span>|<span data-ttu-id="376fd-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="376fd-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-141">description</span><span class="sxs-lookup"><span data-stu-id="376fd-141">description</span></span>|<span data-ttu-id="376fd-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-142">String</span></span>|<span data-ttu-id="376fd-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-143">The description of the app.</span></span> <span data-ttu-id="376fd-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="376fd-145">publisher</span></span>|<span data-ttu-id="376fd-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-146">String</span></span>|<span data-ttu-id="376fd-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-147">The publisher of the app.</span></span> <span data-ttu-id="376fd-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="376fd-149">largeIcon</span></span>|[<span data-ttu-id="376fd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="376fd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="376fd-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="376fd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="376fd-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="376fd-153">createdDateTime</span></span>|<span data-ttu-id="376fd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376fd-154">DateTimeOffset</span></span>|<span data-ttu-id="376fd-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-155">The date and time the app was created.</span></span> <span data-ttu-id="376fd-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="376fd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="376fd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376fd-158">DateTimeOffset</span></span>|<span data-ttu-id="376fd-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="376fd-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="376fd-161">isFeatured</span></span>|<span data-ttu-id="376fd-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="376fd-162">Boolean</span></span>|<span data-ttu-id="376fd-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="376fd-164">privacyInformationUrl</span></span>|<span data-ttu-id="376fd-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-165">String</span></span>|<span data-ttu-id="376fd-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="376fd-166">The privacy statement Url.</span></span> <span data-ttu-id="376fd-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="376fd-168">informationUrl</span></span>|<span data-ttu-id="376fd-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-169">String</span></span>|<span data-ttu-id="376fd-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="376fd-170">The more information Url.</span></span> <span data-ttu-id="376fd-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-172">owner</span><span class="sxs-lookup"><span data-stu-id="376fd-172">owner</span></span>|<span data-ttu-id="376fd-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-173">String</span></span>|<span data-ttu-id="376fd-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-174">The owner of the app.</span></span> <span data-ttu-id="376fd-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-176">developer</span><span class="sxs-lookup"><span data-stu-id="376fd-176">developer</span></span>|<span data-ttu-id="376fd-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-177">String</span></span>|<span data-ttu-id="376fd-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-178">The developer of the app.</span></span> <span data-ttu-id="376fd-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-180">notes</span><span class="sxs-lookup"><span data-stu-id="376fd-180">notes</span></span>|<span data-ttu-id="376fd-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-181">String</span></span>|<span data-ttu-id="376fd-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="376fd-182">Notes for the app.</span></span> <span data-ttu-id="376fd-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="376fd-184">uploadState</span></span>|<span data-ttu-id="376fd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="376fd-185">Int32</span></span>|<span data-ttu-id="376fd-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="376fd-186">The upload state.</span></span> <span data-ttu-id="376fd-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="376fd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="376fd-188">publishingState</span></span>|[<span data-ttu-id="376fd-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="376fd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="376fd-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="376fd-190">The publishing state for the app.</span></span> <span data-ttu-id="376fd-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="376fd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="376fd-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="376fd-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="376fd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="376fd-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="376fd-194">appAvailability</span></span>|[<span data-ttu-id="376fd-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="376fd-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="376fd-196">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="376fd-196">The Application's availability.</span></span> <span data-ttu-id="376fd-197">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="376fd-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="376fd-198">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="376fd-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="376fd-199">version</span><span class="sxs-lookup"><span data-stu-id="376fd-199">version</span></span>|<span data-ttu-id="376fd-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-200">String</span></span>|<span data-ttu-id="376fd-201">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="376fd-201">The Application's version.</span></span> <span data-ttu-id="376fd-202">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="376fd-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="376fd-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="376fd-203">bundleId</span></span>|<span data-ttu-id="376fd-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-204">String</span></span>|<span data-ttu-id="376fd-205">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="376fd-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="376fd-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="376fd-206">appStoreUrl</span></span>|<span data-ttu-id="376fd-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="376fd-207">String</span></span>|<span data-ttu-id="376fd-208">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="376fd-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="376fd-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="376fd-209">applicableDeviceType</span></span>|[<span data-ttu-id="376fd-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="376fd-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="376fd-211">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="376fd-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="376fd-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="376fd-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="376fd-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="376fd-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="376fd-214">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="376fd-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="376fd-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="376fd-215">Response</span></span>
<span data-ttu-id="376fd-216">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="376fd-216">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376fd-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="376fd-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="376fd-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="376fd-218">Request</span></span>
<span data-ttu-id="376fd-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="376fd-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="376fd-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="376fd-220">Response</span></span>
<span data-ttu-id="376fd-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="376fd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1278

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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





