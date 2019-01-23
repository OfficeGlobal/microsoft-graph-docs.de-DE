---
title: managedAndroidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidStoreApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07cd1d7ca6bbec237a853e8670437e07a06cb2a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421046"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="fac87-103">managedAndroidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fac87-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="fac87-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fac87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fac87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fac87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fac87-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fac87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fac87-107">Aktualisieren der Eigenschaften eines [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fac87-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fac87-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fac87-108">Prerequisites</span></span>
<span data-ttu-id="fac87-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fac87-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fac87-111">Permission type</span></span>|<span data-ttu-id="fac87-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fac87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fac87-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fac87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fac87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fac87-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fac87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fac87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fac87-116">Not supported.</span></span>|
|<span data-ttu-id="fac87-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fac87-117">Application</span></span>|<span data-ttu-id="fac87-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fac87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fac87-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fac87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="fac87-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fac87-120">Request headers</span></span>
|<span data-ttu-id="fac87-121">Header</span><span class="sxs-lookup"><span data-stu-id="fac87-121">Header</span></span>|<span data-ttu-id="fac87-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fac87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fac87-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fac87-123">Authorization</span></span>|<span data-ttu-id="fac87-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fac87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fac87-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fac87-125">Accept</span></span>|<span data-ttu-id="fac87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fac87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fac87-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fac87-127">Request body</span></span>
<span data-ttu-id="fac87-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fac87-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="fac87-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fac87-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="fac87-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fac87-130">Property</span></span>|<span data-ttu-id="fac87-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fac87-131">Type</span></span>|<span data-ttu-id="fac87-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fac87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fac87-133">id</span><span class="sxs-lookup"><span data-stu-id="fac87-133">id</span></span>|<span data-ttu-id="fac87-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-134">String</span></span>|<span data-ttu-id="fac87-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fac87-135">Key of the entity.</span></span> <span data-ttu-id="fac87-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fac87-137">displayName</span></span>|<span data-ttu-id="fac87-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-138">String</span></span>|<span data-ttu-id="fac87-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fac87-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-141">description</span><span class="sxs-lookup"><span data-stu-id="fac87-141">description</span></span>|<span data-ttu-id="fac87-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-142">String</span></span>|<span data-ttu-id="fac87-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-143">The description of the app.</span></span> <span data-ttu-id="fac87-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fac87-145">publisher</span></span>|<span data-ttu-id="fac87-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-146">String</span></span>|<span data-ttu-id="fac87-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-147">The publisher of the app.</span></span> <span data-ttu-id="fac87-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fac87-149">largeIcon</span></span>|[<span data-ttu-id="fac87-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fac87-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fac87-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="fac87-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fac87-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fac87-153">createdDateTime</span></span>|<span data-ttu-id="fac87-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fac87-154">DateTimeOffset</span></span>|<span data-ttu-id="fac87-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-155">The date and time the app was created.</span></span> <span data-ttu-id="fac87-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fac87-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fac87-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fac87-158">DateTimeOffset</span></span>|<span data-ttu-id="fac87-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fac87-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fac87-161">isFeatured</span></span>|<span data-ttu-id="fac87-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fac87-162">Boolean</span></span>|<span data-ttu-id="fac87-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fac87-164">privacyInformationUrl</span></span>|<span data-ttu-id="fac87-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-165">String</span></span>|<span data-ttu-id="fac87-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="fac87-166">The privacy statement Url.</span></span> <span data-ttu-id="fac87-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fac87-168">informationUrl</span></span>|<span data-ttu-id="fac87-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-169">String</span></span>|<span data-ttu-id="fac87-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="fac87-170">The more information Url.</span></span> <span data-ttu-id="fac87-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-172">owner</span><span class="sxs-lookup"><span data-stu-id="fac87-172">owner</span></span>|<span data-ttu-id="fac87-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-173">String</span></span>|<span data-ttu-id="fac87-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-174">The owner of the app.</span></span> <span data-ttu-id="fac87-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-176">developer</span><span class="sxs-lookup"><span data-stu-id="fac87-176">developer</span></span>|<span data-ttu-id="fac87-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-177">String</span></span>|<span data-ttu-id="fac87-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-178">The developer of the app.</span></span> <span data-ttu-id="fac87-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-180">notes</span><span class="sxs-lookup"><span data-stu-id="fac87-180">notes</span></span>|<span data-ttu-id="fac87-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-181">String</span></span>|<span data-ttu-id="fac87-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="fac87-182">Notes for the app.</span></span> <span data-ttu-id="fac87-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fac87-184">uploadState</span></span>|<span data-ttu-id="fac87-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fac87-185">Int32</span></span>|<span data-ttu-id="fac87-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="fac87-186">The upload state.</span></span> <span data-ttu-id="fac87-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="fac87-188">publishingState</span></span>|[<span data-ttu-id="fac87-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fac87-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fac87-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-190">The publishing state for the app.</span></span> <span data-ttu-id="fac87-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="fac87-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fac87-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fac87-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="fac87-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fac87-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fac87-194">isAssigned</span></span>|<span data-ttu-id="fac87-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="fac87-195">Boolean</span></span>|<span data-ttu-id="fac87-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="fac87-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fac87-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fac87-198">roleScopeTagIds</span></span>|<span data-ttu-id="fac87-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="fac87-199">String collection</span></span>|<span data-ttu-id="fac87-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="fac87-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fac87-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fac87-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="fac87-202">appAvailability</span></span>|[<span data-ttu-id="fac87-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="fac87-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="fac87-204">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="fac87-204">The Application's availability.</span></span> <span data-ttu-id="fac87-205">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fac87-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="fac87-206">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="fac87-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="fac87-207">version</span><span class="sxs-lookup"><span data-stu-id="fac87-207">version</span></span>|<span data-ttu-id="fac87-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-208">String</span></span>|<span data-ttu-id="fac87-209">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="fac87-209">The Application's version.</span></span> <span data-ttu-id="fac87-210">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="fac87-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="fac87-211">packageId</span><span class="sxs-lookup"><span data-stu-id="fac87-211">packageId</span></span>|<span data-ttu-id="fac87-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-212">String</span></span>|<span data-ttu-id="fac87-213">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="fac87-213">The app's package ID.</span></span>|
|<span data-ttu-id="fac87-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fac87-214">appStoreUrl</span></span>|<span data-ttu-id="fac87-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fac87-215">String</span></span>|<span data-ttu-id="fac87-216">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="fac87-216">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="fac87-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fac87-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fac87-218">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fac87-218">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="fac87-219">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="fac87-219">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="fac87-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="fac87-220">Response</span></span>
<span data-ttu-id="fac87-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fac87-221">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fac87-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fac87-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="fac87-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fac87-223">Request</span></span>
<span data-ttu-id="fac87-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fac87-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="fac87-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="fac87-225">Response</span></span>
<span data-ttu-id="fac87-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fac87-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




