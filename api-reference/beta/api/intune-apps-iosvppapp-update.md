---
title: iosVppApp aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0ac3ad93fa6847ce62b6710286fc6eec977c66d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819509"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="b099e-103">iosVppApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b099e-103">Update iosVppApp</span></span>

> <span data-ttu-id="b099e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b099e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b099e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b099e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b099e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b099e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b099e-107">Aktualisiert die Eigenschaften von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b099e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b099e-108">Prerequisites</span></span>
<span data-ttu-id="b099e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b099e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b099e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b099e-111">Permission type</span></span>|<span data-ttu-id="b099e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b099e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b099e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b099e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b099e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b099e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b099e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b099e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b099e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b099e-116">Not supported.</span></span>|
|<span data-ttu-id="b099e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b099e-117">Application</span></span>|<span data-ttu-id="b099e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b099e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b099e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b099e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b099e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b099e-120">Request headers</span></span>
|<span data-ttu-id="b099e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b099e-121">Header</span></span>|<span data-ttu-id="b099e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b099e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b099e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b099e-123">Authorization</span></span>|<span data-ttu-id="b099e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b099e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b099e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b099e-125">Accept</span></span>|<span data-ttu-id="b099e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b099e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b099e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b099e-127">Request body</span></span>
<span data-ttu-id="b099e-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b099e-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="b099e-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosVppApp](../resources/intune-apps-iosvppapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b099e-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="b099e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b099e-130">Property</span></span>|<span data-ttu-id="b099e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b099e-131">Type</span></span>|<span data-ttu-id="b099e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b099e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b099e-133">id</span><span class="sxs-lookup"><span data-stu-id="b099e-133">id</span></span>|<span data-ttu-id="b099e-134">String</span><span class="sxs-lookup"><span data-stu-id="b099e-134">String</span></span>|<span data-ttu-id="b099e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b099e-135">Key of the entity.</span></span> <span data-ttu-id="b099e-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b099e-137">displayName</span></span>|<span data-ttu-id="b099e-138">String</span><span class="sxs-lookup"><span data-stu-id="b099e-138">String</span></span>|<span data-ttu-id="b099e-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b099e-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-141">description</span><span class="sxs-lookup"><span data-stu-id="b099e-141">description</span></span>|<span data-ttu-id="b099e-142">String</span><span class="sxs-lookup"><span data-stu-id="b099e-142">String</span></span>|<span data-ttu-id="b099e-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-143">The description of the app.</span></span> <span data-ttu-id="b099e-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b099e-145">publisher</span></span>|<span data-ttu-id="b099e-146">String</span><span class="sxs-lookup"><span data-stu-id="b099e-146">String</span></span>|<span data-ttu-id="b099e-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-147">The publisher of the app.</span></span> <span data-ttu-id="b099e-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b099e-149">largeIcon</span></span>|[<span data-ttu-id="b099e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b099e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b099e-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b099e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b099e-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b099e-153">createdDateTime</span></span>|<span data-ttu-id="b099e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b099e-154">DateTimeOffset</span></span>|<span data-ttu-id="b099e-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-155">The date and time the app was created.</span></span> <span data-ttu-id="b099e-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b099e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b099e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b099e-158">DateTimeOffset</span></span>|<span data-ttu-id="b099e-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b099e-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b099e-161">isFeatured</span></span>|<span data-ttu-id="b099e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b099e-162">Boolean</span></span>|<span data-ttu-id="b099e-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b099e-164">privacyInformationUrl</span></span>|<span data-ttu-id="b099e-165">String</span><span class="sxs-lookup"><span data-stu-id="b099e-165">String</span></span>|<span data-ttu-id="b099e-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="b099e-166">The privacy statement Url.</span></span> <span data-ttu-id="b099e-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b099e-168">informationUrl</span></span>|<span data-ttu-id="b099e-169">String</span><span class="sxs-lookup"><span data-stu-id="b099e-169">String</span></span>|<span data-ttu-id="b099e-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="b099e-170">The more information Url.</span></span> <span data-ttu-id="b099e-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-172">owner</span><span class="sxs-lookup"><span data-stu-id="b099e-172">owner</span></span>|<span data-ttu-id="b099e-173">String</span><span class="sxs-lookup"><span data-stu-id="b099e-173">String</span></span>|<span data-ttu-id="b099e-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-174">The owner of the app.</span></span> <span data-ttu-id="b099e-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-176">developer</span><span class="sxs-lookup"><span data-stu-id="b099e-176">developer</span></span>|<span data-ttu-id="b099e-177">String</span><span class="sxs-lookup"><span data-stu-id="b099e-177">String</span></span>|<span data-ttu-id="b099e-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-178">The developer of the app.</span></span> <span data-ttu-id="b099e-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-180">notes</span><span class="sxs-lookup"><span data-stu-id="b099e-180">notes</span></span>|<span data-ttu-id="b099e-181">String</span><span class="sxs-lookup"><span data-stu-id="b099e-181">String</span></span>|<span data-ttu-id="b099e-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="b099e-182">Notes for the app.</span></span> <span data-ttu-id="b099e-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b099e-184">uploadState</span></span>|<span data-ttu-id="b099e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b099e-185">Int32</span></span>|<span data-ttu-id="b099e-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="b099e-186">The upload state.</span></span> <span data-ttu-id="b099e-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b099e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b099e-188">publishingState</span></span>|[<span data-ttu-id="b099e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b099e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b099e-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="b099e-190">The publishing state for the app.</span></span> <span data-ttu-id="b099e-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="b099e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b099e-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b099e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b099e-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="b099e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b099e-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b099e-194">usedLicenseCount</span></span>|<span data-ttu-id="b099e-195">Int32</span><span class="sxs-lookup"><span data-stu-id="b099e-195">Int32</span></span>|<span data-ttu-id="b099e-196">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b099e-196">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="b099e-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b099e-197">totalLicenseCount</span></span>|<span data-ttu-id="b099e-198">Int32</span><span class="sxs-lookup"><span data-stu-id="b099e-198">Int32</span></span>|<span data-ttu-id="b099e-199">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="b099e-199">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="b099e-200">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b099e-200">releaseDateTime</span></span>|<span data-ttu-id="b099e-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b099e-201">DateTimeOffset</span></span>|<span data-ttu-id="b099e-202">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="b099e-202">The VPP application release date and time.</span></span>|
|<span data-ttu-id="b099e-203">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b099e-203">appStoreUrl</span></span>|<span data-ttu-id="b099e-204">String</span><span class="sxs-lookup"><span data-stu-id="b099e-204">String</span></span>|<span data-ttu-id="b099e-205">Store-URL</span><span class="sxs-lookup"><span data-stu-id="b099e-205">The store URL.</span></span>|
|<span data-ttu-id="b099e-206">licensingType</span><span class="sxs-lookup"><span data-stu-id="b099e-206">licensingType</span></span>|[<span data-ttu-id="b099e-207">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="b099e-207">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="b099e-208">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="b099e-208">The supported License Type.</span></span>|
|<span data-ttu-id="b099e-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b099e-209">applicableDeviceType</span></span>|[<span data-ttu-id="b099e-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b099e-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b099e-211">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="b099e-211">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="b099e-212">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b099e-212">vppTokenOrganizationName</span></span>|<span data-ttu-id="b099e-213">String</span><span class="sxs-lookup"><span data-stu-id="b099e-213">String</span></span>|<span data-ttu-id="b099e-214">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="b099e-214">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b099e-215">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b099e-215">vppTokenAccountType</span></span>|[<span data-ttu-id="b099e-216">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b099e-216">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="b099e-217">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b099e-217">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b099e-218">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="b099e-218">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="b099e-219">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="b099e-219">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b099e-220">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="b099e-220">vppTokenAppleId</span></span>|<span data-ttu-id="b099e-221">String</span><span class="sxs-lookup"><span data-stu-id="b099e-221">String</span></span>|<span data-ttu-id="b099e-222">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="b099e-222">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b099e-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="b099e-223">bundleId</span></span>|<span data-ttu-id="b099e-224">String</span><span class="sxs-lookup"><span data-stu-id="b099e-224">String</span></span>|<span data-ttu-id="b099e-225">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="b099e-225">The Identity Name.</span></span>|
|<span data-ttu-id="b099e-226">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b099e-226">vppTokenId</span></span>|<span data-ttu-id="b099e-227">String</span><span class="sxs-lookup"><span data-stu-id="b099e-227">String</span></span>|<span data-ttu-id="b099e-228">Bezeichner des Tokens VPP diese app zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="b099e-228">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="b099e-229">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="b099e-229">revokeLicenseActionResults</span></span>|<span data-ttu-id="b099e-230">[IosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b099e-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="b099e-231">Ergebnisse der widerrufen diese app-Lizenz Aktionen.</span><span class="sxs-lookup"><span data-stu-id="b099e-231">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="b099e-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="b099e-232">Response</span></span>
<span data-ttu-id="b099e-233">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b099e-233">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b099e-234">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b099e-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="b099e-235">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b099e-235">Request</span></span>
<span data-ttu-id="b099e-236">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b099e-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1903

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
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
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b099e-237">Antwort</span><span class="sxs-lookup"><span data-stu-id="b099e-237">Response</span></span>
<span data-ttu-id="b099e-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b099e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2059

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
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
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
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```





