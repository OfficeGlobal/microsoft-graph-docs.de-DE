---
title: softwareUpdateStatusSummary aktualisieren
description: Aktualisieren der Eigenschaften eines softwareUpdateStatusSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ea208150ac85aefb4fb3e34b4d081d02089bdee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982413"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="09145-103">softwareUpdateStatusSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="09145-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="09145-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="09145-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09145-105">Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="09145-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09145-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09145-106">Prerequisites</span></span>
<span data-ttu-id="09145-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09145-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09145-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09145-109">Permission type</span></span>|<span data-ttu-id="09145-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09145-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09145-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09145-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09145-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09145-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09145-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09145-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09145-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09145-114">Not supported.</span></span>|
|<span data-ttu-id="09145-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09145-115">Application</span></span>|<span data-ttu-id="09145-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09145-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09145-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09145-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="09145-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09145-118">Request headers</span></span>
|<span data-ttu-id="09145-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="09145-119">Header</span></span>|<span data-ttu-id="09145-120">Wert</span><span class="sxs-lookup"><span data-stu-id="09145-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09145-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09145-121">Authorization</span></span>|<span data-ttu-id="09145-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09145-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09145-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09145-123">Accept</span></span>|<span data-ttu-id="09145-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09145-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09145-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09145-125">Request body</span></span>
<span data-ttu-id="09145-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="09145-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="09145-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="09145-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="09145-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09145-128">Property</span></span>|<span data-ttu-id="09145-129">Typ</span><span class="sxs-lookup"><span data-stu-id="09145-129">Type</span></span>|<span data-ttu-id="09145-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09145-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09145-131">id</span><span class="sxs-lookup"><span data-stu-id="09145-131">id</span></span>|<span data-ttu-id="09145-132">String</span><span class="sxs-lookup"><span data-stu-id="09145-132">String</span></span>|<span data-ttu-id="09145-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="09145-133">Key of the entity.</span></span>|
|<span data-ttu-id="09145-134">displayName</span><span class="sxs-lookup"><span data-stu-id="09145-134">displayName</span></span>|<span data-ttu-id="09145-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09145-135">String</span></span>|<span data-ttu-id="09145-136">Der Name der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="09145-136">The name of the policy.</span></span>|
|<span data-ttu-id="09145-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-137">compliantDeviceCount</span></span>|<span data-ttu-id="09145-138">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-138">Int32</span></span>|<span data-ttu-id="09145-139">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="09145-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="09145-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="09145-141">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-141">Int32</span></span>|<span data-ttu-id="09145-142">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="09145-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="09145-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-143">remediatedDeviceCount</span></span>|<span data-ttu-id="09145-144">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-144">Int32</span></span>|<span data-ttu-id="09145-145">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="09145-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="09145-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-146">errorDeviceCount</span></span>|<span data-ttu-id="09145-147">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-147">Int32</span></span>|<span data-ttu-id="09145-148">Anzahl der Geräte mit Fehler</span><span class="sxs-lookup"><span data-stu-id="09145-148">Number of devices had error.</span></span>|
|<span data-ttu-id="09145-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-149">unknownDeviceCount</span></span>|<span data-ttu-id="09145-150">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-150">Int32</span></span>|<span data-ttu-id="09145-151">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="09145-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="09145-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-152">conflictDeviceCount</span></span>|<span data-ttu-id="09145-153">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-153">Int32</span></span>|<span data-ttu-id="09145-154">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="09145-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="09145-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09145-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="09145-156">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-156">Int32</span></span>|<span data-ttu-id="09145-157">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="09145-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="09145-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-158">compliantUserCount</span></span>|<span data-ttu-id="09145-159">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-159">Int32</span></span>|<span data-ttu-id="09145-160">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="09145-160">Number of compliant users.</span></span>|
|<span data-ttu-id="09145-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-161">nonCompliantUserCount</span></span>|<span data-ttu-id="09145-162">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-162">Int32</span></span>|<span data-ttu-id="09145-163">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="09145-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="09145-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-164">remediatedUserCount</span></span>|<span data-ttu-id="09145-165">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-165">Int32</span></span>|<span data-ttu-id="09145-166">Anzahl der korrigierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="09145-166">Number of remediated users.</span></span>|
|<span data-ttu-id="09145-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-167">errorUserCount</span></span>|<span data-ttu-id="09145-168">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-168">Int32</span></span>|<span data-ttu-id="09145-169">Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="09145-169">Number of users had error.</span></span>|
|<span data-ttu-id="09145-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-170">unknownUserCount</span></span>|<span data-ttu-id="09145-171">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-171">Int32</span></span>|<span data-ttu-id="09145-172">Anzahl der unbekannten Benutzer</span><span class="sxs-lookup"><span data-stu-id="09145-172">Number of unknown users.</span></span>|
|<span data-ttu-id="09145-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-173">conflictUserCount</span></span>|<span data-ttu-id="09145-174">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-174">Int32</span></span>|<span data-ttu-id="09145-175">Anzahl der Benutzer mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="09145-175">Number of conflict users.</span></span>|
|<span data-ttu-id="09145-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="09145-176">notApplicableUserCount</span></span>|<span data-ttu-id="09145-177">Int32</span><span class="sxs-lookup"><span data-stu-id="09145-177">Int32</span></span>|<span data-ttu-id="09145-178">Anzahl der nicht anwendbaren Benutzer.</span><span class="sxs-lookup"><span data-stu-id="09145-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="09145-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="09145-179">Response</span></span>
<span data-ttu-id="09145-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="09145-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09145-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09145-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="09145-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09145-182">Request</span></span>
<span data-ttu-id="09145-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09145-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
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

### <a name="response"></a><span data-ttu-id="09145-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="09145-184">Response</span></span>
<span data-ttu-id="09145-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09145-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



