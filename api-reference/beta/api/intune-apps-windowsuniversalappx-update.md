---
title: windowsUniversalAppX aktualisieren
description: Aktualisieren der Eigenschaften eines windowsUniversalAppX-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe87fe726fc20fadbfb915647f2fd972c3389c29
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424413"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="54fae-103">windowsUniversalAppX aktualisieren</span><span class="sxs-lookup"><span data-stu-id="54fae-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="54fae-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="54fae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54fae-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54fae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54fae-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="54fae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54fae-107">Aktualisieren der Eigenschaften eines [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="54fae-107">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54fae-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54fae-108">Prerequisites</span></span>
<span data-ttu-id="54fae-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54fae-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54fae-111">Permission type</span></span>|<span data-ttu-id="54fae-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54fae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54fae-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54fae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54fae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54fae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54fae-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54fae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54fae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54fae-116">Not supported.</span></span>|
|<span data-ttu-id="54fae-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54fae-117">Application</span></span>|<span data-ttu-id="54fae-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54fae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54fae-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54fae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="54fae-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54fae-120">Request headers</span></span>
|<span data-ttu-id="54fae-121">Header</span><span class="sxs-lookup"><span data-stu-id="54fae-121">Header</span></span>|<span data-ttu-id="54fae-122">Wert</span><span class="sxs-lookup"><span data-stu-id="54fae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54fae-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="54fae-123">Authorization</span></span>|<span data-ttu-id="54fae-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54fae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54fae-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="54fae-125">Accept</span></span>|<span data-ttu-id="54fae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54fae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54fae-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54fae-127">Request body</span></span>
<span data-ttu-id="54fae-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="54fae-128">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="54fae-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="54fae-129">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="54fae-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54fae-130">Property</span></span>|<span data-ttu-id="54fae-131">Typ</span><span class="sxs-lookup"><span data-stu-id="54fae-131">Type</span></span>|<span data-ttu-id="54fae-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54fae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54fae-133">id</span><span class="sxs-lookup"><span data-stu-id="54fae-133">id</span></span>|<span data-ttu-id="54fae-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-134">String</span></span>|<span data-ttu-id="54fae-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="54fae-135">Key of the entity.</span></span> <span data-ttu-id="54fae-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-137">displayName</span><span class="sxs-lookup"><span data-stu-id="54fae-137">displayName</span></span>|<span data-ttu-id="54fae-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-138">String</span></span>|<span data-ttu-id="54fae-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="54fae-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-141">description</span><span class="sxs-lookup"><span data-stu-id="54fae-141">description</span></span>|<span data-ttu-id="54fae-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-142">String</span></span>|<span data-ttu-id="54fae-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-143">The description of the app.</span></span> <span data-ttu-id="54fae-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-145">publisher</span><span class="sxs-lookup"><span data-stu-id="54fae-145">publisher</span></span>|<span data-ttu-id="54fae-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-146">String</span></span>|<span data-ttu-id="54fae-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-147">The publisher of the app.</span></span> <span data-ttu-id="54fae-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="54fae-149">largeIcon</span></span>|[<span data-ttu-id="54fae-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="54fae-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="54fae-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="54fae-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="54fae-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54fae-153">createdDateTime</span></span>|<span data-ttu-id="54fae-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54fae-154">DateTimeOffset</span></span>|<span data-ttu-id="54fae-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-155">The date and time the app was created.</span></span> <span data-ttu-id="54fae-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54fae-157">lastModifiedDateTime</span></span>|<span data-ttu-id="54fae-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54fae-158">DateTimeOffset</span></span>|<span data-ttu-id="54fae-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-159">The date and time the app was last modified.</span></span> <span data-ttu-id="54fae-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="54fae-161">isFeatured</span></span>|<span data-ttu-id="54fae-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fae-162">Boolean</span></span>|<span data-ttu-id="54fae-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="54fae-164">privacyInformationUrl</span></span>|<span data-ttu-id="54fae-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-165">String</span></span>|<span data-ttu-id="54fae-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="54fae-166">The privacy statement Url.</span></span> <span data-ttu-id="54fae-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="54fae-168">informationUrl</span></span>|<span data-ttu-id="54fae-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-169">String</span></span>|<span data-ttu-id="54fae-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="54fae-170">The more information Url.</span></span> <span data-ttu-id="54fae-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-172">owner</span><span class="sxs-lookup"><span data-stu-id="54fae-172">owner</span></span>|<span data-ttu-id="54fae-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-173">String</span></span>|<span data-ttu-id="54fae-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-174">The owner of the app.</span></span> <span data-ttu-id="54fae-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-176">developer</span><span class="sxs-lookup"><span data-stu-id="54fae-176">developer</span></span>|<span data-ttu-id="54fae-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-177">String</span></span>|<span data-ttu-id="54fae-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-178">The developer of the app.</span></span> <span data-ttu-id="54fae-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-180">notes</span><span class="sxs-lookup"><span data-stu-id="54fae-180">notes</span></span>|<span data-ttu-id="54fae-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-181">String</span></span>|<span data-ttu-id="54fae-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="54fae-182">Notes for the app.</span></span> <span data-ttu-id="54fae-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="54fae-184">uploadState</span></span>|<span data-ttu-id="54fae-185">Int32</span><span class="sxs-lookup"><span data-stu-id="54fae-185">Int32</span></span>|<span data-ttu-id="54fae-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="54fae-186">The upload state.</span></span> <span data-ttu-id="54fae-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="54fae-188">publishingState</span></span>|[<span data-ttu-id="54fae-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="54fae-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="54fae-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="54fae-190">The publishing state for the app.</span></span> <span data-ttu-id="54fae-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="54fae-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="54fae-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="54fae-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="54fae-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="54fae-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="54fae-194">isAssigned</span></span>|<span data-ttu-id="54fae-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fae-195">Boolean</span></span>|<span data-ttu-id="54fae-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="54fae-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="54fae-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54fae-198">roleScopeTagIds</span></span>|<span data-ttu-id="54fae-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="54fae-199">String collection</span></span>|<span data-ttu-id="54fae-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="54fae-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="54fae-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54fae-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="54fae-202">committedContentVersion</span></span>|<span data-ttu-id="54fae-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-203">String</span></span>|<span data-ttu-id="54fae-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="54fae-204">The internal committed content version.</span></span> <span data-ttu-id="54fae-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54fae-206">fileName</span><span class="sxs-lookup"><span data-stu-id="54fae-206">fileName</span></span>|<span data-ttu-id="54fae-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-207">String</span></span>|<span data-ttu-id="54fae-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="54fae-208">The name of the main Lob application file.</span></span> <span data-ttu-id="54fae-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54fae-210">size</span><span class="sxs-lookup"><span data-stu-id="54fae-210">size</span></span>|<span data-ttu-id="54fae-211">Int64</span><span class="sxs-lookup"><span data-stu-id="54fae-211">Int64</span></span>|<span data-ttu-id="54fae-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="54fae-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="54fae-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54fae-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54fae-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="54fae-214">applicableArchitectures</span></span>|[<span data-ttu-id="54fae-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="54fae-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="54fae-216">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="54fae-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="54fae-217">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="54fae-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="54fae-218">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="54fae-218">applicableDeviceTypes</span></span>|[<span data-ttu-id="54fae-219">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="54fae-219">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="54fae-220">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="54fae-220">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="54fae-221">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="54fae-221">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="54fae-222">identityName</span><span class="sxs-lookup"><span data-stu-id="54fae-222">identityName</span></span>|<span data-ttu-id="54fae-223">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-223">String</span></span>|<span data-ttu-id="54fae-224">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="54fae-224">The Identity Name.</span></span>|
|<span data-ttu-id="54fae-225">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="54fae-225">identityPublisherHash</span></span>|<span data-ttu-id="54fae-226">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-226">String</span></span>|<span data-ttu-id="54fae-227">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="54fae-227">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="54fae-228">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="54fae-228">identityResourceIdentifier</span></span>|<span data-ttu-id="54fae-229">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-229">String</span></span>|<span data-ttu-id="54fae-230">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="54fae-230">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="54fae-231">isBundle</span><span class="sxs-lookup"><span data-stu-id="54fae-231">isBundle</span></span>|<span data-ttu-id="54fae-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fae-232">Boolean</span></span>|<span data-ttu-id="54fae-233">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="54fae-233">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="54fae-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54fae-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="54fae-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54fae-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="54fae-236">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="54fae-236">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="54fae-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="54fae-237">identityVersion</span></span>|<span data-ttu-id="54fae-238">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fae-238">String</span></span>|<span data-ttu-id="54fae-239">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="54fae-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="54fae-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="54fae-240">Response</span></span>
<span data-ttu-id="54fae-241">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="54fae-241">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54fae-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54fae-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="54fae-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54fae-243">Request</span></span>
<span data-ttu-id="54fae-244">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54fae-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1388

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
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

### <a name="response"></a><span data-ttu-id="54fae-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="54fae-245">Response</span></span>
<span data-ttu-id="54fae-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54fae-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1560

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
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




