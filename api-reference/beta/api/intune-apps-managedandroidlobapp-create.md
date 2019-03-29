---
title: managedAndroidLobApp erstellen
description: Erstellen eines neuen managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f81cf78430119e1b244c6063f8d4f92920dca3b0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973719"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="8289a-103">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="8289a-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="8289a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8289a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8289a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8289a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8289a-106">Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8289a-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8289a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8289a-107">Prerequisites</span></span>
<span data-ttu-id="8289a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8289a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8289a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8289a-110">Permission type</span></span>|<span data-ttu-id="8289a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8289a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8289a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8289a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8289a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8289a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8289a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8289a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8289a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8289a-115">Not supported.</span></span>|
|<span data-ttu-id="8289a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8289a-116">Application</span></span>|<span data-ttu-id="8289a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8289a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8289a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8289a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8289a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8289a-119">Request headers</span></span>
|<span data-ttu-id="8289a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8289a-120">Header</span></span>|<span data-ttu-id="8289a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8289a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8289a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8289a-122">Authorization</span></span>|<span data-ttu-id="8289a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8289a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8289a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8289a-124">Accept</span></span>|<span data-ttu-id="8289a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8289a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8289a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8289a-126">Request body</span></span>
<span data-ttu-id="8289a-127">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8289a-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="8289a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8289a-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="8289a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8289a-129">Property</span></span>|<span data-ttu-id="8289a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8289a-130">Type</span></span>|<span data-ttu-id="8289a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8289a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8289a-132">id</span><span class="sxs-lookup"><span data-stu-id="8289a-132">id</span></span>|<span data-ttu-id="8289a-133">String</span><span class="sxs-lookup"><span data-stu-id="8289a-133">String</span></span>|<span data-ttu-id="8289a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8289a-134">Key of the entity.</span></span> <span data-ttu-id="8289a-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8289a-136">displayName</span></span>|<span data-ttu-id="8289a-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8289a-137">String</span></span>|<span data-ttu-id="8289a-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8289a-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-140">description</span><span class="sxs-lookup"><span data-stu-id="8289a-140">description</span></span>|<span data-ttu-id="8289a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8289a-141">String</span></span>|<span data-ttu-id="8289a-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-142">The description of the app.</span></span> <span data-ttu-id="8289a-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8289a-144">publisher</span></span>|<span data-ttu-id="8289a-145">String</span><span class="sxs-lookup"><span data-stu-id="8289a-145">String</span></span>|<span data-ttu-id="8289a-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-146">The publisher of the app.</span></span> <span data-ttu-id="8289a-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8289a-148">largeIcon</span></span>|[<span data-ttu-id="8289a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8289a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8289a-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8289a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8289a-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8289a-152">createdDateTime</span></span>|<span data-ttu-id="8289a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8289a-153">DateTimeOffset</span></span>|<span data-ttu-id="8289a-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-154">The date and time the app was created.</span></span> <span data-ttu-id="8289a-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8289a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8289a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8289a-157">DateTimeOffset</span></span>|<span data-ttu-id="8289a-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8289a-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8289a-160">isFeatured</span></span>|<span data-ttu-id="8289a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8289a-161">Boolean</span></span>|<span data-ttu-id="8289a-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8289a-163">privacyInformationUrl</span></span>|<span data-ttu-id="8289a-164">String</span><span class="sxs-lookup"><span data-stu-id="8289a-164">String</span></span>|<span data-ttu-id="8289a-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="8289a-165">The privacy statement Url.</span></span> <span data-ttu-id="8289a-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8289a-167">informationUrl</span></span>|<span data-ttu-id="8289a-168">String</span><span class="sxs-lookup"><span data-stu-id="8289a-168">String</span></span>|<span data-ttu-id="8289a-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8289a-169">The more information Url.</span></span> <span data-ttu-id="8289a-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-171">owner</span><span class="sxs-lookup"><span data-stu-id="8289a-171">owner</span></span>|<span data-ttu-id="8289a-172">String</span><span class="sxs-lookup"><span data-stu-id="8289a-172">String</span></span>|<span data-ttu-id="8289a-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-173">The owner of the app.</span></span> <span data-ttu-id="8289a-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-175">developer</span><span class="sxs-lookup"><span data-stu-id="8289a-175">developer</span></span>|<span data-ttu-id="8289a-176">String</span><span class="sxs-lookup"><span data-stu-id="8289a-176">String</span></span>|<span data-ttu-id="8289a-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="8289a-177">The developer of the app.</span></span> <span data-ttu-id="8289a-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-179">notes</span><span class="sxs-lookup"><span data-stu-id="8289a-179">notes</span></span>|<span data-ttu-id="8289a-180">String</span><span class="sxs-lookup"><span data-stu-id="8289a-180">String</span></span>|<span data-ttu-id="8289a-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="8289a-181">Notes for the app.</span></span> <span data-ttu-id="8289a-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8289a-183">uploadState</span></span>|<span data-ttu-id="8289a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8289a-184">Int32</span></span>|<span data-ttu-id="8289a-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="8289a-185">The upload state.</span></span> <span data-ttu-id="8289a-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8289a-187">publishingState</span></span>|[<span data-ttu-id="8289a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8289a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8289a-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="8289a-189">The publishing state for the app.</span></span> <span data-ttu-id="8289a-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="8289a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8289a-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="8289a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8289a-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="8289a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8289a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8289a-193">isAssigned</span></span>|<span data-ttu-id="8289a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8289a-194">Boolean</span></span>|<span data-ttu-id="8289a-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="8289a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8289a-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="8289a-197">roleScopeTagIds</span></span>|<span data-ttu-id="8289a-198">String collection</span><span class="sxs-lookup"><span data-stu-id="8289a-198">String collection</span></span>|<span data-ttu-id="8289a-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="8289a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8289a-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8289a-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8289a-201">appAvailability</span></span>|[<span data-ttu-id="8289a-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8289a-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8289a-203">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8289a-203">The Application's availability.</span></span> <span data-ttu-id="8289a-204">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="8289a-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8289a-205">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8289a-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8289a-206">version</span><span class="sxs-lookup"><span data-stu-id="8289a-206">version</span></span>|<span data-ttu-id="8289a-207">String</span><span class="sxs-lookup"><span data-stu-id="8289a-207">String</span></span>|<span data-ttu-id="8289a-208">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8289a-208">The Application's version.</span></span> <span data-ttu-id="8289a-209">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8289a-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8289a-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8289a-210">committedContentVersion</span></span>|<span data-ttu-id="8289a-211">String</span><span class="sxs-lookup"><span data-stu-id="8289a-211">String</span></span>|<span data-ttu-id="8289a-212">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="8289a-212">The internal committed content version.</span></span> <span data-ttu-id="8289a-213">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8289a-214">fileName</span><span class="sxs-lookup"><span data-stu-id="8289a-214">fileName</span></span>|<span data-ttu-id="8289a-215">String</span><span class="sxs-lookup"><span data-stu-id="8289a-215">String</span></span>|<span data-ttu-id="8289a-216">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="8289a-216">The name of the main Lob application file.</span></span> <span data-ttu-id="8289a-217">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8289a-218">size</span><span class="sxs-lookup"><span data-stu-id="8289a-218">size</span></span>|<span data-ttu-id="8289a-219">Int64</span><span class="sxs-lookup"><span data-stu-id="8289a-219">Int64</span></span>|<span data-ttu-id="8289a-220">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="8289a-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="8289a-221">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8289a-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8289a-222">packageId</span><span class="sxs-lookup"><span data-stu-id="8289a-222">packageId</span></span>|<span data-ttu-id="8289a-223">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8289a-223">String</span></span>|<span data-ttu-id="8289a-224">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="8289a-224">The package identifier.</span></span>|
|<span data-ttu-id="8289a-225">identityName</span><span class="sxs-lookup"><span data-stu-id="8289a-225">identityName</span></span>|<span data-ttu-id="8289a-226">String</span><span class="sxs-lookup"><span data-stu-id="8289a-226">String</span></span>|<span data-ttu-id="8289a-227">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="8289a-227">The Identity Name.</span></span>|
|<span data-ttu-id="8289a-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8289a-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8289a-229">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8289a-229">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8289a-230">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="8289a-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8289a-231">versionName</span><span class="sxs-lookup"><span data-stu-id="8289a-231">versionName</span></span>|<span data-ttu-id="8289a-232">String</span><span class="sxs-lookup"><span data-stu-id="8289a-232">String</span></span>|<span data-ttu-id="8289a-233">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="8289a-233">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8289a-234">versionCode</span><span class="sxs-lookup"><span data-stu-id="8289a-234">versionCode</span></span>|<span data-ttu-id="8289a-235">String</span><span class="sxs-lookup"><span data-stu-id="8289a-235">String</span></span>|<span data-ttu-id="8289a-236">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="8289a-236">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8289a-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8289a-237">identityVersion</span></span>|<span data-ttu-id="8289a-238">String</span><span class="sxs-lookup"><span data-stu-id="8289a-238">String</span></span>|<span data-ttu-id="8289a-239">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="8289a-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8289a-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="8289a-240">Response</span></span>
<span data-ttu-id="8289a-241">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8289a-241">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8289a-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8289a-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="8289a-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8289a-243">Request</span></span>
<span data-ttu-id="8289a-244">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8289a-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1464

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

### <a name="response"></a><span data-ttu-id="8289a-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="8289a-245">Response</span></span>
<span data-ttu-id="8289a-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8289a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1636

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




