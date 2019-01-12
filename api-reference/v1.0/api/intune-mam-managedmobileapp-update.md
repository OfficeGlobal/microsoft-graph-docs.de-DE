---
title: Aktualisieren von „managedMobileApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efa34a090a52c54034e132e92e6ab853802bece3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941863"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="a0183-103">Aktualisieren von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="a0183-103">Update managedMobileApp</span></span>

> <span data-ttu-id="a0183-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a0183-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0183-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a0183-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0183-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a0183-106">Prerequisites</span></span>
<span data-ttu-id="a0183-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0183-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0183-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0183-109">Permission type</span></span>|<span data-ttu-id="a0183-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0183-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0183-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0183-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0183-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0183-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0183-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0183-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0183-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0183-114">Not supported.</span></span>|
|<span data-ttu-id="a0183-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0183-115">Application</span></span>|<span data-ttu-id="a0183-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0183-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0183-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0183-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a0183-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0183-118">Request headers</span></span>
|<span data-ttu-id="a0183-119">Header</span><span class="sxs-lookup"><span data-stu-id="a0183-119">Header</span></span>|<span data-ttu-id="a0183-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a0183-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0183-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0183-121">Authorization</span></span>|<span data-ttu-id="a0183-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a0183-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0183-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a0183-123">Accept</span></span>|<span data-ttu-id="a0183-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0183-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0183-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0183-125">Request body</span></span>
<span data-ttu-id="a0183-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="a0183-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="a0183-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a0183-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="a0183-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0183-128">Property</span></span>|<span data-ttu-id="a0183-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a0183-129">Type</span></span>|<span data-ttu-id="a0183-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0183-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0183-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a0183-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="a0183-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a0183-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a0183-133">Bezeichner der App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="a0183-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="a0183-134">id</span><span class="sxs-lookup"><span data-stu-id="a0183-134">id</span></span>|<span data-ttu-id="a0183-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0183-135">String</span></span>|<span data-ttu-id="a0183-136">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a0183-136">Key of the entity.</span></span>|
|<span data-ttu-id="a0183-137">Version</span><span class="sxs-lookup"><span data-stu-id="a0183-137">version</span></span>|<span data-ttu-id="a0183-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0183-138">String</span></span>|<span data-ttu-id="a0183-139">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="a0183-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a0183-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0183-140">Response</span></span>
<span data-ttu-id="a0183-141">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a0183-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0183-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0183-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0183-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0183-143">Request</span></span>
<span data-ttu-id="a0183-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0183-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="a0183-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0183-145">Response</span></span>
<span data-ttu-id="a0183-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0183-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



