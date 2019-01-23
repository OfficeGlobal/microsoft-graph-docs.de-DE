---
title: WindowsPhoneXAP aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsPhoneXAP-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90943bafd09a31efeb6451ae91aa3f25205e0be4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421256"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="eb3b6-103">WindowsPhoneXAP aktualisieren</span><span class="sxs-lookup"><span data-stu-id="eb3b6-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="eb3b6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eb3b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb3b6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb3b6-107">Aktualisieren Sie die Eigenschaften eines [WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb3b6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb3b6-108">Prerequisites</span></span>
<span data-ttu-id="eb3b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eb3b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb3b6-111">Permission type</span></span>|<span data-ttu-id="eb3b6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb3b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb3b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb3b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb3b6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb3b6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eb3b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb3b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb3b6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb3b6-116">Not supported.</span></span>|
|<span data-ttu-id="eb3b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb3b6-117">Application</span></span>|<span data-ttu-id="eb3b6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb3b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb3b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb3b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="eb3b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb3b6-120">Request headers</span></span>
|<span data-ttu-id="eb3b6-121">Header</span><span class="sxs-lookup"><span data-stu-id="eb3b6-121">Header</span></span>|<span data-ttu-id="eb3b6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eb3b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb3b6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eb3b6-123">Authorization</span></span>|<span data-ttu-id="eb3b6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb3b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb3b6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb3b6-125">Accept</span></span>|<span data-ttu-id="eb3b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb3b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb3b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb3b6-127">Request body</span></span>
<span data-ttu-id="eb3b6-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="eb3b6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="eb3b6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb3b6-130">Property</span></span>|<span data-ttu-id="eb3b6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="eb3b6-131">Type</span></span>|<span data-ttu-id="eb3b6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb3b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb3b6-133">id</span><span class="sxs-lookup"><span data-stu-id="eb3b6-133">id</span></span>|<span data-ttu-id="eb3b6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-134">String</span></span>|<span data-ttu-id="eb3b6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eb3b6-135">Key of the entity.</span></span> <span data-ttu-id="eb3b6-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eb3b6-137">displayName</span></span>|<span data-ttu-id="eb3b6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-138">String</span></span>|<span data-ttu-id="eb3b6-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eb3b6-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-141">description</span><span class="sxs-lookup"><span data-stu-id="eb3b6-141">description</span></span>|<span data-ttu-id="eb3b6-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-142">String</span></span>|<span data-ttu-id="eb3b6-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-143">The description of the app.</span></span> <span data-ttu-id="eb3b6-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-145">publisher</span><span class="sxs-lookup"><span data-stu-id="eb3b6-145">publisher</span></span>|<span data-ttu-id="eb3b6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-146">String</span></span>|<span data-ttu-id="eb3b6-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-147">The publisher of the app.</span></span> <span data-ttu-id="eb3b6-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eb3b6-149">largeIcon</span></span>|[<span data-ttu-id="eb3b6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eb3b6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eb3b6-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eb3b6-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb3b6-153">createdDateTime</span></span>|<span data-ttu-id="eb3b6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb3b6-154">DateTimeOffset</span></span>|<span data-ttu-id="eb3b6-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-155">The date and time the app was created.</span></span> <span data-ttu-id="eb3b6-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb3b6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="eb3b6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb3b6-158">DateTimeOffset</span></span>|<span data-ttu-id="eb3b6-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="eb3b6-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eb3b6-161">isFeatured</span></span>|<span data-ttu-id="eb3b6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb3b6-162">Boolean</span></span>|<span data-ttu-id="eb3b6-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eb3b6-164">privacyInformationUrl</span></span>|<span data-ttu-id="eb3b6-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-165">String</span></span>|<span data-ttu-id="eb3b6-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-166">The privacy statement Url.</span></span> <span data-ttu-id="eb3b6-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eb3b6-168">informationUrl</span></span>|<span data-ttu-id="eb3b6-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-169">String</span></span>|<span data-ttu-id="eb3b6-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-170">The more information Url.</span></span> <span data-ttu-id="eb3b6-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-172">owner</span><span class="sxs-lookup"><span data-stu-id="eb3b6-172">owner</span></span>|<span data-ttu-id="eb3b6-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-173">String</span></span>|<span data-ttu-id="eb3b6-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-174">The owner of the app.</span></span> <span data-ttu-id="eb3b6-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-176">developer</span><span class="sxs-lookup"><span data-stu-id="eb3b6-176">developer</span></span>|<span data-ttu-id="eb3b6-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-177">String</span></span>|<span data-ttu-id="eb3b6-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-178">The developer of the app.</span></span> <span data-ttu-id="eb3b6-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-180">notes</span><span class="sxs-lookup"><span data-stu-id="eb3b6-180">notes</span></span>|<span data-ttu-id="eb3b6-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-181">String</span></span>|<span data-ttu-id="eb3b6-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-182">Notes for the app.</span></span> <span data-ttu-id="eb3b6-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="eb3b6-184">uploadState</span></span>|<span data-ttu-id="eb3b6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="eb3b6-185">Int32</span></span>|<span data-ttu-id="eb3b6-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-186">The upload state.</span></span> <span data-ttu-id="eb3b6-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="eb3b6-188">publishingState</span></span>|[<span data-ttu-id="eb3b6-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eb3b6-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eb3b6-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-190">The publishing state for the app.</span></span> <span data-ttu-id="eb3b6-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eb3b6-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eb3b6-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eb3b6-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eb3b6-194">isAssigned</span></span>|<span data-ttu-id="eb3b6-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb3b6-195">Boolean</span></span>|<span data-ttu-id="eb3b6-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="eb3b6-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eb3b6-198">roleScopeTagIds</span></span>|<span data-ttu-id="eb3b6-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="eb3b6-199">String collection</span></span>|<span data-ttu-id="eb3b6-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="eb3b6-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb3b6-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="eb3b6-202">committedContentVersion</span></span>|<span data-ttu-id="eb3b6-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-203">String</span></span>|<span data-ttu-id="eb3b6-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-204">The internal committed content version.</span></span> <span data-ttu-id="eb3b6-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eb3b6-206">fileName</span><span class="sxs-lookup"><span data-stu-id="eb3b6-206">fileName</span></span>|<span data-ttu-id="eb3b6-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-207">String</span></span>|<span data-ttu-id="eb3b6-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-208">The name of the main Lob application file.</span></span> <span data-ttu-id="eb3b6-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eb3b6-210">size</span><span class="sxs-lookup"><span data-stu-id="eb3b6-210">size</span></span>|<span data-ttu-id="eb3b6-211">Int64</span><span class="sxs-lookup"><span data-stu-id="eb3b6-211">Int64</span></span>|<span data-ttu-id="eb3b6-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="eb3b6-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eb3b6-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eb3b6-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eb3b6-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="eb3b6-215">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eb3b6-215">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="eb3b6-216">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-216">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="eb3b6-217">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="eb3b6-217">productIdentifier</span></span>|<span data-ttu-id="eb3b6-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-218">String</span></span>|<span data-ttu-id="eb3b6-219">Die Produkt-ID.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-219">The Product Identifier.</span></span>|
|<span data-ttu-id="eb3b6-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="eb3b6-220">identityVersion</span></span>|<span data-ttu-id="eb3b6-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb3b6-221">String</span></span>|<span data-ttu-id="eb3b6-222">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="eb3b6-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="eb3b6-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb3b6-223">Response</span></span>
<span data-ttu-id="eb3b6-224">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb3b6-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb3b6-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb3b6-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb3b6-226">Request</span></span>
<span data-ttu-id="eb3b6-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb3b6-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb3b6-228">Response</span></span>
<span data-ttu-id="eb3b6-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb3b6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




