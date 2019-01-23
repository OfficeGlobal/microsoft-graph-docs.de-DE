---
title: Erstellen von „androidStoreApp“
description: Diese Methode erstellt ein neues Objekt des Typs androidStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa67da6ecbf1a2d0b508c228265998b69b86c4f3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401936"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="065c7-103">Erstellen von „androidStoreApp“</span><span class="sxs-lookup"><span data-stu-id="065c7-103">Create androidStoreApp</span></span>

> <span data-ttu-id="065c7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="065c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="065c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="065c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="065c7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="065c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="065c7-107">Diese Methode erstellt ein neues Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="065c7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="065c7-108">Prerequisites</span></span>
<span data-ttu-id="065c7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="065c7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="065c7-111">Permission type</span></span>|<span data-ttu-id="065c7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="065c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="065c7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="065c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="065c7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="065c7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="065c7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="065c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="065c7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="065c7-116">Not supported.</span></span>|
|<span data-ttu-id="065c7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="065c7-117">Application</span></span>|<span data-ttu-id="065c7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="065c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="065c7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="065c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="065c7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="065c7-120">Request headers</span></span>
|<span data-ttu-id="065c7-121">Header</span><span class="sxs-lookup"><span data-stu-id="065c7-121">Header</span></span>|<span data-ttu-id="065c7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="065c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="065c7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="065c7-123">Authorization</span></span>|<span data-ttu-id="065c7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="065c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="065c7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="065c7-125">Accept</span></span>|<span data-ttu-id="065c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="065c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="065c7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="065c7-127">Request body</span></span>
<span data-ttu-id="065c7-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidStoreApp“ an.</span><span class="sxs-lookup"><span data-stu-id="065c7-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="065c7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidStoreApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="065c7-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="065c7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="065c7-130">Property</span></span>|<span data-ttu-id="065c7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="065c7-131">Type</span></span>|<span data-ttu-id="065c7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="065c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="065c7-133">id</span><span class="sxs-lookup"><span data-stu-id="065c7-133">id</span></span>|<span data-ttu-id="065c7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-134">String</span></span>|<span data-ttu-id="065c7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="065c7-135">Key of the entity.</span></span> <span data-ttu-id="065c7-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="065c7-137">displayName</span></span>|<span data-ttu-id="065c7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-138">String</span></span>|<span data-ttu-id="065c7-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="065c7-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-141">description</span><span class="sxs-lookup"><span data-stu-id="065c7-141">description</span></span>|<span data-ttu-id="065c7-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-142">String</span></span>|<span data-ttu-id="065c7-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-143">The description of the app.</span></span> <span data-ttu-id="065c7-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="065c7-145">publisher</span></span>|<span data-ttu-id="065c7-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-146">String</span></span>|<span data-ttu-id="065c7-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-147">The publisher of the app.</span></span> <span data-ttu-id="065c7-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="065c7-149">largeIcon</span></span>|[<span data-ttu-id="065c7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="065c7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="065c7-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="065c7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="065c7-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="065c7-153">createdDateTime</span></span>|<span data-ttu-id="065c7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="065c7-154">DateTimeOffset</span></span>|<span data-ttu-id="065c7-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-155">The date and time the app was created.</span></span> <span data-ttu-id="065c7-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="065c7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="065c7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="065c7-158">DateTimeOffset</span></span>|<span data-ttu-id="065c7-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="065c7-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="065c7-161">isFeatured</span></span>|<span data-ttu-id="065c7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="065c7-162">Boolean</span></span>|<span data-ttu-id="065c7-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="065c7-164">privacyInformationUrl</span></span>|<span data-ttu-id="065c7-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-165">String</span></span>|<span data-ttu-id="065c7-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="065c7-166">The privacy statement Url.</span></span> <span data-ttu-id="065c7-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="065c7-168">informationUrl</span></span>|<span data-ttu-id="065c7-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-169">String</span></span>|<span data-ttu-id="065c7-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="065c7-170">The more information Url.</span></span> <span data-ttu-id="065c7-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-172">owner</span><span class="sxs-lookup"><span data-stu-id="065c7-172">owner</span></span>|<span data-ttu-id="065c7-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-173">String</span></span>|<span data-ttu-id="065c7-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-174">The owner of the app.</span></span> <span data-ttu-id="065c7-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-176">developer</span><span class="sxs-lookup"><span data-stu-id="065c7-176">developer</span></span>|<span data-ttu-id="065c7-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-177">String</span></span>|<span data-ttu-id="065c7-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-178">The developer of the app.</span></span> <span data-ttu-id="065c7-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-180">notes</span><span class="sxs-lookup"><span data-stu-id="065c7-180">notes</span></span>|<span data-ttu-id="065c7-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-181">String</span></span>|<span data-ttu-id="065c7-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="065c7-182">Notes for the app.</span></span> <span data-ttu-id="065c7-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="065c7-184">uploadState</span></span>|<span data-ttu-id="065c7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="065c7-185">Int32</span></span>|<span data-ttu-id="065c7-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="065c7-186">The upload state.</span></span> <span data-ttu-id="065c7-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="065c7-188">publishingState</span></span>|[<span data-ttu-id="065c7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="065c7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="065c7-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="065c7-190">The publishing state for the app.</span></span> <span data-ttu-id="065c7-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="065c7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="065c7-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="065c7-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="065c7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="065c7-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="065c7-194">isAssigned</span></span>|<span data-ttu-id="065c7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="065c7-195">Boolean</span></span>|<span data-ttu-id="065c7-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="065c7-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="065c7-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="065c7-198">roleScopeTagIds</span></span>|<span data-ttu-id="065c7-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="065c7-199">String collection</span></span>|<span data-ttu-id="065c7-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="065c7-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="065c7-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="065c7-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="065c7-202">packageId</span><span class="sxs-lookup"><span data-stu-id="065c7-202">packageId</span></span>|<span data-ttu-id="065c7-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-203">String</span></span>|<span data-ttu-id="065c7-204">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="065c7-204">The package identifier.</span></span>|
|<span data-ttu-id="065c7-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="065c7-205">appIdentifier</span></span>|<span data-ttu-id="065c7-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-206">String</span></span>|<span data-ttu-id="065c7-207">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="065c7-207">The Identity Name.</span></span>|
|<span data-ttu-id="065c7-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="065c7-208">appStoreUrl</span></span>|<span data-ttu-id="065c7-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065c7-209">String</span></span>|<span data-ttu-id="065c7-210">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="065c7-210">The Android app store URL.</span></span>|
|<span data-ttu-id="065c7-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="065c7-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="065c7-212">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="065c7-212">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="065c7-213">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="065c7-213">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="065c7-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="065c7-214">Response</span></span>
<span data-ttu-id="065c7-215">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="065c7-215">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="065c7-216">Beispiel</span><span class="sxs-lookup"><span data-stu-id="065c7-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="065c7-217">Anforderung</span><span class="sxs-lookup"><span data-stu-id="065c7-217">Request</span></span>
<span data-ttu-id="065c7-218">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="065c7-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1203

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="065c7-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="065c7-219">Response</span></span>
<span data-ttu-id="065c7-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="065c7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1375

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```




