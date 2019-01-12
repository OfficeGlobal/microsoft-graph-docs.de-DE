---
title: managedAndroidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 00b9988df08715d469f3bd0ed1d3b47529620b69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980531"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="039fa-103">managedAndroidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="039fa-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="039fa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="039fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="039fa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="039fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="039fa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="039fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="039fa-107">Aktualisieren der Eigenschaften eines [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="039fa-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="039fa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="039fa-108">Prerequisites</span></span>
<span data-ttu-id="039fa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="039fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="039fa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="039fa-111">Permission type</span></span>|<span data-ttu-id="039fa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="039fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="039fa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="039fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="039fa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039fa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="039fa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="039fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="039fa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="039fa-116">Not supported.</span></span>|
|<span data-ttu-id="039fa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="039fa-117">Application</span></span>|<span data-ttu-id="039fa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="039fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="039fa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="039fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="039fa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="039fa-120">Request headers</span></span>
|<span data-ttu-id="039fa-121">Header</span><span class="sxs-lookup"><span data-stu-id="039fa-121">Header</span></span>|<span data-ttu-id="039fa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="039fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="039fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="039fa-123">Authorization</span></span>|<span data-ttu-id="039fa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="039fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="039fa-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="039fa-125">Accept</span></span>|<span data-ttu-id="039fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="039fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="039fa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="039fa-127">Request body</span></span>
<span data-ttu-id="039fa-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="039fa-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="039fa-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="039fa-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="039fa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="039fa-130">Property</span></span>|<span data-ttu-id="039fa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="039fa-131">Type</span></span>|<span data-ttu-id="039fa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="039fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039fa-133">id</span><span class="sxs-lookup"><span data-stu-id="039fa-133">id</span></span>|<span data-ttu-id="039fa-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-134">String</span></span>|<span data-ttu-id="039fa-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="039fa-135">Key of the entity.</span></span> <span data-ttu-id="039fa-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="039fa-137">displayName</span></span>|<span data-ttu-id="039fa-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-138">String</span></span>|<span data-ttu-id="039fa-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="039fa-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-141">description</span><span class="sxs-lookup"><span data-stu-id="039fa-141">description</span></span>|<span data-ttu-id="039fa-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-142">String</span></span>|<span data-ttu-id="039fa-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-143">The description of the app.</span></span> <span data-ttu-id="039fa-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-145">publisher</span><span class="sxs-lookup"><span data-stu-id="039fa-145">publisher</span></span>|<span data-ttu-id="039fa-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-146">String</span></span>|<span data-ttu-id="039fa-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-147">The publisher of the app.</span></span> <span data-ttu-id="039fa-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="039fa-149">largeIcon</span></span>|[<span data-ttu-id="039fa-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="039fa-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="039fa-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="039fa-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="039fa-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="039fa-153">createdDateTime</span></span>|<span data-ttu-id="039fa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039fa-154">DateTimeOffset</span></span>|<span data-ttu-id="039fa-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-155">The date and time the app was created.</span></span> <span data-ttu-id="039fa-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="039fa-157">lastModifiedDateTime</span></span>|<span data-ttu-id="039fa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039fa-158">DateTimeOffset</span></span>|<span data-ttu-id="039fa-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-159">The date and time the app was last modified.</span></span> <span data-ttu-id="039fa-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="039fa-161">isFeatured</span></span>|<span data-ttu-id="039fa-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="039fa-162">Boolean</span></span>|<span data-ttu-id="039fa-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="039fa-164">privacyInformationUrl</span></span>|<span data-ttu-id="039fa-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-165">String</span></span>|<span data-ttu-id="039fa-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="039fa-166">The privacy statement Url.</span></span> <span data-ttu-id="039fa-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="039fa-168">informationUrl</span></span>|<span data-ttu-id="039fa-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-169">String</span></span>|<span data-ttu-id="039fa-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="039fa-170">The more information Url.</span></span> <span data-ttu-id="039fa-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-172">owner</span><span class="sxs-lookup"><span data-stu-id="039fa-172">owner</span></span>|<span data-ttu-id="039fa-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-173">String</span></span>|<span data-ttu-id="039fa-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-174">The owner of the app.</span></span> <span data-ttu-id="039fa-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-176">developer</span><span class="sxs-lookup"><span data-stu-id="039fa-176">developer</span></span>|<span data-ttu-id="039fa-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-177">String</span></span>|<span data-ttu-id="039fa-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-178">The developer of the app.</span></span> <span data-ttu-id="039fa-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-180">notes</span><span class="sxs-lookup"><span data-stu-id="039fa-180">notes</span></span>|<span data-ttu-id="039fa-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-181">String</span></span>|<span data-ttu-id="039fa-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="039fa-182">Notes for the app.</span></span> <span data-ttu-id="039fa-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="039fa-184">uploadState</span></span>|<span data-ttu-id="039fa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="039fa-185">Int32</span></span>|<span data-ttu-id="039fa-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="039fa-186">The upload state.</span></span> <span data-ttu-id="039fa-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="039fa-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="039fa-188">publishingState</span></span>|[<span data-ttu-id="039fa-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="039fa-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="039fa-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-190">The publishing state for the app.</span></span> <span data-ttu-id="039fa-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="039fa-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="039fa-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="039fa-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="039fa-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="039fa-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="039fa-194">appAvailability</span></span>|[<span data-ttu-id="039fa-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="039fa-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="039fa-196">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="039fa-196">The Application's availability.</span></span> <span data-ttu-id="039fa-197">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="039fa-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="039fa-198">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="039fa-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="039fa-199">version</span><span class="sxs-lookup"><span data-stu-id="039fa-199">version</span></span>|<span data-ttu-id="039fa-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-200">String</span></span>|<span data-ttu-id="039fa-201">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="039fa-201">The Application's version.</span></span> <span data-ttu-id="039fa-202">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="039fa-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="039fa-203">packageId</span><span class="sxs-lookup"><span data-stu-id="039fa-203">packageId</span></span>|<span data-ttu-id="039fa-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-204">String</span></span>|<span data-ttu-id="039fa-205">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="039fa-205">The app's package ID.</span></span>|
|<span data-ttu-id="039fa-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="039fa-206">appStoreUrl</span></span>|<span data-ttu-id="039fa-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039fa-207">String</span></span>|<span data-ttu-id="039fa-208">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="039fa-208">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="039fa-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="039fa-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="039fa-210">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="039fa-210">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="039fa-211">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="039fa-211">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="039fa-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="039fa-212">Response</span></span>
<span data-ttu-id="039fa-213">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="039fa-213">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="039fa-214">Beispiel</span><span class="sxs-lookup"><span data-stu-id="039fa-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="039fa-215">Anforderung</span><span class="sxs-lookup"><span data-stu-id="039fa-215">Request</span></span>
<span data-ttu-id="039fa-216">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="039fa-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1155

{
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

### <a name="response"></a><span data-ttu-id="039fa-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="039fa-217">Response</span></span>
<span data-ttu-id="039fa-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="039fa-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1324

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





