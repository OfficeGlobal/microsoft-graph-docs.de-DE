---
title: AndroidForWorkApp erstellen
description: Erstellen eines neuen androidForWorkApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee453dbc880daa84dac12c4ce8a2555b37474825
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960279"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="c997c-103">AndroidForWorkApp erstellen</span><span class="sxs-lookup"><span data-stu-id="c997c-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="c997c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c997c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c997c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c997c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c997c-106">Erstellen eines neuen [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c997c-106">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c997c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c997c-107">Prerequisites</span></span>
<span data-ttu-id="c997c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c997c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c997c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c997c-110">Permission type</span></span>|<span data-ttu-id="c997c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c997c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c997c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c997c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c997c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c997c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c997c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c997c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c997c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c997c-115">Not supported.</span></span>|
|<span data-ttu-id="c997c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c997c-116">Application</span></span>|<span data-ttu-id="c997c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c997c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c997c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c997c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c997c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c997c-119">Request headers</span></span>
|<span data-ttu-id="c997c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c997c-120">Header</span></span>|<span data-ttu-id="c997c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c997c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c997c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c997c-122">Authorization</span></span>|<span data-ttu-id="c997c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c997c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c997c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c997c-124">Accept</span></span>|<span data-ttu-id="c997c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c997c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c997c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c997c-126">Request body</span></span>
<span data-ttu-id="c997c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidForWorkApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c997c-127">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="c997c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidForWorkApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c997c-128">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="c997c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c997c-129">Property</span></span>|<span data-ttu-id="c997c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c997c-130">Type</span></span>|<span data-ttu-id="c997c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c997c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c997c-132">id</span><span class="sxs-lookup"><span data-stu-id="c997c-132">id</span></span>|<span data-ttu-id="c997c-133">String</span><span class="sxs-lookup"><span data-stu-id="c997c-133">String</span></span>|<span data-ttu-id="c997c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c997c-134">Key of the entity.</span></span> <span data-ttu-id="c997c-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c997c-136">displayName</span></span>|<span data-ttu-id="c997c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c997c-137">String</span></span>|<span data-ttu-id="c997c-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c997c-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-140">description</span><span class="sxs-lookup"><span data-stu-id="c997c-140">description</span></span>|<span data-ttu-id="c997c-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c997c-141">String</span></span>|<span data-ttu-id="c997c-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-142">The description of the app.</span></span> <span data-ttu-id="c997c-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c997c-144">publisher</span></span>|<span data-ttu-id="c997c-145">String</span><span class="sxs-lookup"><span data-stu-id="c997c-145">String</span></span>|<span data-ttu-id="c997c-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-146">The publisher of the app.</span></span> <span data-ttu-id="c997c-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c997c-148">largeIcon</span></span>|[<span data-ttu-id="c997c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c997c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c997c-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c997c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c997c-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c997c-152">createdDateTime</span></span>|<span data-ttu-id="c997c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c997c-153">DateTimeOffset</span></span>|<span data-ttu-id="c997c-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-154">The date and time the app was created.</span></span> <span data-ttu-id="c997c-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c997c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c997c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c997c-157">DateTimeOffset</span></span>|<span data-ttu-id="c997c-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c997c-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c997c-160">isFeatured</span></span>|<span data-ttu-id="c997c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c997c-161">Boolean</span></span>|<span data-ttu-id="c997c-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c997c-163">privacyInformationUrl</span></span>|<span data-ttu-id="c997c-164">String</span><span class="sxs-lookup"><span data-stu-id="c997c-164">String</span></span>|<span data-ttu-id="c997c-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="c997c-165">The privacy statement Url.</span></span> <span data-ttu-id="c997c-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c997c-167">informationUrl</span></span>|<span data-ttu-id="c997c-168">String</span><span class="sxs-lookup"><span data-stu-id="c997c-168">String</span></span>|<span data-ttu-id="c997c-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c997c-169">The more information Url.</span></span> <span data-ttu-id="c997c-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-171">owner</span><span class="sxs-lookup"><span data-stu-id="c997c-171">owner</span></span>|<span data-ttu-id="c997c-172">String</span><span class="sxs-lookup"><span data-stu-id="c997c-172">String</span></span>|<span data-ttu-id="c997c-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-173">The owner of the app.</span></span> <span data-ttu-id="c997c-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-175">developer</span><span class="sxs-lookup"><span data-stu-id="c997c-175">developer</span></span>|<span data-ttu-id="c997c-176">String</span><span class="sxs-lookup"><span data-stu-id="c997c-176">String</span></span>|<span data-ttu-id="c997c-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c997c-177">The developer of the app.</span></span> <span data-ttu-id="c997c-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-179">notes</span><span class="sxs-lookup"><span data-stu-id="c997c-179">notes</span></span>|<span data-ttu-id="c997c-180">String</span><span class="sxs-lookup"><span data-stu-id="c997c-180">String</span></span>|<span data-ttu-id="c997c-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="c997c-181">Notes for the app.</span></span> <span data-ttu-id="c997c-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c997c-183">uploadState</span></span>|<span data-ttu-id="c997c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c997c-184">Int32</span></span>|<span data-ttu-id="c997c-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="c997c-185">The upload state.</span></span> <span data-ttu-id="c997c-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c997c-187">publishingState</span></span>|[<span data-ttu-id="c997c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c997c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c997c-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="c997c-189">The publishing state for the app.</span></span> <span data-ttu-id="c997c-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c997c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c997c-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c997c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c997c-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c997c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c997c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c997c-193">isAssigned</span></span>|<span data-ttu-id="c997c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c997c-194">Boolean</span></span>|<span data-ttu-id="c997c-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c997c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c997c-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c997c-197">roleScopeTagIds</span></span>|<span data-ttu-id="c997c-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c997c-198">String collection</span></span>|<span data-ttu-id="c997c-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="c997c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c997c-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c997c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c997c-201">packageId</span><span class="sxs-lookup"><span data-stu-id="c997c-201">packageId</span></span>|<span data-ttu-id="c997c-202">String</span><span class="sxs-lookup"><span data-stu-id="c997c-202">String</span></span>|<span data-ttu-id="c997c-203">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="c997c-203">The package identifier.</span></span>|
|<span data-ttu-id="c997c-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c997c-204">appIdentifier</span></span>|<span data-ttu-id="c997c-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c997c-205">String</span></span>|<span data-ttu-id="c997c-206">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="c997c-206">The Identity Name.</span></span>|
|<span data-ttu-id="c997c-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c997c-207">usedLicenseCount</span></span>|<span data-ttu-id="c997c-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c997c-208">Int32</span></span>|<span data-ttu-id="c997c-209">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c997c-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="c997c-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c997c-210">totalLicenseCount</span></span>|<span data-ttu-id="c997c-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c997c-211">Int32</span></span>|<span data-ttu-id="c997c-212">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c997c-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="c997c-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c997c-213">appStoreUrl</span></span>|<span data-ttu-id="c997c-214">String</span><span class="sxs-lookup"><span data-stu-id="c997c-214">String</span></span>|<span data-ttu-id="c997c-215">Die App-URL für die Wiedergabe für Arbeitsspeicher.</span><span class="sxs-lookup"><span data-stu-id="c997c-215">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="c997c-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="c997c-216">Response</span></span>
<span data-ttu-id="c997c-217">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c997c-217">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c997c-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c997c-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="c997c-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c997c-219">Request</span></span>
<span data-ttu-id="c997c-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c997c-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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

### <a name="response"></a><span data-ttu-id="c997c-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="c997c-221">Response</span></span>
<span data-ttu-id="c997c-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c997c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1048

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




