---
title: webApp aktualisieren
description: Aktualisieren der Eigenschaften eines webApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 811ebeaa69e621bc25b822557784f41662596f39
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140327"
---
# <a name="update-webapp"></a><span data-ttu-id="a92d4-103">webApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a92d4-103">Update webApp</span></span>

> <span data-ttu-id="a92d4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a92d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a92d4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a92d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a92d4-106">Aktualisieren der Eigenschaften eines [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a92d4-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a92d4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a92d4-107">Prerequisites</span></span>
<span data-ttu-id="a92d4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a92d4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a92d4-110">Permission type</span></span>|<span data-ttu-id="a92d4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a92d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a92d4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a92d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a92d4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a92d4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a92d4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a92d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a92d4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a92d4-115">Not supported.</span></span>|
|<span data-ttu-id="a92d4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a92d4-116">Application</span></span>|<span data-ttu-id="a92d4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a92d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a92d4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a92d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a92d4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a92d4-119">Request headers</span></span>
|<span data-ttu-id="a92d4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a92d4-120">Header</span></span>|<span data-ttu-id="a92d4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a92d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a92d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a92d4-122">Authorization</span></span>|<span data-ttu-id="a92d4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a92d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a92d4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a92d4-124">Accept</span></span>|<span data-ttu-id="a92d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a92d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a92d4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a92d4-126">Request body</span></span>
<span data-ttu-id="a92d4-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [webApp](../resources/intune-apps-webapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a92d4-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="a92d4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [webApp](../resources/intune-apps-webapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a92d4-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="a92d4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a92d4-129">Property</span></span>|<span data-ttu-id="a92d4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a92d4-130">Type</span></span>|<span data-ttu-id="a92d4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a92d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a92d4-132">id</span><span class="sxs-lookup"><span data-stu-id="a92d4-132">id</span></span>|<span data-ttu-id="a92d4-133">string</span><span class="sxs-lookup"><span data-stu-id="a92d4-133">String</span></span>|<span data-ttu-id="a92d4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a92d4-134">Key of the entity.</span></span> <span data-ttu-id="a92d4-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a92d4-136">displayName</span></span>|<span data-ttu-id="a92d4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a92d4-137">String</span></span>|<span data-ttu-id="a92d4-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a92d4-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-140">description</span><span class="sxs-lookup"><span data-stu-id="a92d4-140">description</span></span>|<span data-ttu-id="a92d4-141">String</span><span class="sxs-lookup"><span data-stu-id="a92d4-141">String</span></span>|<span data-ttu-id="a92d4-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-142">The description of the app.</span></span> <span data-ttu-id="a92d4-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a92d4-144">publisher</span></span>|<span data-ttu-id="a92d4-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a92d4-145">String</span></span>|<span data-ttu-id="a92d4-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-146">The publisher of the app.</span></span> <span data-ttu-id="a92d4-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a92d4-148">largeIcon</span></span>|[<span data-ttu-id="a92d4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a92d4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a92d4-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a92d4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a92d4-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a92d4-152">createdDateTime</span></span>|<span data-ttu-id="a92d4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a92d4-153">DateTimeOffset</span></span>|<span data-ttu-id="a92d4-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-154">The date and time the app was created.</span></span> <span data-ttu-id="a92d4-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a92d4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a92d4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a92d4-157">DateTimeOffset</span></span>|<span data-ttu-id="a92d4-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a92d4-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a92d4-160">isFeatured</span></span>|<span data-ttu-id="a92d4-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a92d4-161">Boolean</span></span>|<span data-ttu-id="a92d4-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a92d4-163">privacyInformationUrl</span></span>|<span data-ttu-id="a92d4-164">String</span><span class="sxs-lookup"><span data-stu-id="a92d4-164">String</span></span>|<span data-ttu-id="a92d4-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="a92d4-165">The privacy statement Url.</span></span> <span data-ttu-id="a92d4-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a92d4-167">informationUrl</span></span>|<span data-ttu-id="a92d4-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a92d4-168">String</span></span>|<span data-ttu-id="a92d4-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a92d4-169">The more information Url.</span></span> <span data-ttu-id="a92d4-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-171">owner</span><span class="sxs-lookup"><span data-stu-id="a92d4-171">owner</span></span>|<span data-ttu-id="a92d4-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a92d4-172">String</span></span>|<span data-ttu-id="a92d4-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-173">The owner of the app.</span></span> <span data-ttu-id="a92d4-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-175">developer</span><span class="sxs-lookup"><span data-stu-id="a92d4-175">developer</span></span>|<span data-ttu-id="a92d4-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a92d4-176">String</span></span>|<span data-ttu-id="a92d4-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-177">The developer of the app.</span></span> <span data-ttu-id="a92d4-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-179">notes</span><span class="sxs-lookup"><span data-stu-id="a92d4-179">notes</span></span>|<span data-ttu-id="a92d4-180">String</span><span class="sxs-lookup"><span data-stu-id="a92d4-180">String</span></span>|<span data-ttu-id="a92d4-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-181">Notes for the app.</span></span> <span data-ttu-id="a92d4-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a92d4-183">uploadState</span></span>|<span data-ttu-id="a92d4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a92d4-184">Int32</span></span>|<span data-ttu-id="a92d4-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="a92d4-185">The upload state.</span></span> <span data-ttu-id="a92d4-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a92d4-187">publishingState</span></span>|[<span data-ttu-id="a92d4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a92d4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a92d4-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-189">The publishing state for the app.</span></span> <span data-ttu-id="a92d4-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a92d4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a92d4-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a92d4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a92d4-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a92d4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a92d4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a92d4-193">isAssigned</span></span>|<span data-ttu-id="a92d4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a92d4-194">Boolean</span></span>|<span data-ttu-id="a92d4-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="a92d4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a92d4-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="a92d4-197">roleScopeTagIds</span></span>|<span data-ttu-id="a92d4-198">String collection</span><span class="sxs-lookup"><span data-stu-id="a92d4-198">String collection</span></span>|<span data-ttu-id="a92d4-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a92d4-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a92d4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a92d4-201">appUrl</span><span class="sxs-lookup"><span data-stu-id="a92d4-201">appUrl</span></span>|<span data-ttu-id="a92d4-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a92d4-202">String</span></span>|<span data-ttu-id="a92d4-203">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="a92d4-203">The web app URL.</span></span>|
|<span data-ttu-id="a92d4-204">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="a92d4-204">useManagedBrowser</span></span>|<span data-ttu-id="a92d4-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a92d4-205">Boolean</span></span>|<span data-ttu-id="a92d4-206">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a92d4-206">Whether or not to use managed browser.</span></span> <span data-ttu-id="a92d4-207">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="a92d4-207">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="a92d4-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="a92d4-208">Response</span></span>
<span data-ttu-id="a92d4-209">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a92d4-209">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a92d4-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a92d4-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="a92d4-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a92d4-211">Request</span></span>
<span data-ttu-id="a92d4-212">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a92d4-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 752

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="a92d4-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="a92d4-213">Response</span></span>
<span data-ttu-id="a92d4-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a92d4-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 924

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




