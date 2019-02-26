---
title: managedAndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24d985046fa7fad39e121466e27c99c16909cd5b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261418"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="2892d-103">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2892d-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="2892d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2892d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2892d-105">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2892d-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2892d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2892d-106">Prerequisites</span></span>
<span data-ttu-id="2892d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2892d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2892d-109">Permission type</span></span>|<span data-ttu-id="2892d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2892d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2892d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2892d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2892d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2892d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2892d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2892d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2892d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2892d-114">Not supported.</span></span>|
|<span data-ttu-id="2892d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2892d-115">Application</span></span>|<span data-ttu-id="2892d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2892d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2892d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2892d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2892d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2892d-118">Request headers</span></span>
|<span data-ttu-id="2892d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2892d-119">Header</span></span>|<span data-ttu-id="2892d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2892d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2892d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2892d-121">Authorization</span></span>|<span data-ttu-id="2892d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2892d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2892d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2892d-123">Accept</span></span>|<span data-ttu-id="2892d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2892d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2892d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2892d-125">Request body</span></span>
<span data-ttu-id="2892d-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2892d-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="2892d-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2892d-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="2892d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2892d-128">Property</span></span>|<span data-ttu-id="2892d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2892d-129">Type</span></span>|<span data-ttu-id="2892d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2892d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2892d-131">id</span><span class="sxs-lookup"><span data-stu-id="2892d-131">id</span></span>|<span data-ttu-id="2892d-132">string</span><span class="sxs-lookup"><span data-stu-id="2892d-132">String</span></span>|<span data-ttu-id="2892d-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2892d-133">Key of the entity.</span></span> <span data-ttu-id="2892d-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2892d-135">displayName</span></span>|<span data-ttu-id="2892d-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-136">String</span></span>|<span data-ttu-id="2892d-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2892d-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-139">description</span><span class="sxs-lookup"><span data-stu-id="2892d-139">description</span></span>|<span data-ttu-id="2892d-140">String</span><span class="sxs-lookup"><span data-stu-id="2892d-140">String</span></span>|<span data-ttu-id="2892d-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-141">The description of the app.</span></span> <span data-ttu-id="2892d-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="2892d-143">publisher</span></span>|<span data-ttu-id="2892d-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-144">String</span></span>|<span data-ttu-id="2892d-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-145">The publisher of the app.</span></span> <span data-ttu-id="2892d-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2892d-147">largeIcon</span></span>|[<span data-ttu-id="2892d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2892d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2892d-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2892d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2892d-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2892d-151">createdDateTime</span></span>|<span data-ttu-id="2892d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2892d-152">DateTimeOffset</span></span>|<span data-ttu-id="2892d-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-153">The date and time the app was created.</span></span> <span data-ttu-id="2892d-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2892d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2892d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2892d-156">DateTimeOffset</span></span>|<span data-ttu-id="2892d-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="2892d-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2892d-159">isFeatured</span></span>|<span data-ttu-id="2892d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2892d-160">Boolean</span></span>|<span data-ttu-id="2892d-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2892d-162">privacyInformationUrl</span></span>|<span data-ttu-id="2892d-163">String</span><span class="sxs-lookup"><span data-stu-id="2892d-163">String</span></span>|<span data-ttu-id="2892d-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="2892d-164">The privacy statement Url.</span></span> <span data-ttu-id="2892d-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2892d-166">informationUrl</span></span>|<span data-ttu-id="2892d-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-167">String</span></span>|<span data-ttu-id="2892d-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="2892d-168">The more information Url.</span></span> <span data-ttu-id="2892d-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-170">owner</span><span class="sxs-lookup"><span data-stu-id="2892d-170">owner</span></span>|<span data-ttu-id="2892d-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-171">String</span></span>|<span data-ttu-id="2892d-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-172">The owner of the app.</span></span> <span data-ttu-id="2892d-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-174">developer</span><span class="sxs-lookup"><span data-stu-id="2892d-174">developer</span></span>|<span data-ttu-id="2892d-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-175">String</span></span>|<span data-ttu-id="2892d-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-176">The developer of the app.</span></span> <span data-ttu-id="2892d-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-178">notes</span><span class="sxs-lookup"><span data-stu-id="2892d-178">notes</span></span>|<span data-ttu-id="2892d-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-179">String</span></span>|<span data-ttu-id="2892d-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="2892d-180">Notes for the app.</span></span> <span data-ttu-id="2892d-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2892d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="2892d-182">publishingState</span></span>|[<span data-ttu-id="2892d-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2892d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2892d-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="2892d-184">The publishing state for the app.</span></span> <span data-ttu-id="2892d-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="2892d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2892d-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="2892d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2892d-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="2892d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2892d-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="2892d-188">appAvailability</span></span>|[<span data-ttu-id="2892d-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="2892d-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="2892d-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="2892d-190">The Application's availability.</span></span> <span data-ttu-id="2892d-191">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="2892d-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="2892d-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="2892d-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="2892d-193">version</span><span class="sxs-lookup"><span data-stu-id="2892d-193">version</span></span>|<span data-ttu-id="2892d-194">String</span><span class="sxs-lookup"><span data-stu-id="2892d-194">String</span></span>|<span data-ttu-id="2892d-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="2892d-195">The Application's version.</span></span> <span data-ttu-id="2892d-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2892d-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="2892d-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2892d-197">committedContentVersion</span></span>|<span data-ttu-id="2892d-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-198">String</span></span>|<span data-ttu-id="2892d-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="2892d-199">The internal committed content version.</span></span> <span data-ttu-id="2892d-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2892d-201">fileName</span><span class="sxs-lookup"><span data-stu-id="2892d-201">fileName</span></span>|<span data-ttu-id="2892d-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-202">String</span></span>|<span data-ttu-id="2892d-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="2892d-203">The name of the main Lob application file.</span></span> <span data-ttu-id="2892d-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2892d-205">size</span><span class="sxs-lookup"><span data-stu-id="2892d-205">size</span></span>|<span data-ttu-id="2892d-206">Int64</span><span class="sxs-lookup"><span data-stu-id="2892d-206">Int64</span></span>|<span data-ttu-id="2892d-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="2892d-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="2892d-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2892d-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2892d-209">packageId</span><span class="sxs-lookup"><span data-stu-id="2892d-209">packageId</span></span>|<span data-ttu-id="2892d-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-210">String</span></span>|<span data-ttu-id="2892d-211">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="2892d-211">The package identifier.</span></span>|
|<span data-ttu-id="2892d-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2892d-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2892d-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2892d-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="2892d-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="2892d-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2892d-215">versionName</span><span class="sxs-lookup"><span data-stu-id="2892d-215">versionName</span></span>|<span data-ttu-id="2892d-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-216">String</span></span>|<span data-ttu-id="2892d-217">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="2892d-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2892d-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="2892d-218">versionCode</span></span>|<span data-ttu-id="2892d-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2892d-219">String</span></span>|<span data-ttu-id="2892d-220">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="2892d-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="2892d-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="2892d-221">Response</span></span>
<span data-ttu-id="2892d-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2892d-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2892d-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2892d-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="2892d-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2892d-224">Request</span></span>
<span data-ttu-id="2892d-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2892d-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="2892d-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="2892d-226">Response</span></span>
<span data-ttu-id="2892d-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2892d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



