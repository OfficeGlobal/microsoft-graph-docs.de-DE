---
title: WindowsPhoneXAP aktualisieren
description: Aktualisieren der Eigenschaften eines windowsPhoneXAP-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 096e7430d0f1e544b5fbd4a9475b70e45ecb0719
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150036"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="8bc26-103">WindowsPhoneXAP aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8bc26-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="8bc26-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bc26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc26-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8bc26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc26-106">Aktualisieren der Eigenschaften eines [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bc26-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bc26-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8bc26-107">Prerequisites</span></span>
<span data-ttu-id="8bc26-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8bc26-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8bc26-110">Permission type</span></span>|<span data-ttu-id="8bc26-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8bc26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bc26-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8bc26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bc26-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bc26-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8bc26-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8bc26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bc26-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bc26-115">Not supported.</span></span>|
|<span data-ttu-id="8bc26-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8bc26-116">Application</span></span>|<span data-ttu-id="8bc26-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bc26-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bc26-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bc26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8bc26-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8bc26-119">Request headers</span></span>
|<span data-ttu-id="8bc26-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8bc26-120">Header</span></span>|<span data-ttu-id="8bc26-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8bc26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bc26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bc26-122">Authorization</span></span>|<span data-ttu-id="8bc26-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8bc26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bc26-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8bc26-124">Accept</span></span>|<span data-ttu-id="8bc26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bc26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bc26-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8bc26-126">Request body</span></span>
<span data-ttu-id="8bc26-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8bc26-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="8bc26-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8bc26-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="8bc26-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8bc26-129">Property</span></span>|<span data-ttu-id="8bc26-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8bc26-130">Type</span></span>|<span data-ttu-id="8bc26-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bc26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc26-132">id</span><span class="sxs-lookup"><span data-stu-id="8bc26-132">id</span></span>|<span data-ttu-id="8bc26-133">string</span><span class="sxs-lookup"><span data-stu-id="8bc26-133">String</span></span>|<span data-ttu-id="8bc26-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8bc26-134">Key of the entity.</span></span> <span data-ttu-id="8bc26-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8bc26-136">displayName</span></span>|<span data-ttu-id="8bc26-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-137">String</span></span>|<span data-ttu-id="8bc26-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8bc26-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-140">description</span><span class="sxs-lookup"><span data-stu-id="8bc26-140">description</span></span>|<span data-ttu-id="8bc26-141">String</span><span class="sxs-lookup"><span data-stu-id="8bc26-141">String</span></span>|<span data-ttu-id="8bc26-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-142">The description of the app.</span></span> <span data-ttu-id="8bc26-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8bc26-144">publisher</span></span>|<span data-ttu-id="8bc26-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-145">String</span></span>|<span data-ttu-id="8bc26-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-146">The publisher of the app.</span></span> <span data-ttu-id="8bc26-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8bc26-148">largeIcon</span></span>|[<span data-ttu-id="8bc26-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8bc26-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8bc26-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8bc26-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8bc26-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc26-152">createdDateTime</span></span>|<span data-ttu-id="8bc26-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc26-153">DateTimeOffset</span></span>|<span data-ttu-id="8bc26-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-154">The date and time the app was created.</span></span> <span data-ttu-id="8bc26-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc26-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8bc26-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc26-157">DateTimeOffset</span></span>|<span data-ttu-id="8bc26-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8bc26-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8bc26-160">isFeatured</span></span>|<span data-ttu-id="8bc26-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bc26-161">Boolean</span></span>|<span data-ttu-id="8bc26-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8bc26-163">privacyInformationUrl</span></span>|<span data-ttu-id="8bc26-164">String</span><span class="sxs-lookup"><span data-stu-id="8bc26-164">String</span></span>|<span data-ttu-id="8bc26-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="8bc26-165">The privacy statement Url.</span></span> <span data-ttu-id="8bc26-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8bc26-167">informationUrl</span></span>|<span data-ttu-id="8bc26-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-168">String</span></span>|<span data-ttu-id="8bc26-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8bc26-169">The more information Url.</span></span> <span data-ttu-id="8bc26-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-171">owner</span><span class="sxs-lookup"><span data-stu-id="8bc26-171">owner</span></span>|<span data-ttu-id="8bc26-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-172">String</span></span>|<span data-ttu-id="8bc26-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-173">The owner of the app.</span></span> <span data-ttu-id="8bc26-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-175">developer</span><span class="sxs-lookup"><span data-stu-id="8bc26-175">developer</span></span>|<span data-ttu-id="8bc26-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-176">String</span></span>|<span data-ttu-id="8bc26-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-177">The developer of the app.</span></span> <span data-ttu-id="8bc26-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-179">notes</span><span class="sxs-lookup"><span data-stu-id="8bc26-179">notes</span></span>|<span data-ttu-id="8bc26-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-180">String</span></span>|<span data-ttu-id="8bc26-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-181">Notes for the app.</span></span> <span data-ttu-id="8bc26-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8bc26-183">uploadState</span></span>|<span data-ttu-id="8bc26-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8bc26-184">Int32</span></span>|<span data-ttu-id="8bc26-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="8bc26-185">The upload state.</span></span> <span data-ttu-id="8bc26-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8bc26-187">publishingState</span></span>|[<span data-ttu-id="8bc26-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8bc26-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8bc26-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-189">The publishing state for the app.</span></span> <span data-ttu-id="8bc26-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="8bc26-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8bc26-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="8bc26-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8bc26-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="8bc26-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8bc26-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8bc26-193">isAssigned</span></span>|<span data-ttu-id="8bc26-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bc26-194">Boolean</span></span>|<span data-ttu-id="8bc26-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="8bc26-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8bc26-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="8bc26-197">roleScopeTagIds</span></span>|<span data-ttu-id="8bc26-198">String collection</span><span class="sxs-lookup"><span data-stu-id="8bc26-198">String collection</span></span>|<span data-ttu-id="8bc26-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="8bc26-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8bc26-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8bc26-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8bc26-201">committedContentVersion</span></span>|<span data-ttu-id="8bc26-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-202">String</span></span>|<span data-ttu-id="8bc26-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="8bc26-203">The internal committed content version.</span></span> <span data-ttu-id="8bc26-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8bc26-205">fileName</span><span class="sxs-lookup"><span data-stu-id="8bc26-205">fileName</span></span>|<span data-ttu-id="8bc26-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-206">String</span></span>|<span data-ttu-id="8bc26-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="8bc26-207">The name of the main Lob application file.</span></span> <span data-ttu-id="8bc26-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8bc26-209">size</span><span class="sxs-lookup"><span data-stu-id="8bc26-209">size</span></span>|<span data-ttu-id="8bc26-210">Int64</span><span class="sxs-lookup"><span data-stu-id="8bc26-210">Int64</span></span>|<span data-ttu-id="8bc26-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="8bc26-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="8bc26-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bc26-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8bc26-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8bc26-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8bc26-214">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8bc26-214">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="8bc26-215">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="8bc26-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8bc26-216">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="8bc26-216">productIdentifier</span></span>|<span data-ttu-id="8bc26-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-217">String</span></span>|<span data-ttu-id="8bc26-218">Der Product Identifier.</span><span class="sxs-lookup"><span data-stu-id="8bc26-218">The Product Identifier.</span></span>|
|<span data-ttu-id="8bc26-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8bc26-219">identityVersion</span></span>|<span data-ttu-id="8bc26-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bc26-220">String</span></span>|<span data-ttu-id="8bc26-221">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="8bc26-221">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8bc26-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bc26-222">Response</span></span>
<span data-ttu-id="8bc26-223">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8bc26-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bc26-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8bc26-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bc26-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bc26-225">Request</span></span>
<span data-ttu-id="8bc26-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8bc26-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1164

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

### <a name="response"></a><span data-ttu-id="8bc26-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bc26-227">Response</span></span>
<span data-ttu-id="8bc26-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8bc26-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1336

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




