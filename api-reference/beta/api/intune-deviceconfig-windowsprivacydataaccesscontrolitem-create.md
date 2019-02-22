---
title: WindowsPrivacyDataAccessControlItem erstellen
description: Erstellen eines neuen windowsPrivacyDataAccessControlItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efe12eba472c86dec225b74d7390b669de9928f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144611"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="3ef50-103">WindowsPrivacyDataAccessControlItem erstellen</span><span class="sxs-lookup"><span data-stu-id="3ef50-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="3ef50-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ef50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ef50-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3ef50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ef50-106">Erstellen eines neuen [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ef50-106">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ef50-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ef50-107">Prerequisites</span></span>
<span data-ttu-id="3ef50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ef50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3ef50-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ef50-110">Permission type</span></span>|<span data-ttu-id="3ef50-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ef50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ef50-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ef50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ef50-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ef50-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ef50-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ef50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ef50-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ef50-115">Not supported.</span></span>|
|<span data-ttu-id="3ef50-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ef50-116">Application</span></span>|<span data-ttu-id="3ef50-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ef50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ef50-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ef50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="3ef50-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ef50-119">Request headers</span></span>
|<span data-ttu-id="3ef50-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3ef50-120">Header</span></span>|<span data-ttu-id="3ef50-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3ef50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ef50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ef50-122">Authorization</span></span>|<span data-ttu-id="3ef50-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ef50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ef50-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3ef50-124">Accept</span></span>|<span data-ttu-id="3ef50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ef50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ef50-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ef50-126">Request body</span></span>
<span data-ttu-id="3ef50-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsPrivacyDataAccessControlItem-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="3ef50-127">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="3ef50-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPrivacyDataAccessControlItem erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3ef50-128">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="3ef50-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ef50-129">Property</span></span>|<span data-ttu-id="3ef50-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3ef50-130">Type</span></span>|<span data-ttu-id="3ef50-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ef50-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef50-132">id</span><span class="sxs-lookup"><span data-stu-id="3ef50-132">id</span></span>|<span data-ttu-id="3ef50-133">string</span><span class="sxs-lookup"><span data-stu-id="3ef50-133">String</span></span>|<span data-ttu-id="3ef50-134">Der Schlüssel von WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="3ef50-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="3ef50-135">Access Level</span><span class="sxs-lookup"><span data-stu-id="3ef50-135">accessLevel</span></span>|[<span data-ttu-id="3ef50-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="3ef50-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="3ef50-137">Dies gibt eine Zugriffsebene für die Datenschutzkategorie an, der die angegebene Anwendung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="3ef50-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="3ef50-138">Mögliche Werte: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="3ef50-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="3ef50-139">dataCategory</span><span class="sxs-lookup"><span data-stu-id="3ef50-139">dataCategory</span></span>|[<span data-ttu-id="3ef50-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="3ef50-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="3ef50-141">Dies gibt eine Datenschutzkategorie an, auf die die spezifische Zugriffssteuerung angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3ef50-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="3ef50-142">Mögliche Werte sind: `notConfigured`, `accountInfo`, `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `email` `location` `messaging` `microphone` `motion` `notifications` `phone`,,,,,,,, `radios`,, `trustedDevices` ,,,,,, `tasks` `syncWithDevices` `diagnosticsInfo` .</span><span class="sxs-lookup"><span data-stu-id="3ef50-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="3ef50-143">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="3ef50-143">appPackageFamilyName</span></span>|<span data-ttu-id="3ef50-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ef50-144">String</span></span>|<span data-ttu-id="3ef50-145">Der Name der Paketfamilie einer Windows-app.</span><span class="sxs-lookup"><span data-stu-id="3ef50-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="3ef50-146">Wenn diese Einstellung festgelegt ist, gilt die Zugriffsebene für die angegebene Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3ef50-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="3ef50-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3ef50-147">appDisplayName</span></span>|<span data-ttu-id="3ef50-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ef50-148">String</span></span>|<span data-ttu-id="3ef50-149">Der Name der Paketfamilie einer Windows-app.</span><span class="sxs-lookup"><span data-stu-id="3ef50-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="3ef50-150">Wenn diese Einstellung festgelegt ist, gilt die Zugriffsebene für die angegebene Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3ef50-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="3ef50-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ef50-151">Response</span></span>
<span data-ttu-id="3ef50-152">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3ef50-152">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ef50-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ef50-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ef50-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ef50-154">Request</span></span>
<span data-ttu-id="3ef50-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ef50-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="3ef50-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ef50-156">Response</span></span>
<span data-ttu-id="3ef50-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ef50-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```




