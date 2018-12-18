---
title: iosVppApp aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs iosVppApp.
author: tfitzmac
ms.openlocfilehash: 05da16de7fc9d9cf5c556fd48f29d327bd6cd6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348006"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="000a5-103">iosVppApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="000a5-103">Update iosVppApp</span></span>

> <span data-ttu-id="000a5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="000a5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="000a5-105">Aktualisiert die Eigenschaften von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="000a5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="000a5-106">Prerequisites</span></span>
<span data-ttu-id="000a5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="000a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="000a5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="000a5-109">Permission type</span></span>|<span data-ttu-id="000a5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="000a5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="000a5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="000a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="000a5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="000a5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="000a5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="000a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="000a5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="000a5-114">Not supported.</span></span>|
|<span data-ttu-id="000a5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="000a5-115">Application</span></span>|<span data-ttu-id="000a5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="000a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="000a5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="000a5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="000a5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="000a5-118">Request headers</span></span>
|<span data-ttu-id="000a5-119">Header</span><span class="sxs-lookup"><span data-stu-id="000a5-119">Header</span></span>|<span data-ttu-id="000a5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="000a5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="000a5-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="000a5-121">Authorization</span></span>|<span data-ttu-id="000a5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="000a5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="000a5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="000a5-123">Accept</span></span>|<span data-ttu-id="000a5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="000a5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="000a5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="000a5-125">Request body</span></span>
<span data-ttu-id="000a5-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="000a5-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="000a5-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosVppApp](../resources/intune-apps-iosvppapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="000a5-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="000a5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="000a5-128">Property</span></span>|<span data-ttu-id="000a5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="000a5-129">Type</span></span>|<span data-ttu-id="000a5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="000a5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="000a5-131">id</span><span class="sxs-lookup"><span data-stu-id="000a5-131">id</span></span>|<span data-ttu-id="000a5-132">String</span><span class="sxs-lookup"><span data-stu-id="000a5-132">String</span></span>|<span data-ttu-id="000a5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="000a5-133">Key of the entity.</span></span> <span data-ttu-id="000a5-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="000a5-135">displayName</span></span>|<span data-ttu-id="000a5-136">String</span><span class="sxs-lookup"><span data-stu-id="000a5-136">String</span></span>|<span data-ttu-id="000a5-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="000a5-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-139">description</span><span class="sxs-lookup"><span data-stu-id="000a5-139">description</span></span>|<span data-ttu-id="000a5-140">String</span><span class="sxs-lookup"><span data-stu-id="000a5-140">String</span></span>|<span data-ttu-id="000a5-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-141">The description of the app.</span></span> <span data-ttu-id="000a5-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-143">publisher</span><span class="sxs-lookup"><span data-stu-id="000a5-143">publisher</span></span>|<span data-ttu-id="000a5-144">String</span><span class="sxs-lookup"><span data-stu-id="000a5-144">String</span></span>|<span data-ttu-id="000a5-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-145">The publisher of the app.</span></span> <span data-ttu-id="000a5-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="000a5-147">largeIcon</span></span>|[<span data-ttu-id="000a5-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="000a5-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="000a5-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="000a5-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="000a5-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="000a5-151">createdDateTime</span></span>|<span data-ttu-id="000a5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="000a5-152">DateTimeOffset</span></span>|<span data-ttu-id="000a5-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-153">The date and time the app was created.</span></span> <span data-ttu-id="000a5-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="000a5-155">lastModifiedDateTime</span></span>|<span data-ttu-id="000a5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="000a5-156">DateTimeOffset</span></span>|<span data-ttu-id="000a5-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-157">The date and time the app was last modified.</span></span> <span data-ttu-id="000a5-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="000a5-159">isFeatured</span></span>|<span data-ttu-id="000a5-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="000a5-160">Boolean</span></span>|<span data-ttu-id="000a5-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="000a5-162">privacyInformationUrl</span></span>|<span data-ttu-id="000a5-163">String</span><span class="sxs-lookup"><span data-stu-id="000a5-163">String</span></span>|<span data-ttu-id="000a5-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="000a5-164">The privacy statement Url.</span></span> <span data-ttu-id="000a5-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="000a5-166">informationUrl</span></span>|<span data-ttu-id="000a5-167">String</span><span class="sxs-lookup"><span data-stu-id="000a5-167">String</span></span>|<span data-ttu-id="000a5-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="000a5-168">The more information Url.</span></span> <span data-ttu-id="000a5-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-170">owner</span><span class="sxs-lookup"><span data-stu-id="000a5-170">owner</span></span>|<span data-ttu-id="000a5-171">String</span><span class="sxs-lookup"><span data-stu-id="000a5-171">String</span></span>|<span data-ttu-id="000a5-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-172">The owner of the app.</span></span> <span data-ttu-id="000a5-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-174">developer</span><span class="sxs-lookup"><span data-stu-id="000a5-174">developer</span></span>|<span data-ttu-id="000a5-175">String</span><span class="sxs-lookup"><span data-stu-id="000a5-175">String</span></span>|<span data-ttu-id="000a5-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-176">The developer of the app.</span></span> <span data-ttu-id="000a5-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-178">notes</span><span class="sxs-lookup"><span data-stu-id="000a5-178">notes</span></span>|<span data-ttu-id="000a5-179">String</span><span class="sxs-lookup"><span data-stu-id="000a5-179">String</span></span>|<span data-ttu-id="000a5-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="000a5-180">Notes for the app.</span></span> <span data-ttu-id="000a5-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="000a5-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="000a5-182">publishingState</span></span>|[<span data-ttu-id="000a5-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="000a5-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="000a5-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="000a5-184">The publishing state for the app.</span></span> <span data-ttu-id="000a5-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="000a5-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="000a5-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="000a5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="000a5-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="000a5-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="000a5-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="000a5-188">usedLicenseCount</span></span>|<span data-ttu-id="000a5-189">Int32</span><span class="sxs-lookup"><span data-stu-id="000a5-189">Int32</span></span>|<span data-ttu-id="000a5-190">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="000a5-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="000a5-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="000a5-191">totalLicenseCount</span></span>|<span data-ttu-id="000a5-192">Int32</span><span class="sxs-lookup"><span data-stu-id="000a5-192">Int32</span></span>|<span data-ttu-id="000a5-193">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="000a5-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="000a5-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="000a5-194">releaseDateTime</span></span>|<span data-ttu-id="000a5-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="000a5-195">DateTimeOffset</span></span>|<span data-ttu-id="000a5-196">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="000a5-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="000a5-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="000a5-197">appStoreUrl</span></span>|<span data-ttu-id="000a5-198">String</span><span class="sxs-lookup"><span data-stu-id="000a5-198">String</span></span>|<span data-ttu-id="000a5-199">Store-URL</span><span class="sxs-lookup"><span data-stu-id="000a5-199">The store URL.</span></span>|
|<span data-ttu-id="000a5-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="000a5-200">licensingType</span></span>|[<span data-ttu-id="000a5-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="000a5-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="000a5-202">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="000a5-202">The supported License Type.</span></span>|
|<span data-ttu-id="000a5-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="000a5-203">applicableDeviceType</span></span>|[<span data-ttu-id="000a5-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="000a5-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="000a5-205">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="000a5-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="000a5-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="000a5-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="000a5-207">String</span><span class="sxs-lookup"><span data-stu-id="000a5-207">String</span></span>|<span data-ttu-id="000a5-208">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="000a5-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="000a5-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="000a5-209">vppTokenAccountType</span></span>|[<span data-ttu-id="000a5-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="000a5-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="000a5-211">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="000a5-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="000a5-212">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="000a5-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="000a5-213">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="000a5-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="000a5-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="000a5-214">vppTokenAppleId</span></span>|<span data-ttu-id="000a5-215">String</span><span class="sxs-lookup"><span data-stu-id="000a5-215">String</span></span>|<span data-ttu-id="000a5-216">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="000a5-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="000a5-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="000a5-217">bundleId</span></span>|<span data-ttu-id="000a5-218">String</span><span class="sxs-lookup"><span data-stu-id="000a5-218">String</span></span>|<span data-ttu-id="000a5-219">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="000a5-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="000a5-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="000a5-220">Response</span></span>
<span data-ttu-id="000a5-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="000a5-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="000a5-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="000a5-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="000a5-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="000a5-223">Request</span></span>
<span data-ttu-id="000a5-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="000a5-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="000a5-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="000a5-225">Response</span></span>
<span data-ttu-id="000a5-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="000a5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



