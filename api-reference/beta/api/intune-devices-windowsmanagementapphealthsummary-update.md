---
title: WindowsManagementAppHealthSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsManagementAppHealthSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6749c6858f51295b1221afecf802fa088a952a7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965606"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="3b76a-103">WindowsManagementAppHealthSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3b76a-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="3b76a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b76a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b76a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3b76a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b76a-106">Aktualisieren der Eigenschaften eines [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3b76a-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b76a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b76a-107">Prerequisites</span></span>
<span data-ttu-id="3b76a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b76a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b76a-110">Permission type</span></span>|<span data-ttu-id="3b76a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b76a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b76a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b76a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b76a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b76a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b76a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b76a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b76a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b76a-115">Not supported.</span></span>|
|<span data-ttu-id="3b76a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b76a-116">Application</span></span>|<span data-ttu-id="3b76a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b76a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b76a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b76a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="3b76a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b76a-119">Request headers</span></span>
|<span data-ttu-id="3b76a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3b76a-120">Header</span></span>|<span data-ttu-id="3b76a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3b76a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b76a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b76a-122">Authorization</span></span>|<span data-ttu-id="3b76a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b76a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b76a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3b76a-124">Accept</span></span>|<span data-ttu-id="3b76a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b76a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b76a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b76a-126">Request body</span></span>
<span data-ttu-id="3b76a-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="3b76a-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="3b76a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3b76a-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="3b76a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b76a-129">Property</span></span>|<span data-ttu-id="3b76a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3b76a-130">Type</span></span>|<span data-ttu-id="3b76a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b76a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b76a-132">id</span><span class="sxs-lookup"><span data-stu-id="3b76a-132">id</span></span>|<span data-ttu-id="3b76a-133">String</span><span class="sxs-lookup"><span data-stu-id="3b76a-133">String</span></span>|<span data-ttu-id="3b76a-134">Schlüssel der Status Zusammenfassungs Entität der Windows-Verwaltungs app.</span><span class="sxs-lookup"><span data-stu-id="3b76a-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="3b76a-135">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b76a-135">healthyDeviceCount</span></span>|<span data-ttu-id="3b76a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3b76a-136">Int32</span></span>|<span data-ttu-id="3b76a-137">Anzahl der fehlerfreien Geräte.</span><span class="sxs-lookup"><span data-stu-id="3b76a-137">Healthy device count.</span></span>|
|<span data-ttu-id="3b76a-138">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b76a-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="3b76a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3b76a-139">Int32</span></span>|<span data-ttu-id="3b76a-140">Fehlerhafte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="3b76a-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="3b76a-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b76a-141">unknownDeviceCount</span></span>|<span data-ttu-id="3b76a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3b76a-142">Int32</span></span>|<span data-ttu-id="3b76a-143">Unbekannte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="3b76a-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3b76a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b76a-144">Response</span></span>
<span data-ttu-id="3b76a-145">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3b76a-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b76a-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b76a-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b76a-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b76a-147">Request</span></span>
<span data-ttu-id="3b76a-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b76a-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b76a-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b76a-149">Response</span></span>
<span data-ttu-id="3b76a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b76a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




