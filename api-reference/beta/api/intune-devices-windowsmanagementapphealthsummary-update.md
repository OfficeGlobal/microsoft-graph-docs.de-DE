---
title: WindowsManagementAppHealthSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagementAppHealthSummary-Objekts.
author: tfitzmac
ms.openlocfilehash: 274ffcc65706f7d730815d4a8350af2dee68f763
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307070"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="288d4-103">WindowsManagementAppHealthSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="288d4-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="288d4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="288d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="288d4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="288d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="288d4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="288d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="288d4-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="288d4-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="288d4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="288d4-108">Prerequisites</span></span>
<span data-ttu-id="288d4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="288d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="288d4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="288d4-111">Permission type</span></span>|<span data-ttu-id="288d4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="288d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="288d4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="288d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="288d4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="288d4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="288d4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="288d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="288d4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="288d4-116">Not supported.</span></span>|
|<span data-ttu-id="288d4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="288d4-117">Application</span></span>|<span data-ttu-id="288d4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="288d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="288d4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="288d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="288d4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="288d4-120">Request headers</span></span>
|<span data-ttu-id="288d4-121">Header</span><span class="sxs-lookup"><span data-stu-id="288d4-121">Header</span></span>|<span data-ttu-id="288d4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="288d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="288d4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="288d4-123">Authorization</span></span>|<span data-ttu-id="288d4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="288d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="288d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="288d4-125">Accept</span></span>|<span data-ttu-id="288d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="288d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="288d4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="288d4-127">Request body</span></span>
<span data-ttu-id="288d4-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="288d4-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="288d4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="288d4-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="288d4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="288d4-130">Property</span></span>|<span data-ttu-id="288d4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="288d4-131">Type</span></span>|<span data-ttu-id="288d4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="288d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="288d4-133">id</span><span class="sxs-lookup"><span data-stu-id="288d4-133">id</span></span>|<span data-ttu-id="288d4-134">String</span><span class="sxs-lookup"><span data-stu-id="288d4-134">String</span></span>|<span data-ttu-id="288d4-135">Schlüssel der Windows Management app Health Zusammenfassung Entität.</span><span class="sxs-lookup"><span data-stu-id="288d4-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="288d4-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="288d4-136">healthyDeviceCount</span></span>|<span data-ttu-id="288d4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="288d4-137">Int32</span></span>|<span data-ttu-id="288d4-138">Anzahl der fehlerfrei Geräte.</span><span class="sxs-lookup"><span data-stu-id="288d4-138">Healthy device count.</span></span>|
|<span data-ttu-id="288d4-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="288d4-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="288d4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="288d4-140">Int32</span></span>|<span data-ttu-id="288d4-141">Anzahl der fehlerhaften Geräte.</span><span class="sxs-lookup"><span data-stu-id="288d4-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="288d4-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="288d4-142">unknownDeviceCount</span></span>|<span data-ttu-id="288d4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="288d4-143">Int32</span></span>|<span data-ttu-id="288d4-144">Anzahl der unbekannten Geräte.</span><span class="sxs-lookup"><span data-stu-id="288d4-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="288d4-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="288d4-145">Response</span></span>
<span data-ttu-id="288d4-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="288d4-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="288d4-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="288d4-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="288d4-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="288d4-148">Request</span></span>
<span data-ttu-id="288d4-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="288d4-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 89

{
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="288d4-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="288d4-150">Response</span></span>
<span data-ttu-id="288d4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="288d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





