---
title: WindowsAppX aktualisieren
description: Aktualisieren der Eigenschaften eines windowsAppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5abc2a461019ad7970d6b4c500e2c593b9c4aa7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141230"
---
# <a name="update-windowsappx"></a><span data-ttu-id="7f25e-103">WindowsAppX aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7f25e-103">Update windowsAppX</span></span>

> <span data-ttu-id="7f25e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f25e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f25e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7f25e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f25e-106">Aktualisieren der Eigenschaften eines [windowsAppX](../resources/intune-apps-windowsappx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7f25e-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f25e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7f25e-107">Prerequisites</span></span>
<span data-ttu-id="7f25e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7f25e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f25e-110">Permission type</span></span>|<span data-ttu-id="7f25e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f25e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f25e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f25e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f25e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f25e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f25e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f25e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f25e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f25e-115">Not supported.</span></span>|
|<span data-ttu-id="7f25e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f25e-116">Application</span></span>|<span data-ttu-id="7f25e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f25e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f25e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f25e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7f25e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f25e-119">Request headers</span></span>
|<span data-ttu-id="7f25e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7f25e-120">Header</span></span>|<span data-ttu-id="7f25e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7f25e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f25e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f25e-122">Authorization</span></span>|<span data-ttu-id="7f25e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7f25e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f25e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7f25e-124">Accept</span></span>|<span data-ttu-id="7f25e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f25e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f25e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f25e-126">Request body</span></span>
<span data-ttu-id="7f25e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsAppX](../resources/intune-apps-windowsappx.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7f25e-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="7f25e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsAppX](../resources/intune-apps-windowsappx.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7f25e-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="7f25e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f25e-129">Property</span></span>|<span data-ttu-id="7f25e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7f25e-130">Type</span></span>|<span data-ttu-id="7f25e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f25e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f25e-132">id</span><span class="sxs-lookup"><span data-stu-id="7f25e-132">id</span></span>|<span data-ttu-id="7f25e-133">string</span><span class="sxs-lookup"><span data-stu-id="7f25e-133">String</span></span>|<span data-ttu-id="7f25e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7f25e-134">Key of the entity.</span></span> <span data-ttu-id="7f25e-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7f25e-136">displayName</span></span>|<span data-ttu-id="7f25e-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-137">String</span></span>|<span data-ttu-id="7f25e-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7f25e-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-140">description</span><span class="sxs-lookup"><span data-stu-id="7f25e-140">description</span></span>|<span data-ttu-id="7f25e-141">String</span><span class="sxs-lookup"><span data-stu-id="7f25e-141">String</span></span>|<span data-ttu-id="7f25e-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-142">The description of the app.</span></span> <span data-ttu-id="7f25e-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7f25e-144">publisher</span></span>|<span data-ttu-id="7f25e-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-145">String</span></span>|<span data-ttu-id="7f25e-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-146">The publisher of the app.</span></span> <span data-ttu-id="7f25e-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7f25e-148">largeIcon</span></span>|[<span data-ttu-id="7f25e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7f25e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7f25e-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7f25e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7f25e-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f25e-152">createdDateTime</span></span>|<span data-ttu-id="7f25e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f25e-153">DateTimeOffset</span></span>|<span data-ttu-id="7f25e-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-154">The date and time the app was created.</span></span> <span data-ttu-id="7f25e-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f25e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7f25e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f25e-157">DateTimeOffset</span></span>|<span data-ttu-id="7f25e-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7f25e-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7f25e-160">isFeatured</span></span>|<span data-ttu-id="7f25e-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f25e-161">Boolean</span></span>|<span data-ttu-id="7f25e-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7f25e-163">privacyInformationUrl</span></span>|<span data-ttu-id="7f25e-164">String</span><span class="sxs-lookup"><span data-stu-id="7f25e-164">String</span></span>|<span data-ttu-id="7f25e-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="7f25e-165">The privacy statement Url.</span></span> <span data-ttu-id="7f25e-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7f25e-167">informationUrl</span></span>|<span data-ttu-id="7f25e-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-168">String</span></span>|<span data-ttu-id="7f25e-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="7f25e-169">The more information Url.</span></span> <span data-ttu-id="7f25e-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-171">owner</span><span class="sxs-lookup"><span data-stu-id="7f25e-171">owner</span></span>|<span data-ttu-id="7f25e-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-172">String</span></span>|<span data-ttu-id="7f25e-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-173">The owner of the app.</span></span> <span data-ttu-id="7f25e-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-175">developer</span><span class="sxs-lookup"><span data-stu-id="7f25e-175">developer</span></span>|<span data-ttu-id="7f25e-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-176">String</span></span>|<span data-ttu-id="7f25e-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-177">The developer of the app.</span></span> <span data-ttu-id="7f25e-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-179">notes</span><span class="sxs-lookup"><span data-stu-id="7f25e-179">notes</span></span>|<span data-ttu-id="7f25e-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-180">String</span></span>|<span data-ttu-id="7f25e-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-181">Notes for the app.</span></span> <span data-ttu-id="7f25e-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7f25e-183">uploadState</span></span>|<span data-ttu-id="7f25e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7f25e-184">Int32</span></span>|<span data-ttu-id="7f25e-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="7f25e-185">The upload state.</span></span> <span data-ttu-id="7f25e-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7f25e-187">publishingState</span></span>|[<span data-ttu-id="7f25e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7f25e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7f25e-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-189">The publishing state for the app.</span></span> <span data-ttu-id="7f25e-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="7f25e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7f25e-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="7f25e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7f25e-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="7f25e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7f25e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7f25e-193">isAssigned</span></span>|<span data-ttu-id="7f25e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f25e-194">Boolean</span></span>|<span data-ttu-id="7f25e-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="7f25e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7f25e-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="7f25e-197">roleScopeTagIds</span></span>|<span data-ttu-id="7f25e-198">String collection</span><span class="sxs-lookup"><span data-stu-id="7f25e-198">String collection</span></span>|<span data-ttu-id="7f25e-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="7f25e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7f25e-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f25e-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7f25e-201">committedContentVersion</span></span>|<span data-ttu-id="7f25e-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-202">String</span></span>|<span data-ttu-id="7f25e-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="7f25e-203">The internal committed content version.</span></span> <span data-ttu-id="7f25e-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7f25e-205">fileName</span><span class="sxs-lookup"><span data-stu-id="7f25e-205">fileName</span></span>|<span data-ttu-id="7f25e-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-206">String</span></span>|<span data-ttu-id="7f25e-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="7f25e-207">The name of the main Lob application file.</span></span> <span data-ttu-id="7f25e-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7f25e-209">size</span><span class="sxs-lookup"><span data-stu-id="7f25e-209">size</span></span>|<span data-ttu-id="7f25e-210">Int64</span><span class="sxs-lookup"><span data-stu-id="7f25e-210">Int64</span></span>|<span data-ttu-id="7f25e-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="7f25e-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="7f25e-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f25e-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7f25e-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7f25e-213">applicableArchitectures</span></span>|[<span data-ttu-id="7f25e-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7f25e-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7f25e-215">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="7f25e-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7f25e-216">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7f25e-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7f25e-217">identityName</span><span class="sxs-lookup"><span data-stu-id="7f25e-217">identityName</span></span>|<span data-ttu-id="7f25e-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-218">String</span></span>|<span data-ttu-id="7f25e-219">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="7f25e-219">The Identity Name.</span></span>|
|<span data-ttu-id="7f25e-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="7f25e-220">identityPublisherHash</span></span>|<span data-ttu-id="7f25e-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-221">String</span></span>|<span data-ttu-id="7f25e-222">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="7f25e-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="7f25e-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f25e-223">identityResourceIdentifier</span></span>|<span data-ttu-id="7f25e-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-224">String</span></span>|<span data-ttu-id="7f25e-225">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="7f25e-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7f25e-226">isBundle</span><span class="sxs-lookup"><span data-stu-id="7f25e-226">isBundle</span></span>|<span data-ttu-id="7f25e-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f25e-227">Boolean</span></span>|<span data-ttu-id="7f25e-228">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="7f25e-228">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="7f25e-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7f25e-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7f25e-230">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7f25e-230">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7f25e-231">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="7f25e-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7f25e-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7f25e-232">identityVersion</span></span>|<span data-ttu-id="7f25e-233">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f25e-233">String</span></span>|<span data-ttu-id="7f25e-234">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="7f25e-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7f25e-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f25e-235">Response</span></span>
<span data-ttu-id="7f25e-236">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsAppX](../resources/intune-apps-windowsappx.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7f25e-236">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f25e-237">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f25e-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f25e-238">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f25e-238">Request</span></span>
<span data-ttu-id="7f25e-239">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f25e-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="7f25e-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f25e-240">Response</span></span>
<span data-ttu-id="7f25e-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f25e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```




