---
title: managedAndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a39ba38b9ff8a2e42c024c85710ffba844158319
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967252"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="22aa1-103">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="22aa1-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="22aa1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22aa1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22aa1-105">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="22aa1-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22aa1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22aa1-106">Prerequisites</span></span>
<span data-ttu-id="22aa1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22aa1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22aa1-109">Permission type</span></span>|<span data-ttu-id="22aa1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22aa1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22aa1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22aa1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22aa1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22aa1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22aa1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22aa1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22aa1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22aa1-114">Not supported.</span></span>|
|<span data-ttu-id="22aa1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22aa1-115">Application</span></span>|<span data-ttu-id="22aa1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22aa1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22aa1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22aa1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="22aa1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22aa1-118">Request headers</span></span>
|<span data-ttu-id="22aa1-119">Header</span><span class="sxs-lookup"><span data-stu-id="22aa1-119">Header</span></span>|<span data-ttu-id="22aa1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="22aa1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22aa1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="22aa1-121">Authorization</span></span>|<span data-ttu-id="22aa1-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22aa1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22aa1-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="22aa1-123">Accept</span></span>|<span data-ttu-id="22aa1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22aa1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22aa1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22aa1-125">Request body</span></span>
<span data-ttu-id="22aa1-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="22aa1-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="22aa1-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="22aa1-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="22aa1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22aa1-128">Property</span></span>|<span data-ttu-id="22aa1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="22aa1-129">Type</span></span>|<span data-ttu-id="22aa1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22aa1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22aa1-131">id</span><span class="sxs-lookup"><span data-stu-id="22aa1-131">id</span></span>|<span data-ttu-id="22aa1-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-132">String</span></span>|<span data-ttu-id="22aa1-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="22aa1-133">Key of the entity.</span></span> <span data-ttu-id="22aa1-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="22aa1-135">displayName</span></span>|<span data-ttu-id="22aa1-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-136">String</span></span>|<span data-ttu-id="22aa1-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="22aa1-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-139">description</span><span class="sxs-lookup"><span data-stu-id="22aa1-139">description</span></span>|<span data-ttu-id="22aa1-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-140">String</span></span>|<span data-ttu-id="22aa1-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-141">The description of the app.</span></span> <span data-ttu-id="22aa1-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-143">publisher</span><span class="sxs-lookup"><span data-stu-id="22aa1-143">publisher</span></span>|<span data-ttu-id="22aa1-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-144">String</span></span>|<span data-ttu-id="22aa1-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-145">The publisher of the app.</span></span> <span data-ttu-id="22aa1-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="22aa1-147">largeIcon</span></span>|[<span data-ttu-id="22aa1-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="22aa1-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="22aa1-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="22aa1-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="22aa1-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22aa1-151">createdDateTime</span></span>|<span data-ttu-id="22aa1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22aa1-152">DateTimeOffset</span></span>|<span data-ttu-id="22aa1-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-153">The date and time the app was created.</span></span> <span data-ttu-id="22aa1-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22aa1-155">lastModifiedDateTime</span></span>|<span data-ttu-id="22aa1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22aa1-156">DateTimeOffset</span></span>|<span data-ttu-id="22aa1-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-157">The date and time the app was last modified.</span></span> <span data-ttu-id="22aa1-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="22aa1-159">isFeatured</span></span>|<span data-ttu-id="22aa1-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="22aa1-160">Boolean</span></span>|<span data-ttu-id="22aa1-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="22aa1-162">privacyInformationUrl</span></span>|<span data-ttu-id="22aa1-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-163">String</span></span>|<span data-ttu-id="22aa1-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="22aa1-164">The privacy statement Url.</span></span> <span data-ttu-id="22aa1-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="22aa1-166">informationUrl</span></span>|<span data-ttu-id="22aa1-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-167">String</span></span>|<span data-ttu-id="22aa1-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="22aa1-168">The more information Url.</span></span> <span data-ttu-id="22aa1-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-170">owner</span><span class="sxs-lookup"><span data-stu-id="22aa1-170">owner</span></span>|<span data-ttu-id="22aa1-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-171">String</span></span>|<span data-ttu-id="22aa1-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-172">The owner of the app.</span></span> <span data-ttu-id="22aa1-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-174">developer</span><span class="sxs-lookup"><span data-stu-id="22aa1-174">developer</span></span>|<span data-ttu-id="22aa1-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-175">String</span></span>|<span data-ttu-id="22aa1-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-176">The developer of the app.</span></span> <span data-ttu-id="22aa1-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-178">notes</span><span class="sxs-lookup"><span data-stu-id="22aa1-178">notes</span></span>|<span data-ttu-id="22aa1-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-179">String</span></span>|<span data-ttu-id="22aa1-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-180">Notes for the app.</span></span> <span data-ttu-id="22aa1-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22aa1-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="22aa1-182">publishingState</span></span>|[<span data-ttu-id="22aa1-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="22aa1-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="22aa1-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-184">The publishing state for the app.</span></span> <span data-ttu-id="22aa1-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="22aa1-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="22aa1-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="22aa1-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="22aa1-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="22aa1-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="22aa1-188">appAvailability</span></span>|[<span data-ttu-id="22aa1-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="22aa1-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="22aa1-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="22aa1-190">The Application's availability.</span></span> <span data-ttu-id="22aa1-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="22aa1-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="22aa1-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="22aa1-193">version</span><span class="sxs-lookup"><span data-stu-id="22aa1-193">version</span></span>|<span data-ttu-id="22aa1-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-194">String</span></span>|<span data-ttu-id="22aa1-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="22aa1-195">The Application's version.</span></span> <span data-ttu-id="22aa1-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="22aa1-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="22aa1-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="22aa1-197">committedContentVersion</span></span>|<span data-ttu-id="22aa1-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-198">String</span></span>|<span data-ttu-id="22aa1-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="22aa1-199">The internal committed content version.</span></span> <span data-ttu-id="22aa1-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="22aa1-201">fileName</span><span class="sxs-lookup"><span data-stu-id="22aa1-201">fileName</span></span>|<span data-ttu-id="22aa1-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-202">String</span></span>|<span data-ttu-id="22aa1-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="22aa1-203">The name of the main Lob application file.</span></span> <span data-ttu-id="22aa1-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="22aa1-205">size</span><span class="sxs-lookup"><span data-stu-id="22aa1-205">size</span></span>|<span data-ttu-id="22aa1-206">Int64</span><span class="sxs-lookup"><span data-stu-id="22aa1-206">Int64</span></span>|<span data-ttu-id="22aa1-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="22aa1-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="22aa1-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="22aa1-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="22aa1-209">packageId</span><span class="sxs-lookup"><span data-stu-id="22aa1-209">packageId</span></span>|<span data-ttu-id="22aa1-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-210">String</span></span>|<span data-ttu-id="22aa1-211">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="22aa1-211">The package identifier.</span></span>|
|<span data-ttu-id="22aa1-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22aa1-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="22aa1-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22aa1-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="22aa1-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="22aa1-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="22aa1-215">versionName</span><span class="sxs-lookup"><span data-stu-id="22aa1-215">versionName</span></span>|<span data-ttu-id="22aa1-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-216">String</span></span>|<span data-ttu-id="22aa1-217">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="22aa1-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="22aa1-218">versionCode</span></span>|<span data-ttu-id="22aa1-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22aa1-219">String</span></span>|<span data-ttu-id="22aa1-220">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="22aa1-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="22aa1-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="22aa1-221">Response</span></span>
<span data-ttu-id="22aa1-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22aa1-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22aa1-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22aa1-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="22aa1-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22aa1-224">Request</span></span>
<span data-ttu-id="22aa1-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22aa1-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22aa1-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="22aa1-226">Response</span></span>
<span data-ttu-id="22aa1-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22aa1-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



