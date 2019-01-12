---
title: Erstellen von windowsAssignedAccessProfile
description: Erstellen eines neuen WindowsAssignedAccessProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2313dff2c2f387e0a981775e0b6cc6e53a988f3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956346"
---
# <a name="create-windowsassignedaccessprofile"></a><span data-ttu-id="22d27-103">Erstellen von windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="22d27-103">Create windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="22d27-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="22d27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22d27-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22d27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22d27-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22d27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22d27-107">Erstellen eines neuen [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="22d27-107">Create a new [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22d27-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22d27-108">Prerequisites</span></span>
<span data-ttu-id="22d27-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d27-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22d27-111">Permission type</span></span>|<span data-ttu-id="22d27-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22d27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d27-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22d27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22d27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22d27-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22d27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d27-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22d27-116">Not supported.</span></span>|
|<span data-ttu-id="22d27-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22d27-117">Application</span></span>|<span data-ttu-id="22d27-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22d27-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d27-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22d27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="22d27-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22d27-120">Request headers</span></span>
|<span data-ttu-id="22d27-121">Header</span><span class="sxs-lookup"><span data-stu-id="22d27-121">Header</span></span>|<span data-ttu-id="22d27-122">Wert</span><span class="sxs-lookup"><span data-stu-id="22d27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22d27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d27-123">Authorization</span></span>|<span data-ttu-id="22d27-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22d27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22d27-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="22d27-125">Accept</span></span>|<span data-ttu-id="22d27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22d27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d27-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22d27-127">Request body</span></span>
<span data-ttu-id="22d27-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsAssignedAccessProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="22d27-128">In the request body, supply a JSON representation for the windowsAssignedAccessProfile object.</span></span>

<span data-ttu-id="22d27-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsAssignedAccessProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="22d27-129">The following table shows the properties that are required when you create the windowsAssignedAccessProfile.</span></span>

|<span data-ttu-id="22d27-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22d27-130">Property</span></span>|<span data-ttu-id="22d27-131">Typ</span><span class="sxs-lookup"><span data-stu-id="22d27-131">Type</span></span>|<span data-ttu-id="22d27-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22d27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d27-133">id</span><span class="sxs-lookup"><span data-stu-id="22d27-133">id</span></span>|<span data-ttu-id="22d27-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22d27-134">String</span></span>|<span data-ttu-id="22d27-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="22d27-135">Key of the entity.</span></span>|
|<span data-ttu-id="22d27-136">Profilname</span><span class="sxs-lookup"><span data-stu-id="22d27-136">profileName</span></span>|<span data-ttu-id="22d27-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22d27-137">String</span></span>|<span data-ttu-id="22d27-138">Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="22d27-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="22d27-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="22d27-139">showTaskBar</span></span>|<span data-ttu-id="22d27-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="22d27-140">Boolean</span></span>|<span data-ttu-id="22d27-141">Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="22d27-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="22d27-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="22d27-142">appUserModelIds</span></span>|<span data-ttu-id="22d27-143">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="22d27-143">String collection</span></span>|<span data-ttu-id="22d27-144">Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="22d27-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="22d27-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="22d27-145">desktopAppPaths</span></span>|<span data-ttu-id="22d27-146">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="22d27-146">String collection</span></span>|<span data-ttu-id="22d27-147">Dies sind die Pfade der Desktop-Apps, die auf das Startmenü zur Verfügung stehen, und die einzige apps des Benutzers kann zu starten.</span><span class="sxs-lookup"><span data-stu-id="22d27-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="22d27-148">userAccounts</span><span class="sxs-lookup"><span data-stu-id="22d27-148">userAccounts</span></span>|<span data-ttu-id="22d27-149">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="22d27-149">String collection</span></span>|<span data-ttu-id="22d27-150">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden.</span><span class="sxs-lookup"><span data-stu-id="22d27-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="22d27-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="22d27-151">startMenuLayoutXml</span></span>|<span data-ttu-id="22d27-152">Binär</span><span class="sxs-lookup"><span data-stu-id="22d27-152">Binary</span></span>|<span data-ttu-id="22d27-153">Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.</span><span class="sxs-lookup"><span data-stu-id="22d27-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="22d27-154">Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert.</span><span class="sxs-lookup"><span data-stu-id="22d27-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="22d27-155">XML muss im Binärformat sein.</span><span class="sxs-lookup"><span data-stu-id="22d27-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="22d27-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="22d27-156">Response</span></span>
<span data-ttu-id="22d27-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="22d27-157">If successful, this method returns a `201 Created` response code and a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d27-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22d27-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="22d27-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22d27-159">Request</span></span>
<span data-ttu-id="22d27-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22d27-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
Content-type: application/json
Content-length: 364

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a><span data-ttu-id="22d27-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="22d27-161">Response</span></span>
<span data-ttu-id="22d27-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22d27-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





