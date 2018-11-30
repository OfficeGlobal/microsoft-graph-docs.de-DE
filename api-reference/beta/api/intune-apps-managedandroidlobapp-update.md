---
title: managedAndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidLobApp-Objekts.
ms.openlocfilehash: 72cfb5ac709c7864b5a02fbfa1858eb3bb7f666b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064126"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="62049-103">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="62049-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="62049-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="62049-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62049-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62049-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62049-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="62049-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62049-107">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="62049-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62049-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="62049-108">Prerequisites</span></span>
<span data-ttu-id="62049-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62049-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62049-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62049-111">Permission type</span></span>|<span data-ttu-id="62049-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62049-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62049-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62049-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62049-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62049-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62049-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62049-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62049-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62049-116">Not supported.</span></span>|
|<span data-ttu-id="62049-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62049-117">Application</span></span>|<span data-ttu-id="62049-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62049-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62049-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62049-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="62049-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62049-120">Request headers</span></span>
|<span data-ttu-id="62049-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="62049-121">Header</span></span>|<span data-ttu-id="62049-122">Wert</span><span class="sxs-lookup"><span data-stu-id="62049-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62049-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62049-123">Authorization</span></span>|<span data-ttu-id="62049-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="62049-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62049-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62049-125">Accept</span></span>|<span data-ttu-id="62049-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62049-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62049-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62049-127">Request body</span></span>
<span data-ttu-id="62049-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="62049-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="62049-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="62049-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="62049-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62049-130">Property</span></span>|<span data-ttu-id="62049-131">Typ</span><span class="sxs-lookup"><span data-stu-id="62049-131">Type</span></span>|<span data-ttu-id="62049-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62049-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62049-133">id</span><span class="sxs-lookup"><span data-stu-id="62049-133">id</span></span>|<span data-ttu-id="62049-134">String</span><span class="sxs-lookup"><span data-stu-id="62049-134">String</span></span>|<span data-ttu-id="62049-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="62049-135">Key of the entity.</span></span> <span data-ttu-id="62049-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-137">displayName</span><span class="sxs-lookup"><span data-stu-id="62049-137">displayName</span></span>|<span data-ttu-id="62049-138">String</span><span class="sxs-lookup"><span data-stu-id="62049-138">String</span></span>|<span data-ttu-id="62049-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="62049-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="62049-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-141">description</span><span class="sxs-lookup"><span data-stu-id="62049-141">description</span></span>|<span data-ttu-id="62049-142">String</span><span class="sxs-lookup"><span data-stu-id="62049-142">String</span></span>|<span data-ttu-id="62049-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="62049-143">The description of the app.</span></span> <span data-ttu-id="62049-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-145">publisher</span><span class="sxs-lookup"><span data-stu-id="62049-145">publisher</span></span>|<span data-ttu-id="62049-146">String</span><span class="sxs-lookup"><span data-stu-id="62049-146">String</span></span>|<span data-ttu-id="62049-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="62049-147">The publisher of the app.</span></span> <span data-ttu-id="62049-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="62049-149">largeIcon</span></span>|[<span data-ttu-id="62049-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="62049-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="62049-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="62049-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="62049-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62049-153">createdDateTime</span></span>|<span data-ttu-id="62049-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62049-154">DateTimeOffset</span></span>|<span data-ttu-id="62049-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="62049-155">The date and time the app was created.</span></span> <span data-ttu-id="62049-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62049-157">lastModifiedDateTime</span></span>|<span data-ttu-id="62049-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62049-158">DateTimeOffset</span></span>|<span data-ttu-id="62049-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="62049-159">The date and time the app was last modified.</span></span> <span data-ttu-id="62049-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="62049-161">isFeatured</span></span>|<span data-ttu-id="62049-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="62049-162">Boolean</span></span>|<span data-ttu-id="62049-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="62049-164">privacyInformationUrl</span></span>|<span data-ttu-id="62049-165">String</span><span class="sxs-lookup"><span data-stu-id="62049-165">String</span></span>|<span data-ttu-id="62049-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="62049-166">The privacy statement Url.</span></span> <span data-ttu-id="62049-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="62049-168">informationUrl</span></span>|<span data-ttu-id="62049-169">String</span><span class="sxs-lookup"><span data-stu-id="62049-169">String</span></span>|<span data-ttu-id="62049-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="62049-170">The more information Url.</span></span> <span data-ttu-id="62049-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-172">owner</span><span class="sxs-lookup"><span data-stu-id="62049-172">owner</span></span>|<span data-ttu-id="62049-173">String</span><span class="sxs-lookup"><span data-stu-id="62049-173">String</span></span>|<span data-ttu-id="62049-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="62049-174">The owner of the app.</span></span> <span data-ttu-id="62049-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-176">developer</span><span class="sxs-lookup"><span data-stu-id="62049-176">developer</span></span>|<span data-ttu-id="62049-177">String</span><span class="sxs-lookup"><span data-stu-id="62049-177">String</span></span>|<span data-ttu-id="62049-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="62049-178">The developer of the app.</span></span> <span data-ttu-id="62049-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-180">notes</span><span class="sxs-lookup"><span data-stu-id="62049-180">notes</span></span>|<span data-ttu-id="62049-181">String</span><span class="sxs-lookup"><span data-stu-id="62049-181">String</span></span>|<span data-ttu-id="62049-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="62049-182">Notes for the app.</span></span> <span data-ttu-id="62049-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="62049-184">uploadState</span></span>|<span data-ttu-id="62049-185">Int32</span><span class="sxs-lookup"><span data-stu-id="62049-185">Int32</span></span>|<span data-ttu-id="62049-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="62049-186">The upload state.</span></span> <span data-ttu-id="62049-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62049-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="62049-188">publishingState</span></span>|[<span data-ttu-id="62049-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="62049-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="62049-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="62049-190">The publishing state for the app.</span></span> <span data-ttu-id="62049-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="62049-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="62049-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="62049-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="62049-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="62049-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="62049-194">appAvailability</span></span>|[<span data-ttu-id="62049-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="62049-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="62049-196">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="62049-196">The Application's availability.</span></span> <span data-ttu-id="62049-197">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="62049-198">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="62049-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="62049-199">version</span><span class="sxs-lookup"><span data-stu-id="62049-199">version</span></span>|<span data-ttu-id="62049-200">String</span><span class="sxs-lookup"><span data-stu-id="62049-200">String</span></span>|<span data-ttu-id="62049-201">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="62049-201">The Application's version.</span></span> <span data-ttu-id="62049-202">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="62049-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="62049-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="62049-203">committedContentVersion</span></span>|<span data-ttu-id="62049-204">String</span><span class="sxs-lookup"><span data-stu-id="62049-204">String</span></span>|<span data-ttu-id="62049-205">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="62049-205">The internal committed content version.</span></span> <span data-ttu-id="62049-206">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="62049-207">fileName</span><span class="sxs-lookup"><span data-stu-id="62049-207">fileName</span></span>|<span data-ttu-id="62049-208">String</span><span class="sxs-lookup"><span data-stu-id="62049-208">String</span></span>|<span data-ttu-id="62049-209">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="62049-209">The name of the main Lob application file.</span></span> <span data-ttu-id="62049-210">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="62049-211">size</span><span class="sxs-lookup"><span data-stu-id="62049-211">size</span></span>|<span data-ttu-id="62049-212">Int64</span><span class="sxs-lookup"><span data-stu-id="62049-212">Int64</span></span>|<span data-ttu-id="62049-213">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="62049-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="62049-214">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="62049-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="62049-215">packageId</span><span class="sxs-lookup"><span data-stu-id="62049-215">packageId</span></span>|<span data-ttu-id="62049-216">String</span><span class="sxs-lookup"><span data-stu-id="62049-216">String</span></span>|<span data-ttu-id="62049-217">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="62049-217">The package identifier.</span></span>|
|<span data-ttu-id="62049-218">identityName</span><span class="sxs-lookup"><span data-stu-id="62049-218">identityName</span></span>|<span data-ttu-id="62049-219">String</span><span class="sxs-lookup"><span data-stu-id="62049-219">String</span></span>|<span data-ttu-id="62049-220">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="62049-220">The Identity Name.</span></span>|
|<span data-ttu-id="62049-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="62049-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="62049-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="62049-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="62049-223">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="62049-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="62049-224">versionName</span><span class="sxs-lookup"><span data-stu-id="62049-224">versionName</span></span>|<span data-ttu-id="62049-225">String</span><span class="sxs-lookup"><span data-stu-id="62049-225">String</span></span>|<span data-ttu-id="62049-226">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="62049-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="62049-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="62049-227">versionCode</span></span>|<span data-ttu-id="62049-228">String</span><span class="sxs-lookup"><span data-stu-id="62049-228">String</span></span>|<span data-ttu-id="62049-229">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="62049-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="62049-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="62049-230">identityVersion</span></span>|<span data-ttu-id="62049-231">String</span><span class="sxs-lookup"><span data-stu-id="62049-231">String</span></span>|<span data-ttu-id="62049-232">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="62049-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="62049-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="62049-233">Response</span></span>
<span data-ttu-id="62049-234">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62049-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62049-235">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62049-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="62049-236">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62049-236">Request</span></span>
<span data-ttu-id="62049-237">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62049-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1384

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="62049-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="62049-238">Response</span></span>
<span data-ttu-id="62049-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62049-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1551

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
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





