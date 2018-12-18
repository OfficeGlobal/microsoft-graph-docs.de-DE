---
title: WindowsPrivacyDataAccessControlItem aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsPrivacyDataAccessControlItem-Objekts.
author: tfitzmac
ms.openlocfilehash: 38389049c03d822feb4c3791dfee65e327e1afea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324157"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="bce2d-103">WindowsPrivacyDataAccessControlItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bce2d-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="bce2d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bce2d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bce2d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bce2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bce2d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bce2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bce2d-107">Aktualisieren Sie die Eigenschaften eines [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bce2d-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bce2d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bce2d-108">Prerequisites</span></span>
<span data-ttu-id="bce2d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bce2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bce2d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bce2d-111">Permission type</span></span>|<span data-ttu-id="bce2d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bce2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bce2d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bce2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bce2d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bce2d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bce2d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bce2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bce2d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bce2d-116">Not supported.</span></span>|
|<span data-ttu-id="bce2d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bce2d-117">Application</span></span>|<span data-ttu-id="bce2d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bce2d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bce2d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bce2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="bce2d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bce2d-120">Request headers</span></span>
|<span data-ttu-id="bce2d-121">Header</span><span class="sxs-lookup"><span data-stu-id="bce2d-121">Header</span></span>|<span data-ttu-id="bce2d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bce2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bce2d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bce2d-123">Authorization</span></span>|<span data-ttu-id="bce2d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bce2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bce2d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bce2d-125">Accept</span></span>|<span data-ttu-id="bce2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bce2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bce2d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bce2d-127">Request body</span></span>
<span data-ttu-id="bce2d-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="bce2d-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="bce2d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="bce2d-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="bce2d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bce2d-130">Property</span></span>|<span data-ttu-id="bce2d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bce2d-131">Type</span></span>|<span data-ttu-id="bce2d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bce2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bce2d-133">id</span><span class="sxs-lookup"><span data-stu-id="bce2d-133">id</span></span>|<span data-ttu-id="bce2d-134">String</span><span class="sxs-lookup"><span data-stu-id="bce2d-134">String</span></span>|<span data-ttu-id="bce2d-135">Der Schlüssel des WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="bce2d-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="bce2d-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="bce2d-136">accessLevel</span></span>|[<span data-ttu-id="bce2d-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="bce2d-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="bce2d-138">Dies bedeutet eine Zugriffsebene für die Kategorie private Daten an die für die angegebene Anwendung erhalten soll.</span><span class="sxs-lookup"><span data-stu-id="bce2d-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="bce2d-139">Mögliche Werte: sind `notConfigured`, `forceAllow`, `forceDeny` und `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="bce2d-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="bce2d-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="bce2d-140">dataCategory</span></span>|[<span data-ttu-id="bce2d-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="bce2d-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="bce2d-142">Dies bedeutet eine private Datenkategorie für die bestimmten Access Control gelten soll.</span><span class="sxs-lookup"><span data-stu-id="bce2d-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="bce2d-143">Mögliche Werte sind: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="bce2d-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="bce2d-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="bce2d-144">appPackageFamilyName</span></span>|<span data-ttu-id="bce2d-145">String</span><span class="sxs-lookup"><span data-stu-id="bce2d-145">String</span></span>|<span data-ttu-id="bce2d-146">Die Paket-Produktfamilie Name einer Windows-App.</span><span class="sxs-lookup"><span data-stu-id="bce2d-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="bce2d-147">Wenn festgelegt, gilt die Zugriffsebene für die angegebene Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bce2d-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="bce2d-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="bce2d-148">appDisplayName</span></span>|<span data-ttu-id="bce2d-149">String</span><span class="sxs-lookup"><span data-stu-id="bce2d-149">String</span></span>|<span data-ttu-id="bce2d-150">Die Paket-Produktfamilie Name einer Windows-App.</span><span class="sxs-lookup"><span data-stu-id="bce2d-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="bce2d-151">Wenn festgelegt, gilt die Zugriffsebene für die angegebene Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bce2d-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="bce2d-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="bce2d-152">Response</span></span>
<span data-ttu-id="bce2d-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bce2d-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bce2d-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bce2d-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="bce2d-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bce2d-155">Request</span></span>
<span data-ttu-id="bce2d-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bce2d-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
Content-type: application/json
Content-length: 176

{
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="bce2d-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="bce2d-157">Response</span></span>
<span data-ttu-id="bce2d-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bce2d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





