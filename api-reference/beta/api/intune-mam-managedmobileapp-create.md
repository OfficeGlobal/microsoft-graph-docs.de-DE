---
title: Erstellen von „managedMobileApp“
description: Diese Methode erstellt ein neues Objekt des Typs managedMobileApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 546110d3e25c7b5b683f9104997fdbc497e78f9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404701"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="24f6c-103">Erstellen von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="24f6c-103">Create managedMobileApp</span></span>

> <span data-ttu-id="24f6c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="24f6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24f6c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24f6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24f6c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24f6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24f6c-107">Diese Methode erstellt ein neues Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24f6c-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24f6c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24f6c-108">Prerequisites</span></span>
<span data-ttu-id="24f6c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="24f6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="24f6c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24f6c-111">Permission type</span></span>|<span data-ttu-id="24f6c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24f6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24f6c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24f6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24f6c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24f6c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24f6c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24f6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24f6c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24f6c-116">Not supported.</span></span>|
|<span data-ttu-id="24f6c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24f6c-117">Application</span></span>|<span data-ttu-id="24f6c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24f6c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24f6c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24f6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="24f6c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24f6c-120">Request headers</span></span>
|<span data-ttu-id="24f6c-121">Header</span><span class="sxs-lookup"><span data-stu-id="24f6c-121">Header</span></span>|<span data-ttu-id="24f6c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="24f6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24f6c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="24f6c-123">Authorization</span></span>|<span data-ttu-id="24f6c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="24f6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24f6c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="24f6c-125">Accept</span></span>|<span data-ttu-id="24f6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24f6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24f6c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24f6c-127">Request body</span></span>
<span data-ttu-id="24f6c-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedMobileApp“ an.</span><span class="sxs-lookup"><span data-stu-id="24f6c-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="24f6c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedMobileApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="24f6c-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="24f6c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24f6c-130">Property</span></span>|<span data-ttu-id="24f6c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="24f6c-131">Type</span></span>|<span data-ttu-id="24f6c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24f6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24f6c-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="24f6c-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="24f6c-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="24f6c-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="24f6c-135">Bezeichner der App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="24f6c-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="24f6c-136">id</span><span class="sxs-lookup"><span data-stu-id="24f6c-136">id</span></span>|<span data-ttu-id="24f6c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24f6c-137">String</span></span>|<span data-ttu-id="24f6c-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="24f6c-138">Key of the entity.</span></span>|
|<span data-ttu-id="24f6c-139">Version</span><span class="sxs-lookup"><span data-stu-id="24f6c-139">version</span></span>|<span data-ttu-id="24f6c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24f6c-140">String</span></span>|<span data-ttu-id="24f6c-141">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="24f6c-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="24f6c-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="24f6c-142">Response</span></span>
<span data-ttu-id="24f6c-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="24f6c-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24f6c-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24f6c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="24f6c-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24f6c-145">Request</span></span>
<span data-ttu-id="24f6c-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24f6c-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="24f6c-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="24f6c-147">Response</span></span>
<span data-ttu-id="24f6c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24f6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




