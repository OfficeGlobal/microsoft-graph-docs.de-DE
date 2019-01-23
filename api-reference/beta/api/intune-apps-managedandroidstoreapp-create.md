---
title: managedAndroidStoreApp erstellen
description: Erstellen eines neuen ManagedAndroidStoreApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a7bd4cf3b84140c61cdd84b024c6574271440620
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405205"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="73427-103">managedAndroidStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="73427-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="73427-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="73427-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73427-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73427-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73427-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73427-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73427-107">Erstellen eines neuen [ManagedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73427-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73427-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73427-108">Prerequisites</span></span>
<span data-ttu-id="73427-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="73427-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73427-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73427-111">Permission type</span></span>|<span data-ttu-id="73427-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73427-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73427-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73427-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73427-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73427-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73427-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73427-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73427-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73427-116">Not supported.</span></span>|
|<span data-ttu-id="73427-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73427-117">Application</span></span>|<span data-ttu-id="73427-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73427-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73427-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73427-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73427-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73427-120">Request headers</span></span>
|<span data-ttu-id="73427-121">Header</span><span class="sxs-lookup"><span data-stu-id="73427-121">Header</span></span>|<span data-ttu-id="73427-122">Wert</span><span class="sxs-lookup"><span data-stu-id="73427-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73427-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="73427-123">Authorization</span></span>|<span data-ttu-id="73427-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73427-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73427-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73427-125">Accept</span></span>|<span data-ttu-id="73427-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73427-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73427-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73427-127">Request body</span></span>
<span data-ttu-id="73427-128">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="73427-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="73427-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="73427-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="73427-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73427-130">Property</span></span>|<span data-ttu-id="73427-131">Typ</span><span class="sxs-lookup"><span data-stu-id="73427-131">Type</span></span>|<span data-ttu-id="73427-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73427-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73427-133">id</span><span class="sxs-lookup"><span data-stu-id="73427-133">id</span></span>|<span data-ttu-id="73427-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-134">String</span></span>|<span data-ttu-id="73427-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="73427-135">Key of the entity.</span></span> <span data-ttu-id="73427-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-137">displayName</span><span class="sxs-lookup"><span data-stu-id="73427-137">displayName</span></span>|<span data-ttu-id="73427-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-138">String</span></span>|<span data-ttu-id="73427-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="73427-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73427-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-141">description</span><span class="sxs-lookup"><span data-stu-id="73427-141">description</span></span>|<span data-ttu-id="73427-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-142">String</span></span>|<span data-ttu-id="73427-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="73427-143">The description of the app.</span></span> <span data-ttu-id="73427-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-145">publisher</span><span class="sxs-lookup"><span data-stu-id="73427-145">publisher</span></span>|<span data-ttu-id="73427-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-146">String</span></span>|<span data-ttu-id="73427-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="73427-147">The publisher of the app.</span></span> <span data-ttu-id="73427-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73427-149">largeIcon</span></span>|[<span data-ttu-id="73427-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73427-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73427-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="73427-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73427-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73427-153">createdDateTime</span></span>|<span data-ttu-id="73427-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73427-154">DateTimeOffset</span></span>|<span data-ttu-id="73427-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="73427-155">The date and time the app was created.</span></span> <span data-ttu-id="73427-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73427-157">lastModifiedDateTime</span></span>|<span data-ttu-id="73427-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73427-158">DateTimeOffset</span></span>|<span data-ttu-id="73427-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="73427-159">The date and time the app was last modified.</span></span> <span data-ttu-id="73427-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73427-161">isFeatured</span></span>|<span data-ttu-id="73427-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="73427-162">Boolean</span></span>|<span data-ttu-id="73427-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73427-164">privacyInformationUrl</span></span>|<span data-ttu-id="73427-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-165">String</span></span>|<span data-ttu-id="73427-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="73427-166">The privacy statement Url.</span></span> <span data-ttu-id="73427-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73427-168">informationUrl</span></span>|<span data-ttu-id="73427-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-169">String</span></span>|<span data-ttu-id="73427-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="73427-170">The more information Url.</span></span> <span data-ttu-id="73427-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-172">owner</span><span class="sxs-lookup"><span data-stu-id="73427-172">owner</span></span>|<span data-ttu-id="73427-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-173">String</span></span>|<span data-ttu-id="73427-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="73427-174">The owner of the app.</span></span> <span data-ttu-id="73427-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-176">developer</span><span class="sxs-lookup"><span data-stu-id="73427-176">developer</span></span>|<span data-ttu-id="73427-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-177">String</span></span>|<span data-ttu-id="73427-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="73427-178">The developer of the app.</span></span> <span data-ttu-id="73427-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-180">notes</span><span class="sxs-lookup"><span data-stu-id="73427-180">notes</span></span>|<span data-ttu-id="73427-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-181">String</span></span>|<span data-ttu-id="73427-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="73427-182">Notes for the app.</span></span> <span data-ttu-id="73427-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="73427-184">uploadState</span></span>|<span data-ttu-id="73427-185">Int32</span><span class="sxs-lookup"><span data-stu-id="73427-185">Int32</span></span>|<span data-ttu-id="73427-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="73427-186">The upload state.</span></span> <span data-ttu-id="73427-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="73427-188">publishingState</span></span>|[<span data-ttu-id="73427-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="73427-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="73427-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="73427-190">The publishing state for the app.</span></span> <span data-ttu-id="73427-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="73427-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73427-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="73427-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="73427-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="73427-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="73427-194">isAssigned</span></span>|<span data-ttu-id="73427-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="73427-195">Boolean</span></span>|<span data-ttu-id="73427-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="73427-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="73427-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73427-198">roleScopeTagIds</span></span>|<span data-ttu-id="73427-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="73427-199">String collection</span></span>|<span data-ttu-id="73427-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="73427-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="73427-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73427-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="73427-202">appAvailability</span></span>|[<span data-ttu-id="73427-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="73427-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="73427-204">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="73427-204">The Application's availability.</span></span> <span data-ttu-id="73427-205">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="73427-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="73427-206">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="73427-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="73427-207">version</span><span class="sxs-lookup"><span data-stu-id="73427-207">version</span></span>|<span data-ttu-id="73427-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-208">String</span></span>|<span data-ttu-id="73427-209">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="73427-209">The Application's version.</span></span> <span data-ttu-id="73427-210">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="73427-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="73427-211">packageId</span><span class="sxs-lookup"><span data-stu-id="73427-211">packageId</span></span>|<span data-ttu-id="73427-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-212">String</span></span>|<span data-ttu-id="73427-213">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="73427-213">The app's package ID.</span></span>|
|<span data-ttu-id="73427-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="73427-214">appStoreUrl</span></span>|<span data-ttu-id="73427-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73427-215">String</span></span>|<span data-ttu-id="73427-216">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="73427-216">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="73427-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73427-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="73427-218">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73427-218">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="73427-219">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="73427-219">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="73427-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="73427-220">Response</span></span>
<span data-ttu-id="73427-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73427-221">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73427-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73427-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="73427-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73427-223">Request</span></span>
<span data-ttu-id="73427-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73427-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="73427-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="73427-225">Response</span></span>
<span data-ttu-id="73427-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73427-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




