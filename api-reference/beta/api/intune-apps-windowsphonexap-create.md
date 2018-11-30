---
title: Erstellen von windowsPhoneXAP
description: Erstellen eines neuen WindowsPhoneXAP-Objekts.
ms.openlocfilehash: 8b22ed8d9294c8e7a3e5c2e91e5b3d82e8f6bce9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065263"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="23cfd-103">Erstellen von windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="23cfd-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="23cfd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23cfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23cfd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23cfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23cfd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23cfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23cfd-107">Erstellen eines neuen [WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="23cfd-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23cfd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23cfd-108">Prerequisites</span></span>
<span data-ttu-id="23cfd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23cfd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23cfd-111">Permission type</span></span>|<span data-ttu-id="23cfd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23cfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23cfd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23cfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23cfd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cfd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="23cfd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23cfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cfd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23cfd-116">Not supported.</span></span>|
|<span data-ttu-id="23cfd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23cfd-117">Application</span></span>|<span data-ttu-id="23cfd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23cfd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cfd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23cfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="23cfd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23cfd-120">Request headers</span></span>
|<span data-ttu-id="23cfd-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="23cfd-121">Header</span></span>|<span data-ttu-id="23cfd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="23cfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23cfd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23cfd-123">Authorization</span></span>|<span data-ttu-id="23cfd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23cfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23cfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23cfd-125">Accept</span></span>|<span data-ttu-id="23cfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23cfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23cfd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23cfd-127">Request body</span></span>
<span data-ttu-id="23cfd-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsPhoneXAP eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="23cfd-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="23cfd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsPhoneXAP erstellen.</span><span class="sxs-lookup"><span data-stu-id="23cfd-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="23cfd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23cfd-130">Property</span></span>|<span data-ttu-id="23cfd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="23cfd-131">Type</span></span>|<span data-ttu-id="23cfd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23cfd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23cfd-133">id</span><span class="sxs-lookup"><span data-stu-id="23cfd-133">id</span></span>|<span data-ttu-id="23cfd-134">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-134">String</span></span>|<span data-ttu-id="23cfd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="23cfd-135">Key of the entity.</span></span> <span data-ttu-id="23cfd-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="23cfd-137">displayName</span></span>|<span data-ttu-id="23cfd-138">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-138">String</span></span>|<span data-ttu-id="23cfd-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="23cfd-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-141">description</span><span class="sxs-lookup"><span data-stu-id="23cfd-141">description</span></span>|<span data-ttu-id="23cfd-142">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-142">String</span></span>|<span data-ttu-id="23cfd-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-143">The description of the app.</span></span> <span data-ttu-id="23cfd-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="23cfd-145">publisher</span></span>|<span data-ttu-id="23cfd-146">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-146">String</span></span>|<span data-ttu-id="23cfd-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-147">The publisher of the app.</span></span> <span data-ttu-id="23cfd-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="23cfd-149">largeIcon</span></span>|[<span data-ttu-id="23cfd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="23cfd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="23cfd-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="23cfd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="23cfd-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23cfd-153">createdDateTime</span></span>|<span data-ttu-id="23cfd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23cfd-154">DateTimeOffset</span></span>|<span data-ttu-id="23cfd-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-155">The date and time the app was created.</span></span> <span data-ttu-id="23cfd-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23cfd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="23cfd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23cfd-158">DateTimeOffset</span></span>|<span data-ttu-id="23cfd-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="23cfd-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="23cfd-161">isFeatured</span></span>|<span data-ttu-id="23cfd-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="23cfd-162">Boolean</span></span>|<span data-ttu-id="23cfd-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="23cfd-164">privacyInformationUrl</span></span>|<span data-ttu-id="23cfd-165">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-165">String</span></span>|<span data-ttu-id="23cfd-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="23cfd-166">The privacy statement Url.</span></span> <span data-ttu-id="23cfd-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="23cfd-168">informationUrl</span></span>|<span data-ttu-id="23cfd-169">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-169">String</span></span>|<span data-ttu-id="23cfd-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="23cfd-170">The more information Url.</span></span> <span data-ttu-id="23cfd-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-172">owner</span><span class="sxs-lookup"><span data-stu-id="23cfd-172">owner</span></span>|<span data-ttu-id="23cfd-173">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-173">String</span></span>|<span data-ttu-id="23cfd-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-174">The owner of the app.</span></span> <span data-ttu-id="23cfd-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-176">developer</span><span class="sxs-lookup"><span data-stu-id="23cfd-176">developer</span></span>|<span data-ttu-id="23cfd-177">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-177">String</span></span>|<span data-ttu-id="23cfd-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-178">The developer of the app.</span></span> <span data-ttu-id="23cfd-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-180">notes</span><span class="sxs-lookup"><span data-stu-id="23cfd-180">notes</span></span>|<span data-ttu-id="23cfd-181">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-181">String</span></span>|<span data-ttu-id="23cfd-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-182">Notes for the app.</span></span> <span data-ttu-id="23cfd-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="23cfd-184">uploadState</span></span>|<span data-ttu-id="23cfd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="23cfd-185">Int32</span></span>|<span data-ttu-id="23cfd-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="23cfd-186">The upload state.</span></span> <span data-ttu-id="23cfd-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="23cfd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="23cfd-188">publishingState</span></span>|[<span data-ttu-id="23cfd-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="23cfd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="23cfd-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="23cfd-190">The publishing state for the app.</span></span> <span data-ttu-id="23cfd-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="23cfd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="23cfd-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="23cfd-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="23cfd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="23cfd-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="23cfd-194">committedContentVersion</span></span>|<span data-ttu-id="23cfd-195">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-195">String</span></span>|<span data-ttu-id="23cfd-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="23cfd-196">The internal committed content version.</span></span> <span data-ttu-id="23cfd-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="23cfd-198">fileName</span><span class="sxs-lookup"><span data-stu-id="23cfd-198">fileName</span></span>|<span data-ttu-id="23cfd-199">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-199">String</span></span>|<span data-ttu-id="23cfd-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="23cfd-200">The name of the main Lob application file.</span></span> <span data-ttu-id="23cfd-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="23cfd-202">size</span><span class="sxs-lookup"><span data-stu-id="23cfd-202">size</span></span>|<span data-ttu-id="23cfd-203">Int64</span><span class="sxs-lookup"><span data-stu-id="23cfd-203">Int64</span></span>|<span data-ttu-id="23cfd-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="23cfd-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="23cfd-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="23cfd-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="23cfd-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="23cfd-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="23cfd-207">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="23cfd-207">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="23cfd-208">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="23cfd-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="23cfd-209">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="23cfd-209">productIdentifier</span></span>|<span data-ttu-id="23cfd-210">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-210">String</span></span>|<span data-ttu-id="23cfd-211">Die Produkt-ID.</span><span class="sxs-lookup"><span data-stu-id="23cfd-211">The Product Identifier.</span></span>|
|<span data-ttu-id="23cfd-212">identityVersion</span><span class="sxs-lookup"><span data-stu-id="23cfd-212">identityVersion</span></span>|<span data-ttu-id="23cfd-213">String</span><span class="sxs-lookup"><span data-stu-id="23cfd-213">String</span></span>|<span data-ttu-id="23cfd-214">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="23cfd-214">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="23cfd-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="23cfd-215">Response</span></span>
<span data-ttu-id="23cfd-216">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="23cfd-216">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23cfd-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23cfd-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="23cfd-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23cfd-218">Request</span></span>
<span data-ttu-id="23cfd-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23cfd-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1143

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="23cfd-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="23cfd-220">Response</span></span>
<span data-ttu-id="23cfd-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23cfd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





