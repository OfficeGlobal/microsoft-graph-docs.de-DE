---
title: Erstellen von windowsPrivacyDataAccessControlItem
description: Erstellen eines neuen WindowsPrivacyDataAccessControlItem-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e7b78a113134b4d268df3c759dfd7dc700759a35
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405583"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="7b8b3-103">Erstellen von windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="7b8b3-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="7b8b3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b8b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b8b3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b8b3-107">Erstellen eines neuen [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b8b3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b8b3-108">Prerequisites</span></span>
<span data-ttu-id="7b8b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b8b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b8b3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b8b3-111">Permission type</span></span>|<span data-ttu-id="7b8b3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b8b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b8b3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b8b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b8b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b8b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b8b3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b8b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b8b3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b8b3-116">Not supported.</span></span>|
|<span data-ttu-id="7b8b3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b8b3-117">Application</span></span>|<span data-ttu-id="7b8b3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b8b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b8b3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b8b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="7b8b3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b8b3-120">Request headers</span></span>
|<span data-ttu-id="7b8b3-121">Header</span><span class="sxs-lookup"><span data-stu-id="7b8b3-121">Header</span></span>|<span data-ttu-id="7b8b3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7b8b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b8b3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7b8b3-123">Authorization</span></span>|<span data-ttu-id="7b8b3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b8b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b8b3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b8b3-125">Accept</span></span>|<span data-ttu-id="7b8b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b8b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b8b3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b8b3-127">Request body</span></span>
<span data-ttu-id="7b8b3-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsPrivacyDataAccessControlItem eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="7b8b3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsPrivacyDataAccessControlItem erstellen.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="7b8b3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b8b3-130">Property</span></span>|<span data-ttu-id="7b8b3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7b8b3-131">Type</span></span>|<span data-ttu-id="7b8b3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b8b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b8b3-133">id</span><span class="sxs-lookup"><span data-stu-id="7b8b3-133">id</span></span>|<span data-ttu-id="7b8b3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b8b3-134">String</span></span>|<span data-ttu-id="7b8b3-135">Der Schlüssel des WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="7b8b3-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="7b8b3-136">accessLevel</span></span>|[<span data-ttu-id="7b8b3-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="7b8b3-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="7b8b3-138">Dies bedeutet eine Zugriffsebene für die Kategorie private Daten an die für die angegebene Anwendung erhalten soll.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="7b8b3-139">Mögliche Werte: sind `notConfigured`, `forceAllow`, `forceDeny` und `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="7b8b3-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="7b8b3-140">dataCategory</span></span>|[<span data-ttu-id="7b8b3-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="7b8b3-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="7b8b3-142">Dies bedeutet eine private Datenkategorie für die bestimmten Access Control gelten soll.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="7b8b3-143">Mögliche Werte sind: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="7b8b3-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="7b8b3-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="7b8b3-144">appPackageFamilyName</span></span>|<span data-ttu-id="7b8b3-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b8b3-145">String</span></span>|<span data-ttu-id="7b8b3-146">Die Paket-Produktfamilie Name einer Windows-App.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="7b8b3-147">Wenn festgelegt, gilt die Zugriffsebene für die angegebene Anwendung.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="7b8b3-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b8b3-148">appDisplayName</span></span>|<span data-ttu-id="7b8b3-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b8b3-149">String</span></span>|<span data-ttu-id="7b8b3-150">Die Paket-Produktfamilie Name einer Windows-App.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="7b8b3-151">Wenn festgelegt, gilt die Zugriffsebene für die angegebene Anwendung.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="7b8b3-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b8b3-152">Response</span></span>
<span data-ttu-id="7b8b3-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b8b3-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b8b3-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b8b3-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b8b3-155">Request</span></span>
<span data-ttu-id="7b8b3-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b8b3-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b8b3-157">Response</span></span>
<span data-ttu-id="7b8b3-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b8b3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




