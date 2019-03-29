---
title: IntuneBrandingProfile aktualisieren
description: Aktualisieren der Eigenschaften eines intuneBrandingProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8a805e8878dbd41493c550647ed9e038c320b13
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976659"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="37bd4-103">IntuneBrandingProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="37bd4-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="37bd4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37bd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37bd4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="37bd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37bd4-106">Aktualisieren der Eigenschaften eines [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37bd4-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37bd4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37bd4-107">Prerequisites</span></span>
<span data-ttu-id="37bd4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37bd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37bd4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37bd4-110">Permission type</span></span>|<span data-ttu-id="37bd4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37bd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37bd4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37bd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37bd4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37bd4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37bd4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37bd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37bd4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37bd4-115">Not supported.</span></span>|
|<span data-ttu-id="37bd4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37bd4-116">Application</span></span>|<span data-ttu-id="37bd4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37bd4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37bd4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37bd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="37bd4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37bd4-119">Request headers</span></span>
|<span data-ttu-id="37bd4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="37bd4-120">Header</span></span>|<span data-ttu-id="37bd4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="37bd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37bd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37bd4-122">Authorization</span></span>|<span data-ttu-id="37bd4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37bd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37bd4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="37bd4-124">Accept</span></span>|<span data-ttu-id="37bd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37bd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37bd4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37bd4-126">Request body</span></span>
<span data-ttu-id="37bd4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="37bd4-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="37bd4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="37bd4-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="37bd4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37bd4-129">Property</span></span>|<span data-ttu-id="37bd4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="37bd4-130">Type</span></span>|<span data-ttu-id="37bd4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37bd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37bd4-132">id</span><span class="sxs-lookup"><span data-stu-id="37bd4-132">id</span></span>|<span data-ttu-id="37bd4-133">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-133">String</span></span>|<span data-ttu-id="37bd4-134">Profilschlüssel</span><span class="sxs-lookup"><span data-stu-id="37bd4-134">Profile Key</span></span>|
|<span data-ttu-id="37bd4-135">Profilname</span><span class="sxs-lookup"><span data-stu-id="37bd4-135">profileName</span></span>|<span data-ttu-id="37bd4-136">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-136">String</span></span>|<span data-ttu-id="37bd4-137">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="37bd4-137">Name of the profile</span></span>|
|<span data-ttu-id="37bd4-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="37bd4-138">profileDescription</span></span>|<span data-ttu-id="37bd4-139">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-139">String</span></span>|<span data-ttu-id="37bd4-140">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="37bd4-140">Description of the profile</span></span>|
|<span data-ttu-id="37bd4-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="37bd4-141">isDefaultProfile</span></span>|<span data-ttu-id="37bd4-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="37bd4-142">Boolean</span></span>|<span data-ttu-id="37bd4-143">Zeigt an, ob das Profil standardmäßig verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="37bd4-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="37bd4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37bd4-144">createdDateTime</span></span>|<span data-ttu-id="37bd4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37bd4-145">DateTimeOffset</span></span>|<span data-ttu-id="37bd4-146">Bei der Erstellung des BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="37bd4-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="37bd4-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37bd4-147">lastModifiedDateTime</span></span>|<span data-ttu-id="37bd4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37bd4-148">DateTimeOffset</span></span>|<span data-ttu-id="37bd4-149">Wenn die BrandingProfile zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="37bd4-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="37bd4-150">displayName</span><span class="sxs-lookup"><span data-stu-id="37bd4-150">displayName</span></span>|<span data-ttu-id="37bd4-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37bd4-151">String</span></span>|<span data-ttu-id="37bd4-152">Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="37bd4-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="37bd4-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="37bd4-153">contactITName</span></span>|<span data-ttu-id="37bd4-154">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-154">String</span></span>|<span data-ttu-id="37bd4-155">Name der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="37bd4-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="37bd4-156">contactITPhoneNumber</span></span>|<span data-ttu-id="37bd4-157">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-157">String</span></span>|<span data-ttu-id="37bd4-158">Telefonnummer der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="37bd4-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="37bd4-159">contactITEmailAddress</span></span>|<span data-ttu-id="37bd4-160">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-160">String</span></span>|<span data-ttu-id="37bd4-161">E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="37bd4-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="37bd4-162">contactITNotes</span></span>|<span data-ttu-id="37bd4-163">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-163">String</span></span>|<span data-ttu-id="37bd4-164">Textkommentare zu der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="37bd4-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="37bd4-165">privacyUrl</span></span>|<span data-ttu-id="37bd4-166">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-166">String</span></span>|<span data-ttu-id="37bd4-167">URL zur Datenschutzrichtlinie des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="37bd4-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="37bd4-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="37bd4-169">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-169">String</span></span>|<span data-ttu-id="37bd4-170">URL zur IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="37bd4-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="37bd4-171">onlineSupportSiteName</span></span>|<span data-ttu-id="37bd4-172">String</span><span class="sxs-lookup"><span data-stu-id="37bd4-172">String</span></span>|<span data-ttu-id="37bd4-173">Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="37bd4-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="37bd4-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="37bd4-174">themeColor</span></span>|[<span data-ttu-id="37bd4-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="37bd4-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="37bd4-176">Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal</span><span class="sxs-lookup"><span data-stu-id="37bd4-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="37bd4-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="37bd4-177">showLogo</span></span>|<span data-ttu-id="37bd4-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="37bd4-178">Boolean</span></span>|<span data-ttu-id="37bd4-179">Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen</span><span class="sxs-lookup"><span data-stu-id="37bd4-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="37bd4-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="37bd4-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="37bd4-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="37bd4-181">Boolean</span></span>|<span data-ttu-id="37bd4-182">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="37bd4-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="37bd4-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="37bd4-183">themeColorLogo</span></span>|[<span data-ttu-id="37bd4-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="37bd4-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="37bd4-185">Logobild, das in Unternehmens Portal-apps auf Design Farbhintergründen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="37bd4-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="37bd4-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="37bd4-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="37bd4-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="37bd4-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="37bd4-188">Logobild, das in Unternehmens Portal-apps auf hellen Hintergründen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="37bd4-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="37bd4-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="37bd4-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="37bd4-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="37bd4-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="37bd4-191">Angepasstes Bild, das auf der Startseite der Unternehmens Portal-apps angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="37bd4-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="37bd4-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="37bd4-192">Response</span></span>
<span data-ttu-id="37bd4-193">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="37bd4-193">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37bd4-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37bd4-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="37bd4-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37bd4-195">Request</span></span>
<span data-ttu-id="37bd4-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37bd4-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
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

### <a name="response"></a><span data-ttu-id="37bd4-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="37bd4-197">Response</span></span>
<span data-ttu-id="37bd4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37bd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




