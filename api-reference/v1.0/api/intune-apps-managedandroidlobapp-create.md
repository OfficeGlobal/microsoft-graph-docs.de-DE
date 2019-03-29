---
title: managedAndroidLobApp erstellen
description: Erstellen eines neuen managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2f7932a9ea627769432b9c686420c892cc04eb2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962281"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="e2a13-103">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="e2a13-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="e2a13-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e2a13-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2a13-105">Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2a13-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2a13-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e2a13-106">Prerequisites</span></span>
<span data-ttu-id="e2a13-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2a13-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2a13-109">Permission type</span></span>|<span data-ttu-id="e2a13-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2a13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2a13-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2a13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2a13-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a13-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2a13-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2a13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2a13-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2a13-114">Not supported.</span></span>|
|<span data-ttu-id="e2a13-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2a13-115">Application</span></span>|<span data-ttu-id="e2a13-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2a13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2a13-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2a13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e2a13-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2a13-118">Request headers</span></span>
|<span data-ttu-id="e2a13-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e2a13-119">Header</span></span>|<span data-ttu-id="e2a13-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e2a13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2a13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2a13-121">Authorization</span></span>|<span data-ttu-id="e2a13-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e2a13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2a13-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e2a13-123">Accept</span></span>|<span data-ttu-id="e2a13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e2a13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2a13-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2a13-125">Request body</span></span>
<span data-ttu-id="e2a13-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e2a13-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="e2a13-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e2a13-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="e2a13-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2a13-128">Property</span></span>|<span data-ttu-id="e2a13-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e2a13-129">Type</span></span>|<span data-ttu-id="e2a13-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2a13-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a13-131">id</span><span class="sxs-lookup"><span data-stu-id="e2a13-131">id</span></span>|<span data-ttu-id="e2a13-132">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-132">String</span></span>|<span data-ttu-id="e2a13-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e2a13-133">Key of the entity.</span></span> <span data-ttu-id="e2a13-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e2a13-135">displayName</span></span>|<span data-ttu-id="e2a13-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2a13-136">String</span></span>|<span data-ttu-id="e2a13-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e2a13-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-139">description</span><span class="sxs-lookup"><span data-stu-id="e2a13-139">description</span></span>|<span data-ttu-id="e2a13-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2a13-140">String</span></span>|<span data-ttu-id="e2a13-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-141">The description of the app.</span></span> <span data-ttu-id="e2a13-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e2a13-143">publisher</span></span>|<span data-ttu-id="e2a13-144">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-144">String</span></span>|<span data-ttu-id="e2a13-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-145">The publisher of the app.</span></span> <span data-ttu-id="e2a13-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e2a13-147">largeIcon</span></span>|[<span data-ttu-id="e2a13-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2a13-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2a13-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e2a13-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e2a13-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a13-151">createdDateTime</span></span>|<span data-ttu-id="e2a13-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a13-152">DateTimeOffset</span></span>|<span data-ttu-id="e2a13-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-153">The date and time the app was created.</span></span> <span data-ttu-id="e2a13-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a13-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e2a13-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a13-156">DateTimeOffset</span></span>|<span data-ttu-id="e2a13-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e2a13-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e2a13-159">isFeatured</span></span>|<span data-ttu-id="e2a13-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a13-160">Boolean</span></span>|<span data-ttu-id="e2a13-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e2a13-162">privacyInformationUrl</span></span>|<span data-ttu-id="e2a13-163">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-163">String</span></span>|<span data-ttu-id="e2a13-164">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="e2a13-164">The privacy statement Url.</span></span> <span data-ttu-id="e2a13-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e2a13-166">informationUrl</span></span>|<span data-ttu-id="e2a13-167">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-167">String</span></span>|<span data-ttu-id="e2a13-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e2a13-168">The more information Url.</span></span> <span data-ttu-id="e2a13-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-170">owner</span><span class="sxs-lookup"><span data-stu-id="e2a13-170">owner</span></span>|<span data-ttu-id="e2a13-171">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-171">String</span></span>|<span data-ttu-id="e2a13-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-172">The owner of the app.</span></span> <span data-ttu-id="e2a13-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-174">developer</span><span class="sxs-lookup"><span data-stu-id="e2a13-174">developer</span></span>|<span data-ttu-id="e2a13-175">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-175">String</span></span>|<span data-ttu-id="e2a13-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-176">The developer of the app.</span></span> <span data-ttu-id="e2a13-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-178">notes</span><span class="sxs-lookup"><span data-stu-id="e2a13-178">notes</span></span>|<span data-ttu-id="e2a13-179">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-179">String</span></span>|<span data-ttu-id="e2a13-180">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-180">Notes for the app.</span></span> <span data-ttu-id="e2a13-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2a13-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e2a13-182">publishingState</span></span>|[<span data-ttu-id="e2a13-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e2a13-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e2a13-184">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-184">The publishing state for the app.</span></span> <span data-ttu-id="e2a13-185">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e2a13-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e2a13-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e2a13-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e2a13-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e2a13-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e2a13-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e2a13-188">appAvailability</span></span>|[<span data-ttu-id="e2a13-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e2a13-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e2a13-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="e2a13-190">The Application's availability.</span></span> <span data-ttu-id="e2a13-191">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e2a13-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e2a13-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e2a13-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e2a13-193">version</span><span class="sxs-lookup"><span data-stu-id="e2a13-193">version</span></span>|<span data-ttu-id="e2a13-194">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-194">String</span></span>|<span data-ttu-id="e2a13-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="e2a13-195">The Application's version.</span></span> <span data-ttu-id="e2a13-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2a13-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e2a13-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e2a13-197">committedContentVersion</span></span>|<span data-ttu-id="e2a13-198">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-198">String</span></span>|<span data-ttu-id="e2a13-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="e2a13-199">The internal committed content version.</span></span> <span data-ttu-id="e2a13-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e2a13-201">fileName</span><span class="sxs-lookup"><span data-stu-id="e2a13-201">fileName</span></span>|<span data-ttu-id="e2a13-202">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-202">String</span></span>|<span data-ttu-id="e2a13-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="e2a13-203">The name of the main Lob application file.</span></span> <span data-ttu-id="e2a13-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e2a13-205">size</span><span class="sxs-lookup"><span data-stu-id="e2a13-205">size</span></span>|<span data-ttu-id="e2a13-206">Int64</span><span class="sxs-lookup"><span data-stu-id="e2a13-206">Int64</span></span>|<span data-ttu-id="e2a13-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="e2a13-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="e2a13-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e2a13-209">packageId</span><span class="sxs-lookup"><span data-stu-id="e2a13-209">packageId</span></span>|<span data-ttu-id="e2a13-210">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-210">String</span></span>|<span data-ttu-id="e2a13-211">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="e2a13-211">The package identifier.</span></span>|
|<span data-ttu-id="e2a13-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2a13-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e2a13-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2a13-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e2a13-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="e2a13-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e2a13-215">versionName</span><span class="sxs-lookup"><span data-stu-id="e2a13-215">versionName</span></span>|<span data-ttu-id="e2a13-216">String</span><span class="sxs-lookup"><span data-stu-id="e2a13-216">String</span></span>|<span data-ttu-id="e2a13-217">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e2a13-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="e2a13-218">versionCode</span></span>|<span data-ttu-id="e2a13-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2a13-219">String</span></span>|<span data-ttu-id="e2a13-220">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="e2a13-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e2a13-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2a13-221">Response</span></span>
<span data-ttu-id="e2a13-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2a13-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a13-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2a13-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2a13-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2a13-224">Request</span></span>
<span data-ttu-id="e2a13-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2a13-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2a13-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2a13-226">Response</span></span>
<span data-ttu-id="e2a13-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2a13-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



