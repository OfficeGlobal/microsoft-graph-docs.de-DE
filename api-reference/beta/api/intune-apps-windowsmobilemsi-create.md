---
title: Erstellen von „windowsMobileMSI“
description: Erstellen eines neuen windowsMobileMSI-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a794ea35428b606c825dc95de3a76aa839708489
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405114"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="49e59-103">Erstellen von „windowsMobileMSI“</span><span class="sxs-lookup"><span data-stu-id="49e59-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="49e59-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="49e59-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49e59-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49e59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49e59-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49e59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49e59-107">Erstellen eines neuen [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="49e59-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49e59-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="49e59-108">Prerequisites</span></span>
<span data-ttu-id="49e59-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49e59-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49e59-111">Permission type</span></span>|<span data-ttu-id="49e59-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49e59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49e59-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49e59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49e59-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e59-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="49e59-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49e59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49e59-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49e59-116">Not supported.</span></span>|
|<span data-ttu-id="49e59-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49e59-117">Application</span></span>|<span data-ttu-id="49e59-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49e59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49e59-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49e59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="49e59-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49e59-120">Request headers</span></span>
|<span data-ttu-id="49e59-121">Header</span><span class="sxs-lookup"><span data-stu-id="49e59-121">Header</span></span>|<span data-ttu-id="49e59-122">Wert</span><span class="sxs-lookup"><span data-stu-id="49e59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49e59-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="49e59-123">Authorization</span></span>|<span data-ttu-id="49e59-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="49e59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49e59-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="49e59-125">Accept</span></span>|<span data-ttu-id="49e59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49e59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49e59-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49e59-127">Request body</span></span>
<span data-ttu-id="49e59-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsMobileMSI-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="49e59-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="49e59-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsMobileMSI erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="49e59-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="49e59-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49e59-130">Property</span></span>|<span data-ttu-id="49e59-131">Typ</span><span class="sxs-lookup"><span data-stu-id="49e59-131">Type</span></span>|<span data-ttu-id="49e59-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49e59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e59-133">id</span><span class="sxs-lookup"><span data-stu-id="49e59-133">id</span></span>|<span data-ttu-id="49e59-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-134">String</span></span>|<span data-ttu-id="49e59-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="49e59-135">Key of the entity.</span></span> <span data-ttu-id="49e59-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-137">displayName</span><span class="sxs-lookup"><span data-stu-id="49e59-137">displayName</span></span>|<span data-ttu-id="49e59-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-138">String</span></span>|<span data-ttu-id="49e59-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="49e59-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-141">description</span><span class="sxs-lookup"><span data-stu-id="49e59-141">description</span></span>|<span data-ttu-id="49e59-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-142">String</span></span>|<span data-ttu-id="49e59-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-143">The description of the app.</span></span> <span data-ttu-id="49e59-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-145">publisher</span><span class="sxs-lookup"><span data-stu-id="49e59-145">publisher</span></span>|<span data-ttu-id="49e59-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-146">String</span></span>|<span data-ttu-id="49e59-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-147">The publisher of the app.</span></span> <span data-ttu-id="49e59-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="49e59-149">largeIcon</span></span>|[<span data-ttu-id="49e59-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="49e59-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="49e59-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="49e59-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="49e59-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49e59-153">createdDateTime</span></span>|<span data-ttu-id="49e59-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e59-154">DateTimeOffset</span></span>|<span data-ttu-id="49e59-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-155">The date and time the app was created.</span></span> <span data-ttu-id="49e59-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49e59-157">lastModifiedDateTime</span></span>|<span data-ttu-id="49e59-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e59-158">DateTimeOffset</span></span>|<span data-ttu-id="49e59-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-159">The date and time the app was last modified.</span></span> <span data-ttu-id="49e59-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="49e59-161">isFeatured</span></span>|<span data-ttu-id="49e59-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e59-162">Boolean</span></span>|<span data-ttu-id="49e59-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="49e59-164">privacyInformationUrl</span></span>|<span data-ttu-id="49e59-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-165">String</span></span>|<span data-ttu-id="49e59-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="49e59-166">The privacy statement Url.</span></span> <span data-ttu-id="49e59-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="49e59-168">informationUrl</span></span>|<span data-ttu-id="49e59-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-169">String</span></span>|<span data-ttu-id="49e59-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="49e59-170">The more information Url.</span></span> <span data-ttu-id="49e59-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-172">owner</span><span class="sxs-lookup"><span data-stu-id="49e59-172">owner</span></span>|<span data-ttu-id="49e59-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-173">String</span></span>|<span data-ttu-id="49e59-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-174">The owner of the app.</span></span> <span data-ttu-id="49e59-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-176">developer</span><span class="sxs-lookup"><span data-stu-id="49e59-176">developer</span></span>|<span data-ttu-id="49e59-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-177">String</span></span>|<span data-ttu-id="49e59-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-178">The developer of the app.</span></span> <span data-ttu-id="49e59-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-180">notes</span><span class="sxs-lookup"><span data-stu-id="49e59-180">notes</span></span>|<span data-ttu-id="49e59-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-181">String</span></span>|<span data-ttu-id="49e59-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="49e59-182">Notes for the app.</span></span> <span data-ttu-id="49e59-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="49e59-184">uploadState</span></span>|<span data-ttu-id="49e59-185">Int32</span><span class="sxs-lookup"><span data-stu-id="49e59-185">Int32</span></span>|<span data-ttu-id="49e59-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="49e59-186">The upload state.</span></span> <span data-ttu-id="49e59-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="49e59-188">publishingState</span></span>|[<span data-ttu-id="49e59-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="49e59-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="49e59-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="49e59-190">The publishing state for the app.</span></span> <span data-ttu-id="49e59-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="49e59-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="49e59-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="49e59-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="49e59-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="49e59-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="49e59-194">isAssigned</span></span>|<span data-ttu-id="49e59-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e59-195">Boolean</span></span>|<span data-ttu-id="49e59-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="49e59-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="49e59-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49e59-198">roleScopeTagIds</span></span>|<span data-ttu-id="49e59-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="49e59-199">String collection</span></span>|<span data-ttu-id="49e59-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="49e59-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="49e59-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="49e59-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="49e59-202">committedContentVersion</span></span>|<span data-ttu-id="49e59-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-203">String</span></span>|<span data-ttu-id="49e59-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="49e59-204">The internal committed content version.</span></span> <span data-ttu-id="49e59-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="49e59-206">fileName</span><span class="sxs-lookup"><span data-stu-id="49e59-206">fileName</span></span>|<span data-ttu-id="49e59-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-207">String</span></span>|<span data-ttu-id="49e59-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="49e59-208">The name of the main Lob application file.</span></span> <span data-ttu-id="49e59-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="49e59-210">size</span><span class="sxs-lookup"><span data-stu-id="49e59-210">size</span></span>|<span data-ttu-id="49e59-211">Int64</span><span class="sxs-lookup"><span data-stu-id="49e59-211">Int64</span></span>|<span data-ttu-id="49e59-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="49e59-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="49e59-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="49e59-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="49e59-214">commandLine</span><span class="sxs-lookup"><span data-stu-id="49e59-214">commandLine</span></span>|<span data-ttu-id="49e59-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-215">String</span></span>|<span data-ttu-id="49e59-216">Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="49e59-216">The command line.</span></span>|
|<span data-ttu-id="49e59-217">productCode</span><span class="sxs-lookup"><span data-stu-id="49e59-217">productCode</span></span>|<span data-ttu-id="49e59-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-218">String</span></span>|<span data-ttu-id="49e59-219">Produktcode</span><span class="sxs-lookup"><span data-stu-id="49e59-219">The product code.</span></span>|
|<span data-ttu-id="49e59-220">productVersion</span><span class="sxs-lookup"><span data-stu-id="49e59-220">productVersion</span></span>|<span data-ttu-id="49e59-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-221">String</span></span>|<span data-ttu-id="49e59-222">Produktversion der branchenspezifischen Windows Mobile-MSI-App.</span><span class="sxs-lookup"><span data-stu-id="49e59-222">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="49e59-223">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="49e59-223">ignoreVersionDetection</span></span>|<span data-ttu-id="49e59-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e59-224">Boolean</span></span>|<span data-ttu-id="49e59-225">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="49e59-225">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="49e59-226">Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="49e59-226">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="49e59-227">identityVersion</span><span class="sxs-lookup"><span data-stu-id="49e59-227">identityVersion</span></span>|<span data-ttu-id="49e59-228">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49e59-228">String</span></span>|<span data-ttu-id="49e59-229">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="49e59-229">The identity version.</span></span>|
|<span data-ttu-id="49e59-230">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="49e59-230">useDeviceContext</span></span>|<span data-ttu-id="49e59-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="49e59-231">Boolean</span></span>|<span data-ttu-id="49e59-232">Gibt an, ob ein Dualmodus-MSI-Datei im Gerätekontext installiert.</span><span class="sxs-lookup"><span data-stu-id="49e59-232">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="49e59-233">Bei true wird die app für alle Benutzer installiert werden.</span><span class="sxs-lookup"><span data-stu-id="49e59-233">If true, app will be installed for all users.</span></span> <span data-ttu-id="49e59-234">Bei false werden app pro Benutzer installiert.</span><span class="sxs-lookup"><span data-stu-id="49e59-234">If false, app will be installed per-user.</span></span> <span data-ttu-id="49e59-235">Wenn null, wird Service die MSI-Paket Standard-Install-Kontext verwenden.</span><span class="sxs-lookup"><span data-stu-id="49e59-235">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="49e59-236">Im Fall eines WAN-Dualmodus-MSI werden diese Standardeinstellung pro Benutzer.</span><span class="sxs-lookup"><span data-stu-id="49e59-236">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="49e59-237">Kann nicht für apps Dual-Modus festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="49e59-237">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="49e59-238">Kann nach der ursprünglichen Erstellung der Anwendung geändert werden.</span><span class="sxs-lookup"><span data-stu-id="49e59-238">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="49e59-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="49e59-239">Response</span></span>
<span data-ttu-id="49e59-240">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49e59-240">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49e59-241">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49e59-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="49e59-242">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49e59-242">Request</span></span>
<span data-ttu-id="49e59-243">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49e59-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="49e59-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="49e59-244">Response</span></span>
<span data-ttu-id="49e59-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49e59-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




