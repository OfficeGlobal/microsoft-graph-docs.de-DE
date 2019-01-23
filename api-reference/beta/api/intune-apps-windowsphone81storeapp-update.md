---
title: WindowsPhone81StoreApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81StoreApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bcbfcb70d6f97b1a25aebad24b4cd3f0de43c7d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394124"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="b1b06-103">WindowsPhone81StoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b1b06-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="b1b06-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b1b06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1b06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1b06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1b06-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1b06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1b06-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1b06-107">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1b06-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1b06-108">Prerequisites</span></span>
<span data-ttu-id="b1b06-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1b06-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1b06-111">Permission type</span></span>|<span data-ttu-id="b1b06-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1b06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1b06-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1b06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1b06-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b06-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1b06-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1b06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1b06-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1b06-116">Not supported.</span></span>|
|<span data-ttu-id="b1b06-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1b06-117">Application</span></span>|<span data-ttu-id="b1b06-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1b06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1b06-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1b06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b1b06-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1b06-120">Request headers</span></span>
|<span data-ttu-id="b1b06-121">Header</span><span class="sxs-lookup"><span data-stu-id="b1b06-121">Header</span></span>|<span data-ttu-id="b1b06-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b1b06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1b06-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b1b06-123">Authorization</span></span>|<span data-ttu-id="b1b06-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1b06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1b06-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b1b06-125">Accept</span></span>|<span data-ttu-id="b1b06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1b06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1b06-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1b06-127">Request body</span></span>
<span data-ttu-id="b1b06-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b1b06-128">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="b1b06-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b1b06-129">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="b1b06-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1b06-130">Property</span></span>|<span data-ttu-id="b1b06-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b1b06-131">Type</span></span>|<span data-ttu-id="b1b06-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1b06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b06-133">id</span><span class="sxs-lookup"><span data-stu-id="b1b06-133">id</span></span>|<span data-ttu-id="b1b06-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-134">String</span></span>|<span data-ttu-id="b1b06-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b1b06-135">Key of the entity.</span></span> <span data-ttu-id="b1b06-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b1b06-137">displayName</span></span>|<span data-ttu-id="b1b06-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-138">String</span></span>|<span data-ttu-id="b1b06-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b1b06-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-141">description</span><span class="sxs-lookup"><span data-stu-id="b1b06-141">description</span></span>|<span data-ttu-id="b1b06-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-142">String</span></span>|<span data-ttu-id="b1b06-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-143">The description of the app.</span></span> <span data-ttu-id="b1b06-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b1b06-145">publisher</span></span>|<span data-ttu-id="b1b06-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-146">String</span></span>|<span data-ttu-id="b1b06-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-147">The publisher of the app.</span></span> <span data-ttu-id="b1b06-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b1b06-149">largeIcon</span></span>|[<span data-ttu-id="b1b06-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b1b06-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b1b06-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b1b06-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b1b06-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b06-153">createdDateTime</span></span>|<span data-ttu-id="b1b06-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b06-154">DateTimeOffset</span></span>|<span data-ttu-id="b1b06-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-155">The date and time the app was created.</span></span> <span data-ttu-id="b1b06-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b06-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b1b06-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b06-158">DateTimeOffset</span></span>|<span data-ttu-id="b1b06-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b1b06-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b1b06-161">isFeatured</span></span>|<span data-ttu-id="b1b06-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1b06-162">Boolean</span></span>|<span data-ttu-id="b1b06-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b1b06-164">privacyInformationUrl</span></span>|<span data-ttu-id="b1b06-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-165">String</span></span>|<span data-ttu-id="b1b06-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="b1b06-166">The privacy statement Url.</span></span> <span data-ttu-id="b1b06-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b1b06-168">informationUrl</span></span>|<span data-ttu-id="b1b06-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-169">String</span></span>|<span data-ttu-id="b1b06-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="b1b06-170">The more information Url.</span></span> <span data-ttu-id="b1b06-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-172">owner</span><span class="sxs-lookup"><span data-stu-id="b1b06-172">owner</span></span>|<span data-ttu-id="b1b06-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-173">String</span></span>|<span data-ttu-id="b1b06-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-174">The owner of the app.</span></span> <span data-ttu-id="b1b06-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-176">developer</span><span class="sxs-lookup"><span data-stu-id="b1b06-176">developer</span></span>|<span data-ttu-id="b1b06-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-177">String</span></span>|<span data-ttu-id="b1b06-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-178">The developer of the app.</span></span> <span data-ttu-id="b1b06-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-180">notes</span><span class="sxs-lookup"><span data-stu-id="b1b06-180">notes</span></span>|<span data-ttu-id="b1b06-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-181">String</span></span>|<span data-ttu-id="b1b06-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-182">Notes for the app.</span></span> <span data-ttu-id="b1b06-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b1b06-184">uploadState</span></span>|<span data-ttu-id="b1b06-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b06-185">Int32</span></span>|<span data-ttu-id="b1b06-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="b1b06-186">The upload state.</span></span> <span data-ttu-id="b1b06-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b1b06-188">publishingState</span></span>|[<span data-ttu-id="b1b06-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b1b06-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b1b06-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="b1b06-190">The publishing state for the app.</span></span> <span data-ttu-id="b1b06-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="b1b06-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b1b06-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b1b06-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="b1b06-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b1b06-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b1b06-194">isAssigned</span></span>|<span data-ttu-id="b1b06-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1b06-195">Boolean</span></span>|<span data-ttu-id="b1b06-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b1b06-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b1b06-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1b06-198">roleScopeTagIds</span></span>|<span data-ttu-id="b1b06-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b1b06-199">String collection</span></span>|<span data-ttu-id="b1b06-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="b1b06-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b1b06-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1b06-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1b06-202">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b1b06-202">appStoreUrl</span></span>|<span data-ttu-id="b1b06-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1b06-203">String</span></span>|<span data-ttu-id="b1b06-204">Die URL der 8.1 für Windows Phone-app-Store.</span><span class="sxs-lookup"><span data-stu-id="b1b06-204">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="b1b06-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1b06-205">Response</span></span>
<span data-ttu-id="b1b06-206">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b1b06-206">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b06-207">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1b06-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1b06-208">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1b06-208">Request</span></span>
<span data-ttu-id="b1b06-209">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1b06-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="b1b06-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1b06-210">Response</span></span>
<span data-ttu-id="b1b06-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1b06-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 920

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




