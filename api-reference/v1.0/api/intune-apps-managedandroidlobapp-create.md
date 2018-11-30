---
title: managedAndroidLobApp erstellen
description: Erstellen eines neuen managedAndroidLobApp-Objekts.
ms.openlocfilehash: 0822bbc0679f1cb19ec8e4c3d217a3bf5661cdaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019464"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="28644-103">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="28644-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="28644-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="28644-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28644-105">Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28644-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28644-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28644-106">Prerequisites</span></span>
<span data-ttu-id="28644-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28644-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28644-109">Permission type</span></span>|<span data-ttu-id="28644-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28644-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28644-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28644-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28644-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28644-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28644-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28644-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28644-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28644-114">Not supported.</span></span>|
|<span data-ttu-id="28644-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28644-115">Application</span></span>|<span data-ttu-id="28644-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28644-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28644-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28644-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="28644-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28644-118">Request headers</span></span>
|<span data-ttu-id="28644-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="28644-119">Header</span></span>|<span data-ttu-id="28644-120">Wert</span><span class="sxs-lookup"><span data-stu-id="28644-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28644-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28644-121">Authorization</span></span>|<span data-ttu-id="28644-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28644-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28644-123">Accept</span><span class="sxs-lookup"><span data-stu-id="28644-123">Accept</span></span>|<span data-ttu-id="28644-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28644-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28644-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28644-125">Request body</span></span>
<span data-ttu-id="28644-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="28644-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="28644-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="28644-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="28644-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28644-128">Property</span></span>|<span data-ttu-id="28644-129">Typ</span><span class="sxs-lookup"><span data-stu-id="28644-129">Type</span></span>|<span data-ttu-id="28644-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28644-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28644-131">id</span><span class="sxs-lookup"><span data-stu-id="28644-131">id</span></span>|<span data-ttu-id="28644-132">String</span><span class="sxs-lookup"><span data-stu-id="28644-132">String</span></span>|<span data-ttu-id="28644-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="28644-133">Key of the entity.</span></span> <span data-ttu-id="28644-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-135">displayName</span><span class="sxs-lookup"><span data-stu-id="28644-135">displayName</span></span>|<span data-ttu-id="28644-136">String</span><span class="sxs-lookup"><span data-stu-id="28644-136">String</span></span>|<span data-ttu-id="28644-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="28644-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="28644-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-139">description</span><span class="sxs-lookup"><span data-stu-id="28644-139">description</span></span>|<span data-ttu-id="28644-140">String</span><span class="sxs-lookup"><span data-stu-id="28644-140">String</span></span>|<span data-ttu-id="28644-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="28644-141">The description of the app.</span></span> <span data-ttu-id="28644-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-143">publisher</span><span class="sxs-lookup"><span data-stu-id="28644-143">publisher</span></span>|<span data-ttu-id="28644-144">String</span><span class="sxs-lookup"><span data-stu-id="28644-144">String</span></span>|<span data-ttu-id="28644-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="28644-145">The publisher of the app.</span></span> <span data-ttu-id="28644-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="28644-147">largeIcon</span></span>|[<span data-ttu-id="28644-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28644-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28644-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="28644-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="28644-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28644-151">createdDateTime</span></span>|<span data-ttu-id="28644-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28644-152">DateTimeOffset</span></span>|<span data-ttu-id="28644-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="28644-153">The date and time the app was created.</span></span> <span data-ttu-id="28644-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28644-155">lastModifiedDateTime</span></span>|<span data-ttu-id="28644-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28644-156">DateTimeOffset</span></span>|<span data-ttu-id="28644-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="28644-157">The date and time the app was last modified.</span></span> <span data-ttu-id="28644-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="28644-159">isFeatured</span></span>|<span data-ttu-id="28644-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="28644-160">Boolean</span></span>|<span data-ttu-id="28644-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="28644-162">privacyInformationUrl</span></span>|<span data-ttu-id="28644-163">String</span><span class="sxs-lookup"><span data-stu-id="28644-163">String</span></span>|<span data-ttu-id="28644-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="28644-164">The privacy statement Url.</span></span> <span data-ttu-id="28644-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="28644-166">informationUrl</span></span>|<span data-ttu-id="28644-167">String</span><span class="sxs-lookup"><span data-stu-id="28644-167">String</span></span>|<span data-ttu-id="28644-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="28644-168">The more information Url.</span></span> <span data-ttu-id="28644-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-170">owner</span><span class="sxs-lookup"><span data-stu-id="28644-170">owner</span></span>|<span data-ttu-id="28644-171">String</span><span class="sxs-lookup"><span data-stu-id="28644-171">String</span></span>|<span data-ttu-id="28644-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="28644-172">The owner of the app.</span></span> <span data-ttu-id="28644-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-174">developer</span><span class="sxs-lookup"><span data-stu-id="28644-174">developer</span></span>|<span data-ttu-id="28644-175">String</span><span class="sxs-lookup"><span data-stu-id="28644-175">String</span></span>|<span data-ttu-id="28644-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="28644-176">The developer of the app.</span></span> <span data-ttu-id="28644-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-178">notes</span><span class="sxs-lookup"><span data-stu-id="28644-178">notes</span></span>|<span data-ttu-id="28644-179">String</span><span class="sxs-lookup"><span data-stu-id="28644-179">String</span></span>|<span data-ttu-id="28644-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="28644-180">Notes for the app.</span></span> <span data-ttu-id="28644-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="28644-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="28644-182">publishingState</span></span>|[<span data-ttu-id="28644-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="28644-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="28644-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="28644-184">The publishing state for the app.</span></span> <span data-ttu-id="28644-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="28644-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="28644-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="28644-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="28644-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="28644-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="28644-188">appAvailability</span></span>|[<span data-ttu-id="28644-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="28644-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="28644-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="28644-190">The Application's availability.</span></span> <span data-ttu-id="28644-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="28644-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="28644-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="28644-193">version</span><span class="sxs-lookup"><span data-stu-id="28644-193">version</span></span>|<span data-ttu-id="28644-194">String</span><span class="sxs-lookup"><span data-stu-id="28644-194">String</span></span>|<span data-ttu-id="28644-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="28644-195">The Application's version.</span></span> <span data-ttu-id="28644-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="28644-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="28644-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="28644-197">committedContentVersion</span></span>|<span data-ttu-id="28644-198">String</span><span class="sxs-lookup"><span data-stu-id="28644-198">String</span></span>|<span data-ttu-id="28644-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="28644-199">The internal committed content version.</span></span> <span data-ttu-id="28644-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="28644-201">fileName</span><span class="sxs-lookup"><span data-stu-id="28644-201">fileName</span></span>|<span data-ttu-id="28644-202">String</span><span class="sxs-lookup"><span data-stu-id="28644-202">String</span></span>|<span data-ttu-id="28644-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="28644-203">The name of the main Lob application file.</span></span> <span data-ttu-id="28644-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="28644-205">size</span><span class="sxs-lookup"><span data-stu-id="28644-205">size</span></span>|<span data-ttu-id="28644-206">Int64</span><span class="sxs-lookup"><span data-stu-id="28644-206">Int64</span></span>|<span data-ttu-id="28644-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="28644-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="28644-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="28644-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="28644-209">packageId</span><span class="sxs-lookup"><span data-stu-id="28644-209">packageId</span></span>|<span data-ttu-id="28644-210">String</span><span class="sxs-lookup"><span data-stu-id="28644-210">String</span></span>|<span data-ttu-id="28644-211">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="28644-211">The package identifier.</span></span>|
|<span data-ttu-id="28644-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="28644-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="28644-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="28644-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="28644-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="28644-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="28644-215">versionName</span><span class="sxs-lookup"><span data-stu-id="28644-215">versionName</span></span>|<span data-ttu-id="28644-216">String</span><span class="sxs-lookup"><span data-stu-id="28644-216">String</span></span>|<span data-ttu-id="28644-217">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="28644-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="28644-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="28644-218">versionCode</span></span>|<span data-ttu-id="28644-219">String</span><span class="sxs-lookup"><span data-stu-id="28644-219">String</span></span>|<span data-ttu-id="28644-220">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="28644-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="28644-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="28644-221">Response</span></span>
<span data-ttu-id="28644-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28644-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28644-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28644-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="28644-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28644-224">Request</span></span>
<span data-ttu-id="28644-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28644-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="28644-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="28644-226">Response</span></span>
<span data-ttu-id="28644-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28644-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```


