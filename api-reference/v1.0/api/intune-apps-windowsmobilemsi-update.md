---
title: windowsMobileMSI aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windowsMobileMSI.
ms.openlocfilehash: a87c76413080b6c5daae828e5ed22e99be1d6bcf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019007"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="7e608-103">windowsMobileMSI aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7e608-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="7e608-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e608-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e608-105">Aktualisiert die Eigenschaften von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-105">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e608-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7e608-106">Prerequisites</span></span>
<span data-ttu-id="7e608-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e608-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e608-109">Permission type</span></span>|<span data-ttu-id="7e608-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e608-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e608-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e608-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7e608-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e608-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e608-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e608-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e608-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e608-114">Not supported.</span></span>|
|<span data-ttu-id="7e608-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e608-115">Application</span></span>|<span data-ttu-id="7e608-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e608-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e608-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e608-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7e608-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e608-118">Request headers</span></span>
|<span data-ttu-id="7e608-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7e608-119">Header</span></span>|<span data-ttu-id="7e608-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7e608-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e608-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e608-121">Authorization</span></span>|<span data-ttu-id="7e608-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e608-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e608-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7e608-123">Accept</span></span>|<span data-ttu-id="7e608-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7e608-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e608-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e608-125">Request body</span></span>
<span data-ttu-id="7e608-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7e608-126">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="7e608-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7e608-127">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="7e608-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e608-128">Property</span></span>|<span data-ttu-id="7e608-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7e608-129">Type</span></span>|<span data-ttu-id="7e608-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e608-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e608-131">id</span><span class="sxs-lookup"><span data-stu-id="7e608-131">id</span></span>|<span data-ttu-id="7e608-132">String</span><span class="sxs-lookup"><span data-stu-id="7e608-132">String</span></span>|<span data-ttu-id="7e608-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7e608-133">Key of the entity.</span></span> <span data-ttu-id="7e608-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7e608-135">displayName</span></span>|<span data-ttu-id="7e608-136">String</span><span class="sxs-lookup"><span data-stu-id="7e608-136">String</span></span>|<span data-ttu-id="7e608-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7e608-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-139">description</span><span class="sxs-lookup"><span data-stu-id="7e608-139">description</span></span>|<span data-ttu-id="7e608-140">String</span><span class="sxs-lookup"><span data-stu-id="7e608-140">String</span></span>|<span data-ttu-id="7e608-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-141">The description of the app.</span></span> <span data-ttu-id="7e608-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-143">publisher</span><span class="sxs-lookup"><span data-stu-id="7e608-143">publisher</span></span>|<span data-ttu-id="7e608-144">String</span><span class="sxs-lookup"><span data-stu-id="7e608-144">String</span></span>|<span data-ttu-id="7e608-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-145">The publisher of the app.</span></span> <span data-ttu-id="7e608-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7e608-147">largeIcon</span></span>|[<span data-ttu-id="7e608-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7e608-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7e608-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7e608-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7e608-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e608-151">createdDateTime</span></span>|<span data-ttu-id="7e608-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e608-152">DateTimeOffset</span></span>|<span data-ttu-id="7e608-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-153">The date and time the app was created.</span></span> <span data-ttu-id="7e608-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e608-155">lastModifiedDateTime</span></span>|<span data-ttu-id="7e608-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e608-156">DateTimeOffset</span></span>|<span data-ttu-id="7e608-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-157">The date and time the app was last modified.</span></span> <span data-ttu-id="7e608-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7e608-159">isFeatured</span></span>|<span data-ttu-id="7e608-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7e608-160">Boolean</span></span>|<span data-ttu-id="7e608-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7e608-162">privacyInformationUrl</span></span>|<span data-ttu-id="7e608-163">String</span><span class="sxs-lookup"><span data-stu-id="7e608-163">String</span></span>|<span data-ttu-id="7e608-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="7e608-164">The privacy statement Url.</span></span> <span data-ttu-id="7e608-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7e608-166">informationUrl</span></span>|<span data-ttu-id="7e608-167">String</span><span class="sxs-lookup"><span data-stu-id="7e608-167">String</span></span>|<span data-ttu-id="7e608-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="7e608-168">The more information Url.</span></span> <span data-ttu-id="7e608-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-170">owner</span><span class="sxs-lookup"><span data-stu-id="7e608-170">owner</span></span>|<span data-ttu-id="7e608-171">String</span><span class="sxs-lookup"><span data-stu-id="7e608-171">String</span></span>|<span data-ttu-id="7e608-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-172">The owner of the app.</span></span> <span data-ttu-id="7e608-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-174">developer</span><span class="sxs-lookup"><span data-stu-id="7e608-174">developer</span></span>|<span data-ttu-id="7e608-175">String</span><span class="sxs-lookup"><span data-stu-id="7e608-175">String</span></span>|<span data-ttu-id="7e608-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-176">The developer of the app.</span></span> <span data-ttu-id="7e608-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-178">notes</span><span class="sxs-lookup"><span data-stu-id="7e608-178">notes</span></span>|<span data-ttu-id="7e608-179">String</span><span class="sxs-lookup"><span data-stu-id="7e608-179">String</span></span>|<span data-ttu-id="7e608-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="7e608-180">Notes for the app.</span></span> <span data-ttu-id="7e608-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e608-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="7e608-182">publishingState</span></span>|[<span data-ttu-id="7e608-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7e608-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7e608-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="7e608-184">The publishing state for the app.</span></span> <span data-ttu-id="7e608-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="7e608-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7e608-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7e608-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="7e608-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7e608-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7e608-188">committedContentVersion</span></span>|<span data-ttu-id="7e608-189">String</span><span class="sxs-lookup"><span data-stu-id="7e608-189">String</span></span>|<span data-ttu-id="7e608-190">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="7e608-190">The internal committed content version.</span></span> <span data-ttu-id="7e608-191">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7e608-192">fileName</span><span class="sxs-lookup"><span data-stu-id="7e608-192">fileName</span></span>|<span data-ttu-id="7e608-193">String</span><span class="sxs-lookup"><span data-stu-id="7e608-193">String</span></span>|<span data-ttu-id="7e608-194">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="7e608-194">The name of the main Lob application file.</span></span> <span data-ttu-id="7e608-195">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7e608-196">size</span><span class="sxs-lookup"><span data-stu-id="7e608-196">size</span></span>|<span data-ttu-id="7e608-197">Int64</span><span class="sxs-lookup"><span data-stu-id="7e608-197">Int64</span></span>|<span data-ttu-id="7e608-198">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="7e608-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="7e608-199">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e608-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7e608-200">commandLine</span><span class="sxs-lookup"><span data-stu-id="7e608-200">commandLine</span></span>|<span data-ttu-id="7e608-201">String</span><span class="sxs-lookup"><span data-stu-id="7e608-201">String</span></span>|<span data-ttu-id="7e608-202">Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="7e608-202">The command line.</span></span>|
|<span data-ttu-id="7e608-203">productCode</span><span class="sxs-lookup"><span data-stu-id="7e608-203">productCode</span></span>|<span data-ttu-id="7e608-204">String</span><span class="sxs-lookup"><span data-stu-id="7e608-204">String</span></span>|<span data-ttu-id="7e608-205">Produktcode</span><span class="sxs-lookup"><span data-stu-id="7e608-205">The product code.</span></span>|
|<span data-ttu-id="7e608-206">productVersion</span><span class="sxs-lookup"><span data-stu-id="7e608-206">productVersion</span></span>|<span data-ttu-id="7e608-207">String</span><span class="sxs-lookup"><span data-stu-id="7e608-207">String</span></span>|<span data-ttu-id="7e608-208">Produktversion der branchenspezifischen Windows Mobile-MSI-App.</span><span class="sxs-lookup"><span data-stu-id="7e608-208">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7e608-209">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="7e608-209">ignoreVersionDetection</span></span>|<span data-ttu-id="7e608-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7e608-210">Boolean</span></span>|<span data-ttu-id="7e608-211">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7e608-211">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="7e608-212">Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7e608-212">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="7e608-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e608-213">Response</span></span>
<span data-ttu-id="7e608-214">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e608-214">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e608-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e608-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e608-216">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e608-216">Request</span></span>
<span data-ttu-id="7e608-217">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e608-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="7e608-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e608-218">Response</span></span>
<span data-ttu-id="7e608-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e608-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```



