---
title: managedAndroidLobApp erstellen
description: Erstellen eines neuen managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9999b29aa4840f7e27fa0a69e6ff4b76daeec7ca
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250663"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="157f0-103">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="157f0-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="157f0-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="157f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="157f0-105">Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="157f0-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="157f0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="157f0-106">Prerequisites</span></span>
<span data-ttu-id="157f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="157f0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="157f0-109">Permission type</span></span>|<span data-ttu-id="157f0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="157f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="157f0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="157f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="157f0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157f0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="157f0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="157f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="157f0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="157f0-114">Not supported.</span></span>|
|<span data-ttu-id="157f0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="157f0-115">Application</span></span>|<span data-ttu-id="157f0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="157f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="157f0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="157f0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="157f0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="157f0-118">Request headers</span></span>
|<span data-ttu-id="157f0-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="157f0-119">Header</span></span>|<span data-ttu-id="157f0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="157f0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="157f0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="157f0-121">Authorization</span></span>|<span data-ttu-id="157f0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="157f0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="157f0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="157f0-123">Accept</span></span>|<span data-ttu-id="157f0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="157f0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="157f0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="157f0-125">Request body</span></span>
<span data-ttu-id="157f0-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="157f0-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="157f0-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="157f0-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="157f0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="157f0-128">Property</span></span>|<span data-ttu-id="157f0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="157f0-129">Type</span></span>|<span data-ttu-id="157f0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="157f0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157f0-131">id</span><span class="sxs-lookup"><span data-stu-id="157f0-131">id</span></span>|<span data-ttu-id="157f0-132">string</span><span class="sxs-lookup"><span data-stu-id="157f0-132">String</span></span>|<span data-ttu-id="157f0-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="157f0-133">Key of the entity.</span></span> <span data-ttu-id="157f0-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="157f0-135">displayName</span></span>|<span data-ttu-id="157f0-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-136">String</span></span>|<span data-ttu-id="157f0-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="157f0-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-139">description</span><span class="sxs-lookup"><span data-stu-id="157f0-139">description</span></span>|<span data-ttu-id="157f0-140">String</span><span class="sxs-lookup"><span data-stu-id="157f0-140">String</span></span>|<span data-ttu-id="157f0-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-141">The description of the app.</span></span> <span data-ttu-id="157f0-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-143">publisher</span><span class="sxs-lookup"><span data-stu-id="157f0-143">publisher</span></span>|<span data-ttu-id="157f0-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-144">String</span></span>|<span data-ttu-id="157f0-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-145">The publisher of the app.</span></span> <span data-ttu-id="157f0-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="157f0-147">largeIcon</span></span>|[<span data-ttu-id="157f0-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="157f0-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="157f0-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="157f0-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="157f0-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="157f0-151">createdDateTime</span></span>|<span data-ttu-id="157f0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157f0-152">DateTimeOffset</span></span>|<span data-ttu-id="157f0-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-153">The date and time the app was created.</span></span> <span data-ttu-id="157f0-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="157f0-155">lastModifiedDateTime</span></span>|<span data-ttu-id="157f0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157f0-156">DateTimeOffset</span></span>|<span data-ttu-id="157f0-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-157">The date and time the app was last modified.</span></span> <span data-ttu-id="157f0-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="157f0-159">isFeatured</span></span>|<span data-ttu-id="157f0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="157f0-160">Boolean</span></span>|<span data-ttu-id="157f0-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="157f0-162">privacyInformationUrl</span></span>|<span data-ttu-id="157f0-163">String</span><span class="sxs-lookup"><span data-stu-id="157f0-163">String</span></span>|<span data-ttu-id="157f0-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="157f0-164">The privacy statement Url.</span></span> <span data-ttu-id="157f0-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="157f0-166">informationUrl</span></span>|<span data-ttu-id="157f0-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-167">String</span></span>|<span data-ttu-id="157f0-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="157f0-168">The more information Url.</span></span> <span data-ttu-id="157f0-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-170">owner</span><span class="sxs-lookup"><span data-stu-id="157f0-170">owner</span></span>|<span data-ttu-id="157f0-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-171">String</span></span>|<span data-ttu-id="157f0-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-172">The owner of the app.</span></span> <span data-ttu-id="157f0-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-174">developer</span><span class="sxs-lookup"><span data-stu-id="157f0-174">developer</span></span>|<span data-ttu-id="157f0-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-175">String</span></span>|<span data-ttu-id="157f0-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-176">The developer of the app.</span></span> <span data-ttu-id="157f0-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-178">notes</span><span class="sxs-lookup"><span data-stu-id="157f0-178">notes</span></span>|<span data-ttu-id="157f0-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-179">String</span></span>|<span data-ttu-id="157f0-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="157f0-180">Notes for the app.</span></span> <span data-ttu-id="157f0-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="157f0-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="157f0-182">publishingState</span></span>|[<span data-ttu-id="157f0-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="157f0-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="157f0-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="157f0-184">The publishing state for the app.</span></span> <span data-ttu-id="157f0-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="157f0-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="157f0-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="157f0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="157f0-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="157f0-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="157f0-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="157f0-188">appAvailability</span></span>|[<span data-ttu-id="157f0-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="157f0-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="157f0-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="157f0-190">The Application's availability.</span></span> <span data-ttu-id="157f0-191">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="157f0-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="157f0-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="157f0-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="157f0-193">version</span><span class="sxs-lookup"><span data-stu-id="157f0-193">version</span></span>|<span data-ttu-id="157f0-194">String</span><span class="sxs-lookup"><span data-stu-id="157f0-194">String</span></span>|<span data-ttu-id="157f0-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="157f0-195">The Application's version.</span></span> <span data-ttu-id="157f0-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="157f0-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="157f0-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="157f0-197">committedContentVersion</span></span>|<span data-ttu-id="157f0-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-198">String</span></span>|<span data-ttu-id="157f0-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="157f0-199">The internal committed content version.</span></span> <span data-ttu-id="157f0-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="157f0-201">fileName</span><span class="sxs-lookup"><span data-stu-id="157f0-201">fileName</span></span>|<span data-ttu-id="157f0-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-202">String</span></span>|<span data-ttu-id="157f0-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="157f0-203">The name of the main Lob application file.</span></span> <span data-ttu-id="157f0-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="157f0-205">size</span><span class="sxs-lookup"><span data-stu-id="157f0-205">size</span></span>|<span data-ttu-id="157f0-206">Int64</span><span class="sxs-lookup"><span data-stu-id="157f0-206">Int64</span></span>|<span data-ttu-id="157f0-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="157f0-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="157f0-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="157f0-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="157f0-209">packageId</span><span class="sxs-lookup"><span data-stu-id="157f0-209">packageId</span></span>|<span data-ttu-id="157f0-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-210">String</span></span>|<span data-ttu-id="157f0-211">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="157f0-211">The package identifier.</span></span>|
|<span data-ttu-id="157f0-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="157f0-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="157f0-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="157f0-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="157f0-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="157f0-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="157f0-215">versionName</span><span class="sxs-lookup"><span data-stu-id="157f0-215">versionName</span></span>|<span data-ttu-id="157f0-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-216">String</span></span>|<span data-ttu-id="157f0-217">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="157f0-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="157f0-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="157f0-218">versionCode</span></span>|<span data-ttu-id="157f0-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="157f0-219">String</span></span>|<span data-ttu-id="157f0-220">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="157f0-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="157f0-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="157f0-221">Response</span></span>
<span data-ttu-id="157f0-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="157f0-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="157f0-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="157f0-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="157f0-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="157f0-224">Request</span></span>
<span data-ttu-id="157f0-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="157f0-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="157f0-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="157f0-226">Response</span></span>
<span data-ttu-id="157f0-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="157f0-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



