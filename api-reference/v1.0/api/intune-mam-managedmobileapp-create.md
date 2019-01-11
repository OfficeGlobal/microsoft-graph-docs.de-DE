---
title: Erstellen von „managedMobileApp“
description: Diese Methode erstellt ein neues Objekt des Typs managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a79f8ce7e6cbad49c48f5b9b06bf7a86c8e414c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805180"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="9199f-103">Erstellen von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="9199f-103">Create managedMobileApp</span></span>

> <span data-ttu-id="9199f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9199f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9199f-105">Diese Methode erstellt ein neues Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9199f-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9199f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9199f-106">Prerequisites</span></span>
<span data-ttu-id="9199f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9199f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9199f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9199f-109">Permission type</span></span>|<span data-ttu-id="9199f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9199f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9199f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9199f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9199f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9199f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9199f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9199f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9199f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9199f-114">Not supported.</span></span>|
|<span data-ttu-id="9199f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9199f-115">Application</span></span>|<span data-ttu-id="9199f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9199f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9199f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9199f-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9199f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9199f-118">Request headers</span></span>
|<span data-ttu-id="9199f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9199f-119">Header</span></span>|<span data-ttu-id="9199f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9199f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9199f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9199f-121">Authorization</span></span>|<span data-ttu-id="9199f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9199f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9199f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9199f-123">Accept</span></span>|<span data-ttu-id="9199f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9199f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9199f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9199f-125">Request body</span></span>
<span data-ttu-id="9199f-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedMobileApp“ an.</span><span class="sxs-lookup"><span data-stu-id="9199f-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="9199f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedMobileApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9199f-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="9199f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9199f-128">Property</span></span>|<span data-ttu-id="9199f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9199f-129">Type</span></span>|<span data-ttu-id="9199f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9199f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9199f-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9199f-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="9199f-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9199f-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9199f-133">Bezeichner der App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="9199f-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="9199f-134">id</span><span class="sxs-lookup"><span data-stu-id="9199f-134">id</span></span>|<span data-ttu-id="9199f-135">String</span><span class="sxs-lookup"><span data-stu-id="9199f-135">String</span></span>|<span data-ttu-id="9199f-136">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9199f-136">Key of the entity.</span></span>|
|<span data-ttu-id="9199f-137">Version</span><span class="sxs-lookup"><span data-stu-id="9199f-137">version</span></span>|<span data-ttu-id="9199f-138">String</span><span class="sxs-lookup"><span data-stu-id="9199f-138">String</span></span>|<span data-ttu-id="9199f-139">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="9199f-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9199f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9199f-140">Response</span></span>
<span data-ttu-id="9199f-141">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9199f-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9199f-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9199f-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="9199f-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9199f-143">Request</span></span>
<span data-ttu-id="9199f-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9199f-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="9199f-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="9199f-145">Response</span></span>
<span data-ttu-id="9199f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9199f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



