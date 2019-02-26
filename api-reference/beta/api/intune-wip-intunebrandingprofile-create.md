---
title: IntuneBrandingProfile erstellen
description: Erstellen eines neuen intuneBrandingProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4786920476794d370a33d8275c347c909cf538
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142056"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="01b5e-103">IntuneBrandingProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="01b5e-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="01b5e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01b5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01b5e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="01b5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01b5e-106">Erstellen eines neuen [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="01b5e-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01b5e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="01b5e-107">Prerequisites</span></span>
<span data-ttu-id="01b5e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="01b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="01b5e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01b5e-110">Permission type</span></span>|<span data-ttu-id="01b5e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01b5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01b5e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01b5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01b5e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01b5e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01b5e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01b5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01b5e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01b5e-115">Not supported.</span></span>|
|<span data-ttu-id="01b5e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01b5e-116">Application</span></span>|<span data-ttu-id="01b5e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01b5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01b5e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01b5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="01b5e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01b5e-119">Request headers</span></span>
|<span data-ttu-id="01b5e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="01b5e-120">Header</span></span>|<span data-ttu-id="01b5e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="01b5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01b5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01b5e-122">Authorization</span></span>|<span data-ttu-id="01b5e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="01b5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01b5e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="01b5e-124">Accept</span></span>|<span data-ttu-id="01b5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01b5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01b5e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01b5e-126">Request body</span></span>
<span data-ttu-id="01b5e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das intuneBrandingProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="01b5e-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="01b5e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der intuneBrandingProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="01b5e-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="01b5e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01b5e-129">Property</span></span>|<span data-ttu-id="01b5e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="01b5e-130">Type</span></span>|<span data-ttu-id="01b5e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01b5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01b5e-132">id</span><span class="sxs-lookup"><span data-stu-id="01b5e-132">id</span></span>|<span data-ttu-id="01b5e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-133">String</span></span>|<span data-ttu-id="01b5e-134">Profilschlüssel</span><span class="sxs-lookup"><span data-stu-id="01b5e-134">Profile Key</span></span>|
|<span data-ttu-id="01b5e-135">Profilname</span><span class="sxs-lookup"><span data-stu-id="01b5e-135">profileName</span></span>|<span data-ttu-id="01b5e-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-136">String</span></span>|<span data-ttu-id="01b5e-137">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="01b5e-137">Name of the profile</span></span>|
|<span data-ttu-id="01b5e-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="01b5e-138">profileDescription</span></span>|<span data-ttu-id="01b5e-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-139">String</span></span>|<span data-ttu-id="01b5e-140">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="01b5e-140">Description of the profile</span></span>|
|<span data-ttu-id="01b5e-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="01b5e-141">isDefaultProfile</span></span>|<span data-ttu-id="01b5e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="01b5e-142">Boolean</span></span>|<span data-ttu-id="01b5e-143">Zeigt an, ob das Profil standardmäßig verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="01b5e-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="01b5e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01b5e-144">createdDateTime</span></span>|<span data-ttu-id="01b5e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01b5e-145">DateTimeOffset</span></span>|<span data-ttu-id="01b5e-146">Bei der Erstellung des BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="01b5e-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="01b5e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01b5e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="01b5e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01b5e-148">DateTimeOffset</span></span>|<span data-ttu-id="01b5e-149">Wenn die BrandingProfile zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="01b5e-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="01b5e-150">displayName</span><span class="sxs-lookup"><span data-stu-id="01b5e-150">displayName</span></span>|<span data-ttu-id="01b5e-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-151">String</span></span>|<span data-ttu-id="01b5e-152">Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="01b5e-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="01b5e-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="01b5e-153">contactITName</span></span>|<span data-ttu-id="01b5e-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-154">String</span></span>|<span data-ttu-id="01b5e-155">Name der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="01b5e-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="01b5e-156">contactITPhoneNumber</span></span>|<span data-ttu-id="01b5e-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-157">String</span></span>|<span data-ttu-id="01b5e-158">Telefonnummer der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="01b5e-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="01b5e-159">contactITEmailAddress</span></span>|<span data-ttu-id="01b5e-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-160">String</span></span>|<span data-ttu-id="01b5e-161">E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="01b5e-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="01b5e-162">contactITNotes</span></span>|<span data-ttu-id="01b5e-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-163">String</span></span>|<span data-ttu-id="01b5e-164">Textkommentare zu der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="01b5e-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="01b5e-165">privacyUrl</span></span>|<span data-ttu-id="01b5e-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-166">String</span></span>|<span data-ttu-id="01b5e-167">URL zur Datenschutzrichtlinie des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="01b5e-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="01b5e-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="01b5e-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b5e-169">String</span></span>|<span data-ttu-id="01b5e-170">URL zur IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="01b5e-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="01b5e-171">onlineSupportSiteName</span></span>|<span data-ttu-id="01b5e-172">String</span><span class="sxs-lookup"><span data-stu-id="01b5e-172">String</span></span>|<span data-ttu-id="01b5e-173">Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="01b5e-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="01b5e-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="01b5e-174">themeColor</span></span>|[<span data-ttu-id="01b5e-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="01b5e-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="01b5e-176">Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal</span><span class="sxs-lookup"><span data-stu-id="01b5e-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="01b5e-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="01b5e-177">showLogo</span></span>|<span data-ttu-id="01b5e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="01b5e-178">Boolean</span></span>|<span data-ttu-id="01b5e-179">Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen</span><span class="sxs-lookup"><span data-stu-id="01b5e-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="01b5e-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="01b5e-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="01b5e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="01b5e-181">Boolean</span></span>|<span data-ttu-id="01b5e-182">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="01b5e-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="01b5e-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="01b5e-183">themeColorLogo</span></span>|[<span data-ttu-id="01b5e-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="01b5e-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="01b5e-185">Logobild, das in Unternehmens Portal-apps auf Design Farbhintergründen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="01b5e-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="01b5e-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="01b5e-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="01b5e-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="01b5e-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="01b5e-188">Logobild, das in Unternehmens Portal-apps auf hellen Hintergründen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="01b5e-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="01b5e-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="01b5e-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="01b5e-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="01b5e-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="01b5e-191">Angepasstes Bild, das auf der Startseite der Unternehmens Portal-apps angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="01b5e-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="01b5e-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="01b5e-192">Response</span></span>
<span data-ttu-id="01b5e-193">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="01b5e-193">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01b5e-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01b5e-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="01b5e-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01b5e-195">Request</span></span>
<span data-ttu-id="01b5e-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01b5e-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1205

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="01b5e-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="01b5e-197">Response</span></span>
<span data-ttu-id="01b5e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01b5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




