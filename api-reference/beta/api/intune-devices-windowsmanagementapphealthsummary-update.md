---
title: WindowsManagementAppHealthSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsManagementAppHealthSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 764549ee57bc3ab3a2a1e0c2db9c6ac16309b85d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155965"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="8905b-103">WindowsManagementAppHealthSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8905b-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="8905b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8905b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8905b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8905b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8905b-106">Aktualisieren der Eigenschaften eines [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8905b-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8905b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8905b-107">Prerequisites</span></span>
<span data-ttu-id="8905b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8905b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8905b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8905b-110">Permission type</span></span>|<span data-ttu-id="8905b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8905b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8905b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8905b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8905b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8905b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8905b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8905b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8905b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8905b-115">Not supported.</span></span>|
|<span data-ttu-id="8905b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8905b-116">Application</span></span>|<span data-ttu-id="8905b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8905b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8905b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8905b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="8905b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8905b-119">Request headers</span></span>
|<span data-ttu-id="8905b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8905b-120">Header</span></span>|<span data-ttu-id="8905b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8905b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8905b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8905b-122">Authorization</span></span>|<span data-ttu-id="8905b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8905b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8905b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8905b-124">Accept</span></span>|<span data-ttu-id="8905b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8905b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8905b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8905b-126">Request body</span></span>
<span data-ttu-id="8905b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8905b-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="8905b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8905b-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="8905b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8905b-129">Property</span></span>|<span data-ttu-id="8905b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8905b-130">Type</span></span>|<span data-ttu-id="8905b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8905b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8905b-132">id</span><span class="sxs-lookup"><span data-stu-id="8905b-132">id</span></span>|<span data-ttu-id="8905b-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8905b-133">String</span></span>|<span data-ttu-id="8905b-134">Schlüssel der Status Zusammenfassungs Entität der Windows-Verwaltungs app.</span><span class="sxs-lookup"><span data-stu-id="8905b-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="8905b-135">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8905b-135">healthyDeviceCount</span></span>|<span data-ttu-id="8905b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8905b-136">Int32</span></span>|<span data-ttu-id="8905b-137">Anzahl der fehlerfreien Geräte.</span><span class="sxs-lookup"><span data-stu-id="8905b-137">Healthy device count.</span></span>|
|<span data-ttu-id="8905b-138">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8905b-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="8905b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8905b-139">Int32</span></span>|<span data-ttu-id="8905b-140">Fehlerhafte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="8905b-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="8905b-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8905b-141">unknownDeviceCount</span></span>|<span data-ttu-id="8905b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8905b-142">Int32</span></span>|<span data-ttu-id="8905b-143">Unbekannte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="8905b-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="8905b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="8905b-144">Response</span></span>
<span data-ttu-id="8905b-145">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8905b-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8905b-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8905b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="8905b-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8905b-147">Request</span></span>
<span data-ttu-id="8905b-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8905b-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="8905b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8905b-149">Response</span></span>
<span data-ttu-id="8905b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8905b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```




