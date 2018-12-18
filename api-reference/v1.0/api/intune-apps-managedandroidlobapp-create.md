---
title: managedAndroidLobApp erstellen
description: Erstellen eines neuen managedAndroidLobApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 2a86720eb942821bfd8ff47dbc71b934f12d9e7d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302373"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="0717c-103">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="0717c-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="0717c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0717c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0717c-105">Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0717c-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0717c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0717c-106">Prerequisites</span></span>
<span data-ttu-id="0717c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0717c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0717c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0717c-109">Permission type</span></span>|<span data-ttu-id="0717c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0717c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0717c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0717c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0717c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0717c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0717c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0717c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0717c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0717c-114">Not supported.</span></span>|
|<span data-ttu-id="0717c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0717c-115">Application</span></span>|<span data-ttu-id="0717c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0717c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0717c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0717c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0717c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0717c-118">Request headers</span></span>
|<span data-ttu-id="0717c-119">Header</span><span class="sxs-lookup"><span data-stu-id="0717c-119">Header</span></span>|<span data-ttu-id="0717c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0717c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0717c-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0717c-121">Authorization</span></span>|<span data-ttu-id="0717c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0717c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0717c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0717c-123">Accept</span></span>|<span data-ttu-id="0717c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0717c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0717c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0717c-125">Request body</span></span>
<span data-ttu-id="0717c-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0717c-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="0717c-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0717c-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="0717c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0717c-128">Property</span></span>|<span data-ttu-id="0717c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0717c-129">Type</span></span>|<span data-ttu-id="0717c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0717c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0717c-131">id</span><span class="sxs-lookup"><span data-stu-id="0717c-131">id</span></span>|<span data-ttu-id="0717c-132">String</span><span class="sxs-lookup"><span data-stu-id="0717c-132">String</span></span>|<span data-ttu-id="0717c-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0717c-133">Key of the entity.</span></span> <span data-ttu-id="0717c-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0717c-135">displayName</span></span>|<span data-ttu-id="0717c-136">String</span><span class="sxs-lookup"><span data-stu-id="0717c-136">String</span></span>|<span data-ttu-id="0717c-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0717c-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-139">description</span><span class="sxs-lookup"><span data-stu-id="0717c-139">description</span></span>|<span data-ttu-id="0717c-140">String</span><span class="sxs-lookup"><span data-stu-id="0717c-140">String</span></span>|<span data-ttu-id="0717c-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-141">The description of the app.</span></span> <span data-ttu-id="0717c-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-143">publisher</span><span class="sxs-lookup"><span data-stu-id="0717c-143">publisher</span></span>|<span data-ttu-id="0717c-144">String</span><span class="sxs-lookup"><span data-stu-id="0717c-144">String</span></span>|<span data-ttu-id="0717c-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-145">The publisher of the app.</span></span> <span data-ttu-id="0717c-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0717c-147">largeIcon</span></span>|[<span data-ttu-id="0717c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0717c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0717c-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0717c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0717c-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0717c-151">createdDateTime</span></span>|<span data-ttu-id="0717c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0717c-152">DateTimeOffset</span></span>|<span data-ttu-id="0717c-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-153">The date and time the app was created.</span></span> <span data-ttu-id="0717c-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0717c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="0717c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0717c-156">DateTimeOffset</span></span>|<span data-ttu-id="0717c-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="0717c-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0717c-159">isFeatured</span></span>|<span data-ttu-id="0717c-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0717c-160">Boolean</span></span>|<span data-ttu-id="0717c-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0717c-162">privacyInformationUrl</span></span>|<span data-ttu-id="0717c-163">String</span><span class="sxs-lookup"><span data-stu-id="0717c-163">String</span></span>|<span data-ttu-id="0717c-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="0717c-164">The privacy statement Url.</span></span> <span data-ttu-id="0717c-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0717c-166">informationUrl</span></span>|<span data-ttu-id="0717c-167">String</span><span class="sxs-lookup"><span data-stu-id="0717c-167">String</span></span>|<span data-ttu-id="0717c-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="0717c-168">The more information Url.</span></span> <span data-ttu-id="0717c-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-170">owner</span><span class="sxs-lookup"><span data-stu-id="0717c-170">owner</span></span>|<span data-ttu-id="0717c-171">String</span><span class="sxs-lookup"><span data-stu-id="0717c-171">String</span></span>|<span data-ttu-id="0717c-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-172">The owner of the app.</span></span> <span data-ttu-id="0717c-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-174">developer</span><span class="sxs-lookup"><span data-stu-id="0717c-174">developer</span></span>|<span data-ttu-id="0717c-175">String</span><span class="sxs-lookup"><span data-stu-id="0717c-175">String</span></span>|<span data-ttu-id="0717c-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-176">The developer of the app.</span></span> <span data-ttu-id="0717c-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-178">notes</span><span class="sxs-lookup"><span data-stu-id="0717c-178">notes</span></span>|<span data-ttu-id="0717c-179">String</span><span class="sxs-lookup"><span data-stu-id="0717c-179">String</span></span>|<span data-ttu-id="0717c-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="0717c-180">Notes for the app.</span></span> <span data-ttu-id="0717c-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0717c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="0717c-182">publishingState</span></span>|[<span data-ttu-id="0717c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0717c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0717c-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="0717c-184">The publishing state for the app.</span></span> <span data-ttu-id="0717c-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="0717c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0717c-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0717c-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="0717c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0717c-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0717c-188">appAvailability</span></span>|[<span data-ttu-id="0717c-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0717c-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="0717c-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="0717c-190">The Application's availability.</span></span> <span data-ttu-id="0717c-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="0717c-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0717c-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0717c-193">version</span><span class="sxs-lookup"><span data-stu-id="0717c-193">version</span></span>|<span data-ttu-id="0717c-194">String</span><span class="sxs-lookup"><span data-stu-id="0717c-194">String</span></span>|<span data-ttu-id="0717c-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="0717c-195">The Application's version.</span></span> <span data-ttu-id="0717c-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0717c-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="0717c-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0717c-197">committedContentVersion</span></span>|<span data-ttu-id="0717c-198">String</span><span class="sxs-lookup"><span data-stu-id="0717c-198">String</span></span>|<span data-ttu-id="0717c-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="0717c-199">The internal committed content version.</span></span> <span data-ttu-id="0717c-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0717c-201">fileName</span><span class="sxs-lookup"><span data-stu-id="0717c-201">fileName</span></span>|<span data-ttu-id="0717c-202">String</span><span class="sxs-lookup"><span data-stu-id="0717c-202">String</span></span>|<span data-ttu-id="0717c-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="0717c-203">The name of the main Lob application file.</span></span> <span data-ttu-id="0717c-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0717c-205">size</span><span class="sxs-lookup"><span data-stu-id="0717c-205">size</span></span>|<span data-ttu-id="0717c-206">Int64</span><span class="sxs-lookup"><span data-stu-id="0717c-206">Int64</span></span>|<span data-ttu-id="0717c-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="0717c-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="0717c-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0717c-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0717c-209">packageId</span><span class="sxs-lookup"><span data-stu-id="0717c-209">packageId</span></span>|<span data-ttu-id="0717c-210">String</span><span class="sxs-lookup"><span data-stu-id="0717c-210">String</span></span>|<span data-ttu-id="0717c-211">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="0717c-211">The package identifier.</span></span>|
|<span data-ttu-id="0717c-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0717c-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0717c-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0717c-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0717c-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="0717c-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0717c-215">versionName</span><span class="sxs-lookup"><span data-stu-id="0717c-215">versionName</span></span>|<span data-ttu-id="0717c-216">String</span><span class="sxs-lookup"><span data-stu-id="0717c-216">String</span></span>|<span data-ttu-id="0717c-217">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="0717c-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0717c-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="0717c-218">versionCode</span></span>|<span data-ttu-id="0717c-219">String</span><span class="sxs-lookup"><span data-stu-id="0717c-219">String</span></span>|<span data-ttu-id="0717c-220">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="0717c-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="0717c-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="0717c-221">Response</span></span>
<span data-ttu-id="0717c-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0717c-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0717c-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0717c-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="0717c-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0717c-224">Request</span></span>
<span data-ttu-id="0717c-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0717c-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0717c-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="0717c-226">Response</span></span>
<span data-ttu-id="0717c-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0717c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



