---
title: AndroidManagedStoreApp erstellen
description: Erstellen eines neuen androidManagedStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f25ee01127c4a3256f7893d8360d4ebb4362a0d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151646"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="83d0f-103">AndroidManagedStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="83d0f-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="83d0f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83d0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83d0f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="83d0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83d0f-106">Erstellen eines neuen [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="83d0f-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83d0f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83d0f-107">Prerequisites</span></span>
<span data-ttu-id="83d0f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83d0f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83d0f-110">Permission type</span></span>|<span data-ttu-id="83d0f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83d0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83d0f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83d0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83d0f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d0f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83d0f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83d0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83d0f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83d0f-115">Not supported.</span></span>|
|<span data-ttu-id="83d0f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83d0f-116">Application</span></span>|<span data-ttu-id="83d0f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83d0f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83d0f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83d0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="83d0f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83d0f-119">Request headers</span></span>
|<span data-ttu-id="83d0f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83d0f-120">Header</span></span>|<span data-ttu-id="83d0f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="83d0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83d0f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83d0f-122">Authorization</span></span>|<span data-ttu-id="83d0f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83d0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83d0f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="83d0f-124">Accept</span></span>|<span data-ttu-id="83d0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83d0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83d0f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83d0f-126">Request body</span></span>
<span data-ttu-id="83d0f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidManagedStoreApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="83d0f-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="83d0f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidManagedStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="83d0f-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="83d0f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83d0f-129">Property</span></span>|<span data-ttu-id="83d0f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="83d0f-130">Type</span></span>|<span data-ttu-id="83d0f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83d0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83d0f-132">id</span><span class="sxs-lookup"><span data-stu-id="83d0f-132">id</span></span>|<span data-ttu-id="83d0f-133">string</span><span class="sxs-lookup"><span data-stu-id="83d0f-133">String</span></span>|<span data-ttu-id="83d0f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="83d0f-134">Key of the entity.</span></span> <span data-ttu-id="83d0f-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="83d0f-136">displayName</span></span>|<span data-ttu-id="83d0f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-137">String</span></span>|<span data-ttu-id="83d0f-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="83d0f-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-140">description</span><span class="sxs-lookup"><span data-stu-id="83d0f-140">description</span></span>|<span data-ttu-id="83d0f-141">String</span><span class="sxs-lookup"><span data-stu-id="83d0f-141">String</span></span>|<span data-ttu-id="83d0f-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-142">The description of the app.</span></span> <span data-ttu-id="83d0f-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="83d0f-144">publisher</span></span>|<span data-ttu-id="83d0f-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-145">String</span></span>|<span data-ttu-id="83d0f-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-146">The publisher of the app.</span></span> <span data-ttu-id="83d0f-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="83d0f-148">largeIcon</span></span>|[<span data-ttu-id="83d0f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="83d0f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="83d0f-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="83d0f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="83d0f-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83d0f-152">createdDateTime</span></span>|<span data-ttu-id="83d0f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d0f-153">DateTimeOffset</span></span>|<span data-ttu-id="83d0f-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-154">The date and time the app was created.</span></span> <span data-ttu-id="83d0f-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83d0f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="83d0f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d0f-157">DateTimeOffset</span></span>|<span data-ttu-id="83d0f-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="83d0f-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="83d0f-160">isFeatured</span></span>|<span data-ttu-id="83d0f-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83d0f-161">Boolean</span></span>|<span data-ttu-id="83d0f-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="83d0f-163">privacyInformationUrl</span></span>|<span data-ttu-id="83d0f-164">String</span><span class="sxs-lookup"><span data-stu-id="83d0f-164">String</span></span>|<span data-ttu-id="83d0f-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="83d0f-165">The privacy statement Url.</span></span> <span data-ttu-id="83d0f-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="83d0f-167">informationUrl</span></span>|<span data-ttu-id="83d0f-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-168">String</span></span>|<span data-ttu-id="83d0f-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="83d0f-169">The more information Url.</span></span> <span data-ttu-id="83d0f-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-171">owner</span><span class="sxs-lookup"><span data-stu-id="83d0f-171">owner</span></span>|<span data-ttu-id="83d0f-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-172">String</span></span>|<span data-ttu-id="83d0f-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-173">The owner of the app.</span></span> <span data-ttu-id="83d0f-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-175">developer</span><span class="sxs-lookup"><span data-stu-id="83d0f-175">developer</span></span>|<span data-ttu-id="83d0f-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-176">String</span></span>|<span data-ttu-id="83d0f-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-177">The developer of the app.</span></span> <span data-ttu-id="83d0f-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-179">notes</span><span class="sxs-lookup"><span data-stu-id="83d0f-179">notes</span></span>|<span data-ttu-id="83d0f-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-180">String</span></span>|<span data-ttu-id="83d0f-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-181">Notes for the app.</span></span> <span data-ttu-id="83d0f-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="83d0f-183">uploadState</span></span>|<span data-ttu-id="83d0f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="83d0f-184">Int32</span></span>|<span data-ttu-id="83d0f-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="83d0f-185">The upload state.</span></span> <span data-ttu-id="83d0f-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="83d0f-187">publishingState</span></span>|[<span data-ttu-id="83d0f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="83d0f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="83d0f-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-189">The publishing state for the app.</span></span> <span data-ttu-id="83d0f-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="83d0f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="83d0f-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="83d0f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="83d0f-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="83d0f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="83d0f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="83d0f-193">isAssigned</span></span>|<span data-ttu-id="83d0f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="83d0f-194">Boolean</span></span>|<span data-ttu-id="83d0f-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="83d0f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="83d0f-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="83d0f-197">roleScopeTagIds</span></span>|<span data-ttu-id="83d0f-198">String collection</span><span class="sxs-lookup"><span data-stu-id="83d0f-198">String collection</span></span>|<span data-ttu-id="83d0f-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="83d0f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="83d0f-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="83d0f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83d0f-201">packageId</span><span class="sxs-lookup"><span data-stu-id="83d0f-201">packageId</span></span>|<span data-ttu-id="83d0f-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-202">String</span></span>|<span data-ttu-id="83d0f-203">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="83d0f-203">The package identifier.</span></span>|
|<span data-ttu-id="83d0f-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="83d0f-204">appIdentifier</span></span>|<span data-ttu-id="83d0f-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-205">String</span></span>|<span data-ttu-id="83d0f-206">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="83d0f-206">The Identity Name.</span></span>|
|<span data-ttu-id="83d0f-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="83d0f-207">usedLicenseCount</span></span>|<span data-ttu-id="83d0f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="83d0f-208">Int32</span></span>|<span data-ttu-id="83d0f-209">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="83d0f-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="83d0f-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="83d0f-210">totalLicenseCount</span></span>|<span data-ttu-id="83d0f-211">Int32</span><span class="sxs-lookup"><span data-stu-id="83d0f-211">Int32</span></span>|<span data-ttu-id="83d0f-212">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="83d0f-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="83d0f-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="83d0f-213">appStoreUrl</span></span>|<span data-ttu-id="83d0f-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83d0f-214">String</span></span>|<span data-ttu-id="83d0f-215">Die App-URL für die Wiedergabe für Arbeitsspeicher.</span><span class="sxs-lookup"><span data-stu-id="83d0f-215">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="83d0f-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="83d0f-216">Response</span></span>
<span data-ttu-id="83d0f-217">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83d0f-217">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83d0f-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83d0f-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="83d0f-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83d0f-219">Request</span></span>
<span data-ttu-id="83d0f-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83d0f-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="83d0f-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="83d0f-221">Response</span></span>
<span data-ttu-id="83d0f-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83d0f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1053

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




