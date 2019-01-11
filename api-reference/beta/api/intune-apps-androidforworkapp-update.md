---
title: AndroidForWorkApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 757a095733aeb69cf3b92027c1927b09f929cd71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824087"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="69c0d-103">AndroidForWorkApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="69c0d-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="69c0d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69c0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69c0d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69c0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69c0d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69c0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69c0d-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="69c0d-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69c0d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="69c0d-108">Prerequisites</span></span>
<span data-ttu-id="69c0d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69c0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69c0d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69c0d-111">Permission type</span></span>|<span data-ttu-id="69c0d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69c0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69c0d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69c0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69c0d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c0d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69c0d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69c0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69c0d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69c0d-116">Not supported.</span></span>|
|<span data-ttu-id="69c0d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69c0d-117">Application</span></span>|<span data-ttu-id="69c0d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69c0d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69c0d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69c0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="69c0d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69c0d-120">Request headers</span></span>
|<span data-ttu-id="69c0d-121">Header</span><span class="sxs-lookup"><span data-stu-id="69c0d-121">Header</span></span>|<span data-ttu-id="69c0d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="69c0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69c0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69c0d-123">Authorization</span></span>|<span data-ttu-id="69c0d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="69c0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69c0d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="69c0d-125">Accept</span></span>|<span data-ttu-id="69c0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69c0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69c0d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69c0d-127">Request body</span></span>
<span data-ttu-id="69c0d-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="69c0d-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="69c0d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="69c0d-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="69c0d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69c0d-130">Property</span></span>|<span data-ttu-id="69c0d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="69c0d-131">Type</span></span>|<span data-ttu-id="69c0d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69c0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69c0d-133">id</span><span class="sxs-lookup"><span data-stu-id="69c0d-133">id</span></span>|<span data-ttu-id="69c0d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-134">String</span></span>|<span data-ttu-id="69c0d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="69c0d-135">Key of the entity.</span></span> <span data-ttu-id="69c0d-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="69c0d-137">displayName</span></span>|<span data-ttu-id="69c0d-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-138">String</span></span>|<span data-ttu-id="69c0d-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="69c0d-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-141">description</span><span class="sxs-lookup"><span data-stu-id="69c0d-141">description</span></span>|<span data-ttu-id="69c0d-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-142">String</span></span>|<span data-ttu-id="69c0d-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-143">The description of the app.</span></span> <span data-ttu-id="69c0d-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="69c0d-145">publisher</span></span>|<span data-ttu-id="69c0d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-146">String</span></span>|<span data-ttu-id="69c0d-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-147">The publisher of the app.</span></span> <span data-ttu-id="69c0d-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="69c0d-149">largeIcon</span></span>|[<span data-ttu-id="69c0d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="69c0d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="69c0d-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="69c0d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="69c0d-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69c0d-153">createdDateTime</span></span>|<span data-ttu-id="69c0d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c0d-154">DateTimeOffset</span></span>|<span data-ttu-id="69c0d-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-155">The date and time the app was created.</span></span> <span data-ttu-id="69c0d-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69c0d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="69c0d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c0d-158">DateTimeOffset</span></span>|<span data-ttu-id="69c0d-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="69c0d-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="69c0d-161">isFeatured</span></span>|<span data-ttu-id="69c0d-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="69c0d-162">Boolean</span></span>|<span data-ttu-id="69c0d-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="69c0d-164">privacyInformationUrl</span></span>|<span data-ttu-id="69c0d-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-165">String</span></span>|<span data-ttu-id="69c0d-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="69c0d-166">The privacy statement Url.</span></span> <span data-ttu-id="69c0d-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="69c0d-168">informationUrl</span></span>|<span data-ttu-id="69c0d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-169">String</span></span>|<span data-ttu-id="69c0d-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="69c0d-170">The more information Url.</span></span> <span data-ttu-id="69c0d-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-172">owner</span><span class="sxs-lookup"><span data-stu-id="69c0d-172">owner</span></span>|<span data-ttu-id="69c0d-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-173">String</span></span>|<span data-ttu-id="69c0d-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-174">The owner of the app.</span></span> <span data-ttu-id="69c0d-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-176">developer</span><span class="sxs-lookup"><span data-stu-id="69c0d-176">developer</span></span>|<span data-ttu-id="69c0d-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-177">String</span></span>|<span data-ttu-id="69c0d-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-178">The developer of the app.</span></span> <span data-ttu-id="69c0d-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-180">notes</span><span class="sxs-lookup"><span data-stu-id="69c0d-180">notes</span></span>|<span data-ttu-id="69c0d-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-181">String</span></span>|<span data-ttu-id="69c0d-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-182">Notes for the app.</span></span> <span data-ttu-id="69c0d-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="69c0d-184">uploadState</span></span>|<span data-ttu-id="69c0d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="69c0d-185">Int32</span></span>|<span data-ttu-id="69c0d-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="69c0d-186">The upload state.</span></span> <span data-ttu-id="69c0d-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69c0d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="69c0d-188">publishingState</span></span>|[<span data-ttu-id="69c0d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="69c0d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="69c0d-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="69c0d-190">The publishing state for the app.</span></span> <span data-ttu-id="69c0d-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="69c0d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="69c0d-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="69c0d-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="69c0d-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="69c0d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="69c0d-194">packageId</span><span class="sxs-lookup"><span data-stu-id="69c0d-194">packageId</span></span>|<span data-ttu-id="69c0d-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-195">String</span></span>|<span data-ttu-id="69c0d-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="69c0d-196">The package identifier.</span></span>|
|<span data-ttu-id="69c0d-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="69c0d-197">appIdentifier</span></span>|<span data-ttu-id="69c0d-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-198">String</span></span>|<span data-ttu-id="69c0d-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="69c0d-199">The Identity Name.</span></span>|
|<span data-ttu-id="69c0d-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="69c0d-200">usedLicenseCount</span></span>|<span data-ttu-id="69c0d-201">Int32</span><span class="sxs-lookup"><span data-stu-id="69c0d-201">Int32</span></span>|<span data-ttu-id="69c0d-202">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="69c0d-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="69c0d-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="69c0d-203">totalLicenseCount</span></span>|<span data-ttu-id="69c0d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="69c0d-204">Int32</span></span>|<span data-ttu-id="69c0d-205">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="69c0d-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="69c0d-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="69c0d-206">appStoreUrl</span></span>|<span data-ttu-id="69c0d-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69c0d-207">String</span></span>|<span data-ttu-id="69c0d-208">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="69c0d-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="69c0d-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="69c0d-209">Response</span></span>
<span data-ttu-id="69c0d-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="69c0d-210">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69c0d-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69c0d-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="69c0d-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69c0d-212">Request</span></span>
<span data-ttu-id="69c0d-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69c0d-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 799

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="69c0d-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="69c0d-214">Response</span></span>
<span data-ttu-id="69c0d-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69c0d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 963

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





