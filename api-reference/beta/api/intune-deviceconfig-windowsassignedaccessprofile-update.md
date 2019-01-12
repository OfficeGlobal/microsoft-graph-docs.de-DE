---
title: WindowsAssignedAccessProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAssignedAccessProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f82a1ad5a5bdea639ec3dc24f40a3c66c4a0fe1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940379"
---
# <a name="update-windowsassignedaccessprofile"></a><span data-ttu-id="5a5b4-103">WindowsAssignedAccessProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5a5b4-103">Update windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="5a5b4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a5b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a5b4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a5b4-107">Aktualisieren Sie die Eigenschaften eines [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-107">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a5b4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a5b4-108">Prerequisites</span></span>
<span data-ttu-id="5a5b4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a5b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a5b4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a5b4-111">Permission type</span></span>|<span data-ttu-id="5a5b4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a5b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a5b4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a5b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a5b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a5b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a5b4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a5b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a5b4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a5b4-116">Not supported.</span></span>|
|<span data-ttu-id="5a5b4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a5b4-117">Application</span></span>|<span data-ttu-id="5a5b4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a5b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a5b4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a5b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="5a5b4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a5b4-120">Request headers</span></span>
|<span data-ttu-id="5a5b4-121">Header</span><span class="sxs-lookup"><span data-stu-id="5a5b4-121">Header</span></span>|<span data-ttu-id="5a5b4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5a5b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a5b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a5b4-123">Authorization</span></span>|<span data-ttu-id="5a5b4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a5b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a5b4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a5b4-125">Accept</span></span>|<span data-ttu-id="5a5b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a5b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a5b4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a5b4-127">Request body</span></span>
<span data-ttu-id="5a5b4-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-128">In the request body, supply a JSON representation for the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>

<span data-ttu-id="5a5b4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-129">The following table shows the properties that are required when you create the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>

|<span data-ttu-id="5a5b4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a5b4-130">Property</span></span>|<span data-ttu-id="5a5b4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5a5b4-131">Type</span></span>|<span data-ttu-id="5a5b4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a5b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a5b4-133">id</span><span class="sxs-lookup"><span data-stu-id="5a5b4-133">id</span></span>|<span data-ttu-id="5a5b4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a5b4-134">String</span></span>|<span data-ttu-id="5a5b4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5a5b4-135">Key of the entity.</span></span>|
|<span data-ttu-id="5a5b4-136">Profilname</span><span class="sxs-lookup"><span data-stu-id="5a5b4-136">profileName</span></span>|<span data-ttu-id="5a5b4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a5b4-137">String</span></span>|<span data-ttu-id="5a5b4-138">Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="5a5b4-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="5a5b4-139">showTaskBar</span></span>|<span data-ttu-id="5a5b4-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5a5b4-140">Boolean</span></span>|<span data-ttu-id="5a5b4-141">Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="5a5b4-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="5a5b4-142">appUserModelIds</span></span>|<span data-ttu-id="5a5b4-143">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="5a5b4-143">String collection</span></span>|<span data-ttu-id="5a5b4-144">Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="5a5b4-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="5a5b4-145">desktopAppPaths</span></span>|<span data-ttu-id="5a5b4-146">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="5a5b4-146">String collection</span></span>|<span data-ttu-id="5a5b4-147">Dies sind die Pfade der Desktop-Apps, die auf das Startmenü zur Verfügung stehen, und die einzige apps des Benutzers kann zu starten.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="5a5b4-148">userAccounts</span><span class="sxs-lookup"><span data-stu-id="5a5b4-148">userAccounts</span></span>|<span data-ttu-id="5a5b4-149">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="5a5b4-149">String collection</span></span>|<span data-ttu-id="5a5b4-150">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="5a5b4-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="5a5b4-151">startMenuLayoutXml</span></span>|<span data-ttu-id="5a5b4-152">Binär</span><span class="sxs-lookup"><span data-stu-id="5a5b4-152">Binary</span></span>|<span data-ttu-id="5a5b4-153">Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="5a5b4-154">Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="5a5b4-155">XML muss im Binärformat sein.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="5a5b4-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a5b4-156">Response</span></span>
<span data-ttu-id="5a5b4-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-157">If successful, this method returns a `200 OK` response code and an updated [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a5b4-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a5b4-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a5b4-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a5b4-159">Request</span></span>
<span data-ttu-id="5a5b4-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
Content-type: application/json
Content-length: 297

{
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

### <a name="response"></a><span data-ttu-id="5a5b4-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a5b4-161">Response</span></span>
<span data-ttu-id="5a5b4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a5b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





