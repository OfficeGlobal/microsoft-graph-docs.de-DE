---
title: softwareUpdateStatusSummary aktualisieren
description: Aktualisieren der Eigenschaften eines softwareUpdateStatusSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76475402e0bb240606cfff0ed25b4502b2feb206
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145094"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="7c54f-103">softwareUpdateStatusSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7c54f-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="7c54f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c54f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c54f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7c54f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c54f-106">Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c54f-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c54f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c54f-107">Prerequisites</span></span>
<span data-ttu-id="7c54f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c54f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c54f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c54f-110">Permission type</span></span>|<span data-ttu-id="7c54f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c54f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c54f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c54f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c54f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c54f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c54f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c54f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c54f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c54f-115">Not supported.</span></span>|
|<span data-ttu-id="7c54f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c54f-116">Application</span></span>|<span data-ttu-id="7c54f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c54f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c54f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c54f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="7c54f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c54f-119">Request headers</span></span>
|<span data-ttu-id="7c54f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c54f-120">Header</span></span>|<span data-ttu-id="7c54f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7c54f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c54f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c54f-122">Authorization</span></span>|<span data-ttu-id="7c54f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c54f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c54f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c54f-124">Accept</span></span>|<span data-ttu-id="7c54f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c54f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c54f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c54f-126">Request body</span></span>
<span data-ttu-id="7c54f-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="7c54f-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="7c54f-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c54f-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="7c54f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c54f-129">Property</span></span>|<span data-ttu-id="7c54f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7c54f-130">Type</span></span>|<span data-ttu-id="7c54f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c54f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c54f-132">id</span><span class="sxs-lookup"><span data-stu-id="7c54f-132">id</span></span>|<span data-ttu-id="7c54f-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c54f-133">String</span></span>|<span data-ttu-id="7c54f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7c54f-134">Key of the entity.</span></span>|
|<span data-ttu-id="7c54f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7c54f-135">displayName</span></span>|<span data-ttu-id="7c54f-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c54f-136">String</span></span>|<span data-ttu-id="7c54f-137">Der Name der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7c54f-137">The name of the policy.</span></span>|
|<span data-ttu-id="7c54f-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-138">compliantDeviceCount</span></span>|<span data-ttu-id="7c54f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-139">Int32</span></span>|<span data-ttu-id="7c54f-140">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="7c54f-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="7c54f-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7c54f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-142">Int32</span></span>|<span data-ttu-id="7c54f-143">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="7c54f-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="7c54f-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-144">remediatedDeviceCount</span></span>|<span data-ttu-id="7c54f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-145">Int32</span></span>|<span data-ttu-id="7c54f-146">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="7c54f-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="7c54f-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-147">errorDeviceCount</span></span>|<span data-ttu-id="7c54f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-148">Int32</span></span>|<span data-ttu-id="7c54f-149">Anzahl der Geräte mit Fehler</span><span class="sxs-lookup"><span data-stu-id="7c54f-149">Number of devices had error.</span></span>|
|<span data-ttu-id="7c54f-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-150">unknownDeviceCount</span></span>|<span data-ttu-id="7c54f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-151">Int32</span></span>|<span data-ttu-id="7c54f-152">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="7c54f-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="7c54f-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-153">conflictDeviceCount</span></span>|<span data-ttu-id="7c54f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-154">Int32</span></span>|<span data-ttu-id="7c54f-155">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="7c54f-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="7c54f-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="7c54f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-157">Int32</span></span>|<span data-ttu-id="7c54f-158">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="7c54f-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="7c54f-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-159">compliantUserCount</span></span>|<span data-ttu-id="7c54f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-160">Int32</span></span>|<span data-ttu-id="7c54f-161">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="7c54f-161">Number of compliant users.</span></span>|
|<span data-ttu-id="7c54f-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-162">nonCompliantUserCount</span></span>|<span data-ttu-id="7c54f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-163">Int32</span></span>|<span data-ttu-id="7c54f-164">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="7c54f-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="7c54f-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-165">remediatedUserCount</span></span>|<span data-ttu-id="7c54f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-166">Int32</span></span>|<span data-ttu-id="7c54f-167">Anzahl der korrigierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="7c54f-167">Number of remediated users.</span></span>|
|<span data-ttu-id="7c54f-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-168">errorUserCount</span></span>|<span data-ttu-id="7c54f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-169">Int32</span></span>|<span data-ttu-id="7c54f-170">Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="7c54f-170">Number of users had error.</span></span>|
|<span data-ttu-id="7c54f-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-171">unknownUserCount</span></span>|<span data-ttu-id="7c54f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-172">Int32</span></span>|<span data-ttu-id="7c54f-173">Anzahl der unbekannten Benutzer</span><span class="sxs-lookup"><span data-stu-id="7c54f-173">Number of unknown users.</span></span>|
|<span data-ttu-id="7c54f-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-174">conflictUserCount</span></span>|<span data-ttu-id="7c54f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-175">Int32</span></span>|<span data-ttu-id="7c54f-176">Anzahl der Benutzer mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="7c54f-176">Number of conflict users.</span></span>|
|<span data-ttu-id="7c54f-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="7c54f-177">notApplicableUserCount</span></span>|<span data-ttu-id="7c54f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="7c54f-178">Int32</span></span>|<span data-ttu-id="7c54f-179">Anzahl der nicht anwendbaren Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7c54f-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="7c54f-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c54f-180">Response</span></span>
<span data-ttu-id="7c54f-181">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c54f-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c54f-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c54f-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c54f-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c54f-183">Request</span></span>
<span data-ttu-id="7c54f-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c54f-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="7c54f-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c54f-185">Response</span></span>
<span data-ttu-id="7c54f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c54f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```




