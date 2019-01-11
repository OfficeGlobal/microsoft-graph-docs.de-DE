---
title: managedAndroidLobApp erstellen
description: Erstellen eines neuen managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5026406a36e523e535286ff82cc3017571e8a875
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892540"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="4e020-103">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="4e020-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="4e020-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e020-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e020-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e020-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e020-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e020-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e020-107">Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e020-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e020-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e020-108">Prerequisites</span></span>
<span data-ttu-id="4e020-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e020-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e020-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e020-111">Permission type</span></span>|<span data-ttu-id="4e020-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e020-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e020-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e020-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e020-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e020-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e020-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e020-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e020-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e020-116">Not supported.</span></span>|
|<span data-ttu-id="4e020-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e020-117">Application</span></span>|<span data-ttu-id="4e020-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e020-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e020-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e020-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4e020-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e020-120">Request headers</span></span>
|<span data-ttu-id="4e020-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4e020-121">Header</span></span>|<span data-ttu-id="4e020-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4e020-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e020-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e020-123">Authorization</span></span>|<span data-ttu-id="4e020-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e020-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e020-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4e020-125">Accept</span></span>|<span data-ttu-id="4e020-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e020-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e020-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e020-127">Request body</span></span>
<span data-ttu-id="4e020-128">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4e020-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="4e020-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4e020-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="4e020-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e020-130">Property</span></span>|<span data-ttu-id="4e020-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4e020-131">Type</span></span>|<span data-ttu-id="4e020-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e020-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e020-133">id</span><span class="sxs-lookup"><span data-stu-id="4e020-133">id</span></span>|<span data-ttu-id="4e020-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-134">String</span></span>|<span data-ttu-id="4e020-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4e020-135">Key of the entity.</span></span> <span data-ttu-id="4e020-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4e020-137">displayName</span></span>|<span data-ttu-id="4e020-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-138">String</span></span>|<span data-ttu-id="4e020-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4e020-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-141">description</span><span class="sxs-lookup"><span data-stu-id="4e020-141">description</span></span>|<span data-ttu-id="4e020-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-142">String</span></span>|<span data-ttu-id="4e020-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-143">The description of the app.</span></span> <span data-ttu-id="4e020-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4e020-145">publisher</span></span>|<span data-ttu-id="4e020-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-146">String</span></span>|<span data-ttu-id="4e020-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-147">The publisher of the app.</span></span> <span data-ttu-id="4e020-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4e020-149">largeIcon</span></span>|[<span data-ttu-id="4e020-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e020-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e020-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e020-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4e020-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e020-153">createdDateTime</span></span>|<span data-ttu-id="4e020-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e020-154">DateTimeOffset</span></span>|<span data-ttu-id="4e020-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-155">The date and time the app was created.</span></span> <span data-ttu-id="4e020-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e020-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4e020-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e020-158">DateTimeOffset</span></span>|<span data-ttu-id="4e020-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4e020-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4e020-161">isFeatured</span></span>|<span data-ttu-id="4e020-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e020-162">Boolean</span></span>|<span data-ttu-id="4e020-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4e020-164">privacyInformationUrl</span></span>|<span data-ttu-id="4e020-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-165">String</span></span>|<span data-ttu-id="4e020-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="4e020-166">The privacy statement Url.</span></span> <span data-ttu-id="4e020-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4e020-168">informationUrl</span></span>|<span data-ttu-id="4e020-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-169">String</span></span>|<span data-ttu-id="4e020-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="4e020-170">The more information Url.</span></span> <span data-ttu-id="4e020-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-172">owner</span><span class="sxs-lookup"><span data-stu-id="4e020-172">owner</span></span>|<span data-ttu-id="4e020-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-173">String</span></span>|<span data-ttu-id="4e020-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-174">The owner of the app.</span></span> <span data-ttu-id="4e020-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-176">developer</span><span class="sxs-lookup"><span data-stu-id="4e020-176">developer</span></span>|<span data-ttu-id="4e020-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-177">String</span></span>|<span data-ttu-id="4e020-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-178">The developer of the app.</span></span> <span data-ttu-id="4e020-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-180">notes</span><span class="sxs-lookup"><span data-stu-id="4e020-180">notes</span></span>|<span data-ttu-id="4e020-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-181">String</span></span>|<span data-ttu-id="4e020-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="4e020-182">Notes for the app.</span></span> <span data-ttu-id="4e020-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4e020-184">uploadState</span></span>|<span data-ttu-id="4e020-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4e020-185">Int32</span></span>|<span data-ttu-id="4e020-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="4e020-186">The upload state.</span></span> <span data-ttu-id="4e020-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e020-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4e020-188">publishingState</span></span>|[<span data-ttu-id="4e020-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4e020-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4e020-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="4e020-190">The publishing state for the app.</span></span> <span data-ttu-id="4e020-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="4e020-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4e020-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4e020-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="4e020-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4e020-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4e020-194">appAvailability</span></span>|[<span data-ttu-id="4e020-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4e020-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4e020-196">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4e020-196">The Application's availability.</span></span> <span data-ttu-id="4e020-197">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4e020-198">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4e020-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4e020-199">version</span><span class="sxs-lookup"><span data-stu-id="4e020-199">version</span></span>|<span data-ttu-id="4e020-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-200">String</span></span>|<span data-ttu-id="4e020-201">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4e020-201">The Application's version.</span></span> <span data-ttu-id="4e020-202">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e020-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4e020-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4e020-203">committedContentVersion</span></span>|<span data-ttu-id="4e020-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-204">String</span></span>|<span data-ttu-id="4e020-205">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="4e020-205">The internal committed content version.</span></span> <span data-ttu-id="4e020-206">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4e020-207">fileName</span><span class="sxs-lookup"><span data-stu-id="4e020-207">fileName</span></span>|<span data-ttu-id="4e020-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-208">String</span></span>|<span data-ttu-id="4e020-209">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="4e020-209">The name of the main Lob application file.</span></span> <span data-ttu-id="4e020-210">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4e020-211">size</span><span class="sxs-lookup"><span data-stu-id="4e020-211">size</span></span>|<span data-ttu-id="4e020-212">Int64</span><span class="sxs-lookup"><span data-stu-id="4e020-212">Int64</span></span>|<span data-ttu-id="4e020-213">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="4e020-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="4e020-214">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e020-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4e020-215">packageId</span><span class="sxs-lookup"><span data-stu-id="4e020-215">packageId</span></span>|<span data-ttu-id="4e020-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-216">String</span></span>|<span data-ttu-id="4e020-217">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="4e020-217">The package identifier.</span></span>|
|<span data-ttu-id="4e020-218">identityName</span><span class="sxs-lookup"><span data-stu-id="4e020-218">identityName</span></span>|<span data-ttu-id="4e020-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-219">String</span></span>|<span data-ttu-id="4e020-220">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="4e020-220">The Identity Name.</span></span>|
|<span data-ttu-id="4e020-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4e020-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4e020-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4e020-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4e020-223">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="4e020-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4e020-224">versionName</span><span class="sxs-lookup"><span data-stu-id="4e020-224">versionName</span></span>|<span data-ttu-id="4e020-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-225">String</span></span>|<span data-ttu-id="4e020-226">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="4e020-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4e020-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="4e020-227">versionCode</span></span>|<span data-ttu-id="4e020-228">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-228">String</span></span>|<span data-ttu-id="4e020-229">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="4e020-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4e020-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4e020-230">identityVersion</span></span>|<span data-ttu-id="4e020-231">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e020-231">String</span></span>|<span data-ttu-id="4e020-232">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="4e020-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4e020-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e020-233">Response</span></span>
<span data-ttu-id="4e020-234">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e020-234">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e020-235">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e020-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e020-236">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e020-236">Request</span></span>
<span data-ttu-id="4e020-237">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e020-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1443

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

### <a name="response"></a><span data-ttu-id="4e020-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e020-238">Response</span></span>
<span data-ttu-id="4e020-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e020-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





