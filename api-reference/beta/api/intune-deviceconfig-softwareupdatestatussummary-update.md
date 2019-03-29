---
title: softwareUpdateStatusSummary aktualisieren
description: Aktualisieren der Eigenschaften eines softwareUpdateStatusSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb2d0cf3c2dd048f2f1668d2cc88bf24871c0e84
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963772"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="7739e-103">softwareUpdateStatusSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7739e-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="7739e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7739e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7739e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7739e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7739e-106">Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7739e-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7739e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7739e-107">Prerequisites</span></span>
<span data-ttu-id="7739e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7739e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7739e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7739e-110">Permission type</span></span>|<span data-ttu-id="7739e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7739e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7739e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7739e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7739e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7739e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7739e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7739e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7739e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7739e-115">Not supported.</span></span>|
|<span data-ttu-id="7739e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7739e-116">Application</span></span>|<span data-ttu-id="7739e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7739e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7739e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7739e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="7739e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7739e-119">Request headers</span></span>
|<span data-ttu-id="7739e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7739e-120">Header</span></span>|<span data-ttu-id="7739e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7739e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7739e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7739e-122">Authorization</span></span>|<span data-ttu-id="7739e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7739e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7739e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7739e-124">Accept</span></span>|<span data-ttu-id="7739e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7739e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7739e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7739e-126">Request body</span></span>
<span data-ttu-id="7739e-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="7739e-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="7739e-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7739e-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="7739e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7739e-129">Property</span></span>|<span data-ttu-id="7739e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7739e-130">Type</span></span>|<span data-ttu-id="7739e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7739e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7739e-132">id</span><span class="sxs-lookup"><span data-stu-id="7739e-132">id</span></span>|<span data-ttu-id="7739e-133">String</span><span class="sxs-lookup"><span data-stu-id="7739e-133">String</span></span>|<span data-ttu-id="7739e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7739e-134">Key of the entity.</span></span>|
|<span data-ttu-id="7739e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7739e-135">displayName</span></span>|<span data-ttu-id="7739e-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7739e-136">String</span></span>|<span data-ttu-id="7739e-137">Der Name der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7739e-137">The name of the policy.</span></span>|
|<span data-ttu-id="7739e-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-138">compliantDeviceCount</span></span>|<span data-ttu-id="7739e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-139">Int32</span></span>|<span data-ttu-id="7739e-140">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="7739e-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="7739e-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7739e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-142">Int32</span></span>|<span data-ttu-id="7739e-143">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="7739e-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="7739e-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-144">remediatedDeviceCount</span></span>|<span data-ttu-id="7739e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-145">Int32</span></span>|<span data-ttu-id="7739e-146">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="7739e-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="7739e-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-147">errorDeviceCount</span></span>|<span data-ttu-id="7739e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-148">Int32</span></span>|<span data-ttu-id="7739e-149">Anzahl der Geräte mit Fehler</span><span class="sxs-lookup"><span data-stu-id="7739e-149">Number of devices had error.</span></span>|
|<span data-ttu-id="7739e-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-150">unknownDeviceCount</span></span>|<span data-ttu-id="7739e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-151">Int32</span></span>|<span data-ttu-id="7739e-152">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="7739e-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="7739e-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-153">conflictDeviceCount</span></span>|<span data-ttu-id="7739e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-154">Int32</span></span>|<span data-ttu-id="7739e-155">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="7739e-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="7739e-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7739e-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="7739e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-157">Int32</span></span>|<span data-ttu-id="7739e-158">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="7739e-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="7739e-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-159">compliantUserCount</span></span>|<span data-ttu-id="7739e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-160">Int32</span></span>|<span data-ttu-id="7739e-161">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="7739e-161">Number of compliant users.</span></span>|
|<span data-ttu-id="7739e-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-162">nonCompliantUserCount</span></span>|<span data-ttu-id="7739e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-163">Int32</span></span>|<span data-ttu-id="7739e-164">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="7739e-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="7739e-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-165">remediatedUserCount</span></span>|<span data-ttu-id="7739e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-166">Int32</span></span>|<span data-ttu-id="7739e-167">Anzahl der korrigierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="7739e-167">Number of remediated users.</span></span>|
|<span data-ttu-id="7739e-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-168">errorUserCount</span></span>|<span data-ttu-id="7739e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-169">Int32</span></span>|<span data-ttu-id="7739e-170">Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="7739e-170">Number of users had error.</span></span>|
|<span data-ttu-id="7739e-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-171">unknownUserCount</span></span>|<span data-ttu-id="7739e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-172">Int32</span></span>|<span data-ttu-id="7739e-173">Anzahl der unbekannten Benutzer</span><span class="sxs-lookup"><span data-stu-id="7739e-173">Number of unknown users.</span></span>|
|<span data-ttu-id="7739e-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-174">conflictUserCount</span></span>|<span data-ttu-id="7739e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-175">Int32</span></span>|<span data-ttu-id="7739e-176">Anzahl der Benutzer mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="7739e-176">Number of conflict users.</span></span>|
|<span data-ttu-id="7739e-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="7739e-177">notApplicableUserCount</span></span>|<span data-ttu-id="7739e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="7739e-178">Int32</span></span>|<span data-ttu-id="7739e-179">Anzahl der nicht anwendbaren Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7739e-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="7739e-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="7739e-180">Response</span></span>
<span data-ttu-id="7739e-181">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7739e-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7739e-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7739e-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="7739e-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7739e-183">Request</span></span>
<span data-ttu-id="7739e-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7739e-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7739e-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="7739e-185">Response</span></span>
<span data-ttu-id="7739e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7739e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




