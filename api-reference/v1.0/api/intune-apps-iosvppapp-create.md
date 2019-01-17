---
title: Erstellen von „iosVppApp“
description: Erstellen eines neuen iosVppApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 562f9f87effc78ed1723042a3270592ad2d08206
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971354"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="62b50-103">Erstellen von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="62b50-103">Create iosVppApp</span></span>

> <span data-ttu-id="62b50-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="62b50-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62b50-105">Erstellen eines neuen [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="62b50-105">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62b50-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="62b50-106">Prerequisites</span></span>
<span data-ttu-id="62b50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62b50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62b50-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62b50-109">Permission type</span></span>|<span data-ttu-id="62b50-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62b50-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62b50-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62b50-111">Delegated (work or school account)</span></span>|<span data-ttu-id="62b50-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b50-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62b50-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62b50-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62b50-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62b50-114">Not supported.</span></span>|
|<span data-ttu-id="62b50-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62b50-115">Application</span></span>|<span data-ttu-id="62b50-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62b50-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62b50-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62b50-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="62b50-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62b50-118">Request headers</span></span>
|<span data-ttu-id="62b50-119">Header</span><span class="sxs-lookup"><span data-stu-id="62b50-119">Header</span></span>|<span data-ttu-id="62b50-120">Wert</span><span class="sxs-lookup"><span data-stu-id="62b50-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62b50-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62b50-121">Authorization</span></span>|<span data-ttu-id="62b50-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="62b50-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62b50-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="62b50-123">Accept</span></span>|<span data-ttu-id="62b50-124">application/json</span><span class="sxs-lookup"><span data-stu-id="62b50-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62b50-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62b50-125">Request body</span></span>
<span data-ttu-id="62b50-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="62b50-126">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="62b50-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="62b50-127">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="62b50-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62b50-128">Property</span></span>|<span data-ttu-id="62b50-129">Typ</span><span class="sxs-lookup"><span data-stu-id="62b50-129">Type</span></span>|<span data-ttu-id="62b50-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62b50-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b50-131">id</span><span class="sxs-lookup"><span data-stu-id="62b50-131">id</span></span>|<span data-ttu-id="62b50-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-132">String</span></span>|<span data-ttu-id="62b50-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="62b50-133">Key of the entity.</span></span> <span data-ttu-id="62b50-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-135">displayName</span><span class="sxs-lookup"><span data-stu-id="62b50-135">displayName</span></span>|<span data-ttu-id="62b50-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-136">String</span></span>|<span data-ttu-id="62b50-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="62b50-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-139">description</span><span class="sxs-lookup"><span data-stu-id="62b50-139">description</span></span>|<span data-ttu-id="62b50-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-140">String</span></span>|<span data-ttu-id="62b50-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-141">The description of the app.</span></span> <span data-ttu-id="62b50-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-143">publisher</span><span class="sxs-lookup"><span data-stu-id="62b50-143">publisher</span></span>|<span data-ttu-id="62b50-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-144">String</span></span>|<span data-ttu-id="62b50-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-145">The publisher of the app.</span></span> <span data-ttu-id="62b50-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="62b50-147">largeIcon</span></span>|[<span data-ttu-id="62b50-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="62b50-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="62b50-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="62b50-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="62b50-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62b50-151">createdDateTime</span></span>|<span data-ttu-id="62b50-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62b50-152">DateTimeOffset</span></span>|<span data-ttu-id="62b50-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-153">The date and time the app was created.</span></span> <span data-ttu-id="62b50-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62b50-155">lastModifiedDateTime</span></span>|<span data-ttu-id="62b50-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62b50-156">DateTimeOffset</span></span>|<span data-ttu-id="62b50-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-157">The date and time the app was last modified.</span></span> <span data-ttu-id="62b50-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="62b50-159">isFeatured</span></span>|<span data-ttu-id="62b50-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="62b50-160">Boolean</span></span>|<span data-ttu-id="62b50-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="62b50-162">privacyInformationUrl</span></span>|<span data-ttu-id="62b50-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-163">String</span></span>|<span data-ttu-id="62b50-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="62b50-164">The privacy statement Url.</span></span> <span data-ttu-id="62b50-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="62b50-166">informationUrl</span></span>|<span data-ttu-id="62b50-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-167">String</span></span>|<span data-ttu-id="62b50-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="62b50-168">The more information Url.</span></span> <span data-ttu-id="62b50-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-170">owner</span><span class="sxs-lookup"><span data-stu-id="62b50-170">owner</span></span>|<span data-ttu-id="62b50-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-171">String</span></span>|<span data-ttu-id="62b50-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-172">The owner of the app.</span></span> <span data-ttu-id="62b50-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-174">developer</span><span class="sxs-lookup"><span data-stu-id="62b50-174">developer</span></span>|<span data-ttu-id="62b50-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-175">String</span></span>|<span data-ttu-id="62b50-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-176">The developer of the app.</span></span> <span data-ttu-id="62b50-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-178">notes</span><span class="sxs-lookup"><span data-stu-id="62b50-178">notes</span></span>|<span data-ttu-id="62b50-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-179">String</span></span>|<span data-ttu-id="62b50-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="62b50-180">Notes for the app.</span></span> <span data-ttu-id="62b50-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62b50-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="62b50-182">publishingState</span></span>|[<span data-ttu-id="62b50-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="62b50-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="62b50-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="62b50-184">The publishing state for the app.</span></span> <span data-ttu-id="62b50-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="62b50-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="62b50-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62b50-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="62b50-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="62b50-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="62b50-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="62b50-188">usedLicenseCount</span></span>|<span data-ttu-id="62b50-189">Int32</span><span class="sxs-lookup"><span data-stu-id="62b50-189">Int32</span></span>|<span data-ttu-id="62b50-190">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="62b50-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="62b50-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="62b50-191">totalLicenseCount</span></span>|<span data-ttu-id="62b50-192">Int32</span><span class="sxs-lookup"><span data-stu-id="62b50-192">Int32</span></span>|<span data-ttu-id="62b50-193">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="62b50-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="62b50-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="62b50-194">releaseDateTime</span></span>|<span data-ttu-id="62b50-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62b50-195">DateTimeOffset</span></span>|<span data-ttu-id="62b50-196">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="62b50-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="62b50-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="62b50-197">appStoreUrl</span></span>|<span data-ttu-id="62b50-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-198">String</span></span>|<span data-ttu-id="62b50-199">Store-URL</span><span class="sxs-lookup"><span data-stu-id="62b50-199">The store URL.</span></span>|
|<span data-ttu-id="62b50-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="62b50-200">licensingType</span></span>|[<span data-ttu-id="62b50-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="62b50-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="62b50-202">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="62b50-202">The supported License Type.</span></span>|
|<span data-ttu-id="62b50-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="62b50-203">applicableDeviceType</span></span>|[<span data-ttu-id="62b50-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="62b50-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="62b50-205">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="62b50-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="62b50-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="62b50-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="62b50-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-207">String</span></span>|<span data-ttu-id="62b50-208">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="62b50-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="62b50-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="62b50-209">vppTokenAccountType</span></span>|[<span data-ttu-id="62b50-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="62b50-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="62b50-211">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="62b50-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="62b50-212">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="62b50-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="62b50-213">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="62b50-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="62b50-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="62b50-214">vppTokenAppleId</span></span>|<span data-ttu-id="62b50-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-215">String</span></span>|<span data-ttu-id="62b50-216">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="62b50-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="62b50-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="62b50-217">bundleId</span></span>|<span data-ttu-id="62b50-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62b50-218">String</span></span>|<span data-ttu-id="62b50-219">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="62b50-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="62b50-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="62b50-220">Response</span></span>
<span data-ttu-id="62b50-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62b50-221">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62b50-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62b50-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="62b50-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62b50-223">Request</span></span>
<span data-ttu-id="62b50-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62b50-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="62b50-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="62b50-225">Response</span></span>
<span data-ttu-id="62b50-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62b50-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



