---
title: AndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 901de0d479ee21df3f38e896c55fcdd283908cfd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955541"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="dd276-103">AndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dd276-103">Update androidLobApp</span></span>

> <span data-ttu-id="dd276-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd276-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd276-105">Aktualisieren der Eigenschaften eines [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd276-105">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd276-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd276-106">Prerequisites</span></span>
<span data-ttu-id="dd276-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd276-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd276-109">Permission type</span></span>|<span data-ttu-id="dd276-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd276-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd276-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd276-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd276-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd276-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd276-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd276-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd276-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd276-114">Not supported.</span></span>|
|<span data-ttu-id="dd276-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd276-115">Application</span></span>|<span data-ttu-id="dd276-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd276-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd276-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd276-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="dd276-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd276-118">Request headers</span></span>
|<span data-ttu-id="dd276-119">Header</span><span class="sxs-lookup"><span data-stu-id="dd276-119">Header</span></span>|<span data-ttu-id="dd276-120">Wert</span><span class="sxs-lookup"><span data-stu-id="dd276-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd276-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd276-121">Authorization</span></span>|<span data-ttu-id="dd276-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd276-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd276-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd276-123">Accept</span></span>|<span data-ttu-id="dd276-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd276-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd276-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd276-125">Request body</span></span>
<span data-ttu-id="dd276-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidLobApp](../resources/intune-apps-androidlobapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="dd276-126">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="dd276-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidLobApp](../resources/intune-apps-androidlobapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="dd276-127">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="dd276-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd276-128">Property</span></span>|<span data-ttu-id="dd276-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dd276-129">Type</span></span>|<span data-ttu-id="dd276-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd276-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd276-131">id</span><span class="sxs-lookup"><span data-stu-id="dd276-131">id</span></span>|<span data-ttu-id="dd276-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-132">String</span></span>|<span data-ttu-id="dd276-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dd276-133">Key of the entity.</span></span> <span data-ttu-id="dd276-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dd276-135">displayName</span></span>|<span data-ttu-id="dd276-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-136">String</span></span>|<span data-ttu-id="dd276-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dd276-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-139">description</span><span class="sxs-lookup"><span data-stu-id="dd276-139">description</span></span>|<span data-ttu-id="dd276-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-140">String</span></span>|<span data-ttu-id="dd276-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-141">The description of the app.</span></span> <span data-ttu-id="dd276-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-143">publisher</span><span class="sxs-lookup"><span data-stu-id="dd276-143">publisher</span></span>|<span data-ttu-id="dd276-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-144">String</span></span>|<span data-ttu-id="dd276-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-145">The publisher of the app.</span></span> <span data-ttu-id="dd276-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dd276-147">largeIcon</span></span>|[<span data-ttu-id="dd276-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dd276-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dd276-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="dd276-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dd276-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd276-151">createdDateTime</span></span>|<span data-ttu-id="dd276-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd276-152">DateTimeOffset</span></span>|<span data-ttu-id="dd276-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-153">The date and time the app was created.</span></span> <span data-ttu-id="dd276-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd276-155">lastModifiedDateTime</span></span>|<span data-ttu-id="dd276-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd276-156">DateTimeOffset</span></span>|<span data-ttu-id="dd276-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-157">The date and time the app was last modified.</span></span> <span data-ttu-id="dd276-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dd276-159">isFeatured</span></span>|<span data-ttu-id="dd276-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd276-160">Boolean</span></span>|<span data-ttu-id="dd276-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dd276-162">privacyInformationUrl</span></span>|<span data-ttu-id="dd276-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-163">String</span></span>|<span data-ttu-id="dd276-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="dd276-164">The privacy statement Url.</span></span> <span data-ttu-id="dd276-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dd276-166">informationUrl</span></span>|<span data-ttu-id="dd276-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-167">String</span></span>|<span data-ttu-id="dd276-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="dd276-168">The more information Url.</span></span> <span data-ttu-id="dd276-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-170">owner</span><span class="sxs-lookup"><span data-stu-id="dd276-170">owner</span></span>|<span data-ttu-id="dd276-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-171">String</span></span>|<span data-ttu-id="dd276-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-172">The owner of the app.</span></span> <span data-ttu-id="dd276-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-174">developer</span><span class="sxs-lookup"><span data-stu-id="dd276-174">developer</span></span>|<span data-ttu-id="dd276-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-175">String</span></span>|<span data-ttu-id="dd276-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-176">The developer of the app.</span></span> <span data-ttu-id="dd276-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-178">notes</span><span class="sxs-lookup"><span data-stu-id="dd276-178">notes</span></span>|<span data-ttu-id="dd276-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-179">String</span></span>|<span data-ttu-id="dd276-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="dd276-180">Notes for the app.</span></span> <span data-ttu-id="dd276-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd276-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="dd276-182">publishingState</span></span>|[<span data-ttu-id="dd276-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dd276-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dd276-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="dd276-184">The publishing state for the app.</span></span> <span data-ttu-id="dd276-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="dd276-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dd276-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dd276-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="dd276-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dd276-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dd276-188">committedContentVersion</span></span>|<span data-ttu-id="dd276-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-189">String</span></span>|<span data-ttu-id="dd276-190">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="dd276-190">The internal committed content version.</span></span> <span data-ttu-id="dd276-191">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dd276-192">fileName</span><span class="sxs-lookup"><span data-stu-id="dd276-192">fileName</span></span>|<span data-ttu-id="dd276-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-193">String</span></span>|<span data-ttu-id="dd276-194">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="dd276-194">The name of the main Lob application file.</span></span> <span data-ttu-id="dd276-195">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dd276-196">size</span><span class="sxs-lookup"><span data-stu-id="dd276-196">size</span></span>|<span data-ttu-id="dd276-197">Int64</span><span class="sxs-lookup"><span data-stu-id="dd276-197">Int64</span></span>|<span data-ttu-id="dd276-198">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="dd276-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="dd276-199">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd276-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dd276-200">packageId</span><span class="sxs-lookup"><span data-stu-id="dd276-200">packageId</span></span>|<span data-ttu-id="dd276-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-201">String</span></span>|<span data-ttu-id="dd276-202">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="dd276-202">The package identifier.</span></span>|
|<span data-ttu-id="dd276-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd276-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dd276-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd276-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="dd276-205">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="dd276-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dd276-206">versionName</span><span class="sxs-lookup"><span data-stu-id="dd276-206">versionName</span></span>|<span data-ttu-id="dd276-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-207">String</span></span>|<span data-ttu-id="dd276-208">Der Versionsname der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="dd276-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dd276-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="dd276-209">versionCode</span></span>|<span data-ttu-id="dd276-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd276-210">String</span></span>|<span data-ttu-id="dd276-211">Der Versionscode der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="dd276-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="dd276-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd276-212">Response</span></span>
<span data-ttu-id="dd276-213">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd276-213">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd276-214">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd276-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd276-215">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd276-215">Request</span></span>
<span data-ttu-id="dd276-216">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd276-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="dd276-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd276-217">Response</span></span>
<span data-ttu-id="dd276-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd276-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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



