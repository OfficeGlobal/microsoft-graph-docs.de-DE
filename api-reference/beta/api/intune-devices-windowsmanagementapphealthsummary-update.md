---
title: WindowsManagementAppHealthSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagementAppHealthSummary-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7e8c077b8f06b9647e34a18fd5aa92987272e77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394166"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="fc6ab-103">WindowsManagementAppHealthSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fc6ab-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="fc6ab-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc6ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc6ab-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc6ab-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc6ab-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fc6ab-108">Prerequisites</span></span>
<span data-ttu-id="fc6ab-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc6ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fc6ab-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc6ab-111">Permission type</span></span>|<span data-ttu-id="fc6ab-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc6ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc6ab-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc6ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc6ab-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc6ab-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fc6ab-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc6ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc6ab-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc6ab-116">Not supported.</span></span>|
|<span data-ttu-id="fc6ab-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc6ab-117">Application</span></span>|<span data-ttu-id="fc6ab-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc6ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc6ab-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc6ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="fc6ab-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc6ab-120">Request headers</span></span>
|<span data-ttu-id="fc6ab-121">Header</span><span class="sxs-lookup"><span data-stu-id="fc6ab-121">Header</span></span>|<span data-ttu-id="fc6ab-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fc6ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc6ab-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fc6ab-123">Authorization</span></span>|<span data-ttu-id="fc6ab-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc6ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc6ab-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fc6ab-125">Accept</span></span>|<span data-ttu-id="fc6ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc6ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc6ab-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc6ab-127">Request body</span></span>
<span data-ttu-id="fc6ab-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="fc6ab-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="fc6ab-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc6ab-130">Property</span></span>|<span data-ttu-id="fc6ab-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fc6ab-131">Type</span></span>|<span data-ttu-id="fc6ab-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc6ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc6ab-133">id</span><span class="sxs-lookup"><span data-stu-id="fc6ab-133">id</span></span>|<span data-ttu-id="fc6ab-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc6ab-134">String</span></span>|<span data-ttu-id="fc6ab-135">Schlüssel der Windows Management app Health Zusammenfassung Entität.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="fc6ab-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc6ab-136">healthyDeviceCount</span></span>|<span data-ttu-id="fc6ab-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fc6ab-137">Int32</span></span>|<span data-ttu-id="fc6ab-138">Anzahl der fehlerfrei Geräte.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-138">Healthy device count.</span></span>|
|<span data-ttu-id="fc6ab-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc6ab-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="fc6ab-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fc6ab-140">Int32</span></span>|<span data-ttu-id="fc6ab-141">Anzahl der fehlerhaften Geräte.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="fc6ab-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc6ab-142">unknownDeviceCount</span></span>|<span data-ttu-id="fc6ab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fc6ab-143">Int32</span></span>|<span data-ttu-id="fc6ab-144">Anzahl der unbekannten Geräte.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="fc6ab-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc6ab-145">Response</span></span>
<span data-ttu-id="fc6ab-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc6ab-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc6ab-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc6ab-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc6ab-148">Request</span></span>
<span data-ttu-id="fc6ab-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc6ab-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc6ab-150">Response</span></span>
<span data-ttu-id="fc6ab-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc6ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




