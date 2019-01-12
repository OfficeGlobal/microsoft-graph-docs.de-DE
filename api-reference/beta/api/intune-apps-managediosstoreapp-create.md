---
title: managedIOSStoreApp erstellen
description: Erstellen eines neuen managedIOSStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2733d9da3a870489e6a9c92e6ba25bf3ab023b61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915935"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="abda6-103">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="abda6-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="abda6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="abda6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abda6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abda6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abda6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="abda6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abda6-107">Erstellen eines neuen [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="abda6-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abda6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abda6-108">Prerequisites</span></span>
<span data-ttu-id="abda6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abda6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abda6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abda6-111">Permission type</span></span>|<span data-ttu-id="abda6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abda6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abda6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abda6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abda6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abda6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abda6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abda6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abda6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abda6-116">Not supported.</span></span>|
|<span data-ttu-id="abda6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abda6-117">Application</span></span>|<span data-ttu-id="abda6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abda6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abda6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abda6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="abda6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abda6-120">Request headers</span></span>
|<span data-ttu-id="abda6-121">Header</span><span class="sxs-lookup"><span data-stu-id="abda6-121">Header</span></span>|<span data-ttu-id="abda6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="abda6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abda6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abda6-123">Authorization</span></span>|<span data-ttu-id="abda6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abda6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abda6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="abda6-125">Accept</span></span>|<span data-ttu-id="abda6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abda6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abda6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abda6-127">Request body</span></span>
<span data-ttu-id="abda6-128">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="abda6-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="abda6-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="abda6-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="abda6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abda6-130">Property</span></span>|<span data-ttu-id="abda6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="abda6-131">Type</span></span>|<span data-ttu-id="abda6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abda6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abda6-133">id</span><span class="sxs-lookup"><span data-stu-id="abda6-133">id</span></span>|<span data-ttu-id="abda6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-134">String</span></span>|<span data-ttu-id="abda6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="abda6-135">Key of the entity.</span></span> <span data-ttu-id="abda6-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="abda6-137">displayName</span></span>|<span data-ttu-id="abda6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-138">String</span></span>|<span data-ttu-id="abda6-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="abda6-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-141">description</span><span class="sxs-lookup"><span data-stu-id="abda6-141">description</span></span>|<span data-ttu-id="abda6-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-142">String</span></span>|<span data-ttu-id="abda6-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-143">The description of the app.</span></span> <span data-ttu-id="abda6-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-145">publisher</span><span class="sxs-lookup"><span data-stu-id="abda6-145">publisher</span></span>|<span data-ttu-id="abda6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-146">String</span></span>|<span data-ttu-id="abda6-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-147">The publisher of the app.</span></span> <span data-ttu-id="abda6-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="abda6-149">largeIcon</span></span>|[<span data-ttu-id="abda6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="abda6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="abda6-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="abda6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="abda6-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abda6-153">createdDateTime</span></span>|<span data-ttu-id="abda6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abda6-154">DateTimeOffset</span></span>|<span data-ttu-id="abda6-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-155">The date and time the app was created.</span></span> <span data-ttu-id="abda6-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abda6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="abda6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abda6-158">DateTimeOffset</span></span>|<span data-ttu-id="abda6-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="abda6-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="abda6-161">isFeatured</span></span>|<span data-ttu-id="abda6-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="abda6-162">Boolean</span></span>|<span data-ttu-id="abda6-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="abda6-164">privacyInformationUrl</span></span>|<span data-ttu-id="abda6-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-165">String</span></span>|<span data-ttu-id="abda6-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="abda6-166">The privacy statement Url.</span></span> <span data-ttu-id="abda6-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="abda6-168">informationUrl</span></span>|<span data-ttu-id="abda6-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-169">String</span></span>|<span data-ttu-id="abda6-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="abda6-170">The more information Url.</span></span> <span data-ttu-id="abda6-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-172">owner</span><span class="sxs-lookup"><span data-stu-id="abda6-172">owner</span></span>|<span data-ttu-id="abda6-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-173">String</span></span>|<span data-ttu-id="abda6-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-174">The owner of the app.</span></span> <span data-ttu-id="abda6-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-176">developer</span><span class="sxs-lookup"><span data-stu-id="abda6-176">developer</span></span>|<span data-ttu-id="abda6-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-177">String</span></span>|<span data-ttu-id="abda6-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-178">The developer of the app.</span></span> <span data-ttu-id="abda6-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-180">notes</span><span class="sxs-lookup"><span data-stu-id="abda6-180">notes</span></span>|<span data-ttu-id="abda6-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-181">String</span></span>|<span data-ttu-id="abda6-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="abda6-182">Notes for the app.</span></span> <span data-ttu-id="abda6-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="abda6-184">uploadState</span></span>|<span data-ttu-id="abda6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="abda6-185">Int32</span></span>|<span data-ttu-id="abda6-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="abda6-186">The upload state.</span></span> <span data-ttu-id="abda6-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="abda6-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="abda6-188">publishingState</span></span>|[<span data-ttu-id="abda6-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="abda6-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="abda6-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="abda6-190">The publishing state for the app.</span></span> <span data-ttu-id="abda6-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="abda6-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="abda6-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="abda6-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="abda6-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="abda6-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="abda6-194">appAvailability</span></span>|[<span data-ttu-id="abda6-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="abda6-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="abda6-196">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="abda6-196">The Application's availability.</span></span> <span data-ttu-id="abda6-197">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="abda6-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="abda6-198">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="abda6-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="abda6-199">version</span><span class="sxs-lookup"><span data-stu-id="abda6-199">version</span></span>|<span data-ttu-id="abda6-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-200">String</span></span>|<span data-ttu-id="abda6-201">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="abda6-201">The Application's version.</span></span> <span data-ttu-id="abda6-202">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="abda6-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="abda6-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="abda6-203">bundleId</span></span>|<span data-ttu-id="abda6-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-204">String</span></span>|<span data-ttu-id="abda6-205">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="abda6-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="abda6-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="abda6-206">appStoreUrl</span></span>|<span data-ttu-id="abda6-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abda6-207">String</span></span>|<span data-ttu-id="abda6-208">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="abda6-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="abda6-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="abda6-209">applicableDeviceType</span></span>|[<span data-ttu-id="abda6-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="abda6-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="abda6-211">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="abda6-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="abda6-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="abda6-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="abda6-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="abda6-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="abda6-214">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="abda6-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="abda6-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="abda6-215">Response</span></span>
<span data-ttu-id="abda6-216">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abda6-216">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abda6-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abda6-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="abda6-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abda6-218">Request</span></span>
<span data-ttu-id="abda6-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abda6-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="abda6-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="abda6-220">Response</span></span>
<span data-ttu-id="abda6-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abda6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





