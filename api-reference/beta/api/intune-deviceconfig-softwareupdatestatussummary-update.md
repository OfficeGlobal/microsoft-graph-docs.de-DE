---
title: softwareUpdateStatusSummary aktualisieren
description: Aktualisieren der Eigenschaften eines softwareUpdateStatusSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9696daa56c723a8bc6d5ef9d3d674ce16c6e2667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984815"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="5eee7-103">softwareUpdateStatusSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5eee7-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="5eee7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5eee7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eee7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5eee7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5eee7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5eee7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eee7-107">Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5eee7-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5eee7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5eee7-108">Prerequisites</span></span>
<span data-ttu-id="5eee7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eee7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eee7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5eee7-111">Permission type</span></span>|<span data-ttu-id="5eee7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5eee7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eee7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5eee7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5eee7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eee7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5eee7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5eee7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eee7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5eee7-116">Not supported.</span></span>|
|<span data-ttu-id="5eee7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5eee7-117">Application</span></span>|<span data-ttu-id="5eee7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5eee7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eee7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5eee7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="5eee7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5eee7-120">Request headers</span></span>
|<span data-ttu-id="5eee7-121">Header</span><span class="sxs-lookup"><span data-stu-id="5eee7-121">Header</span></span>|<span data-ttu-id="5eee7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5eee7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eee7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eee7-123">Authorization</span></span>|<span data-ttu-id="5eee7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5eee7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eee7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5eee7-125">Accept</span></span>|<span data-ttu-id="5eee7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5eee7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eee7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5eee7-127">Request body</span></span>
<span data-ttu-id="5eee7-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="5eee7-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="5eee7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5eee7-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="5eee7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5eee7-130">Property</span></span>|<span data-ttu-id="5eee7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5eee7-131">Type</span></span>|<span data-ttu-id="5eee7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5eee7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eee7-133">id</span><span class="sxs-lookup"><span data-stu-id="5eee7-133">id</span></span>|<span data-ttu-id="5eee7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5eee7-134">String</span></span>|<span data-ttu-id="5eee7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5eee7-135">Key of the entity.</span></span>|
|<span data-ttu-id="5eee7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5eee7-136">displayName</span></span>|<span data-ttu-id="5eee7-137">String</span><span class="sxs-lookup"><span data-stu-id="5eee7-137">String</span></span>|<span data-ttu-id="5eee7-138">Der Name der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5eee7-138">The name of the policy.</span></span>|
|<span data-ttu-id="5eee7-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-139">compliantDeviceCount</span></span>|<span data-ttu-id="5eee7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-140">Int32</span></span>|<span data-ttu-id="5eee7-141">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="5eee7-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="5eee7-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5eee7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-143">Int32</span></span>|<span data-ttu-id="5eee7-144">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="5eee7-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="5eee7-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-145">remediatedDeviceCount</span></span>|<span data-ttu-id="5eee7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-146">Int32</span></span>|<span data-ttu-id="5eee7-147">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="5eee7-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="5eee7-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-148">errorDeviceCount</span></span>|<span data-ttu-id="5eee7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-149">Int32</span></span>|<span data-ttu-id="5eee7-150">Anzahl der Geräte mit Fehler</span><span class="sxs-lookup"><span data-stu-id="5eee7-150">Number of devices had error.</span></span>|
|<span data-ttu-id="5eee7-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-151">unknownDeviceCount</span></span>|<span data-ttu-id="5eee7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-152">Int32</span></span>|<span data-ttu-id="5eee7-153">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="5eee7-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="5eee7-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-154">conflictDeviceCount</span></span>|<span data-ttu-id="5eee7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-155">Int32</span></span>|<span data-ttu-id="5eee7-156">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="5eee7-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="5eee7-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="5eee7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-158">Int32</span></span>|<span data-ttu-id="5eee7-159">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="5eee7-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="5eee7-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-160">compliantUserCount</span></span>|<span data-ttu-id="5eee7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-161">Int32</span></span>|<span data-ttu-id="5eee7-162">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="5eee7-162">Number of compliant users.</span></span>|
|<span data-ttu-id="5eee7-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-163">nonCompliantUserCount</span></span>|<span data-ttu-id="5eee7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-164">Int32</span></span>|<span data-ttu-id="5eee7-165">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="5eee7-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="5eee7-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-166">remediatedUserCount</span></span>|<span data-ttu-id="5eee7-167">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-167">Int32</span></span>|<span data-ttu-id="5eee7-168">Anzahl der korrigierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="5eee7-168">Number of remediated users.</span></span>|
|<span data-ttu-id="5eee7-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-169">errorUserCount</span></span>|<span data-ttu-id="5eee7-170">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-170">Int32</span></span>|<span data-ttu-id="5eee7-171">Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="5eee7-171">Number of users had error.</span></span>|
|<span data-ttu-id="5eee7-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-172">unknownUserCount</span></span>|<span data-ttu-id="5eee7-173">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-173">Int32</span></span>|<span data-ttu-id="5eee7-174">Anzahl der unbekannten Benutzer</span><span class="sxs-lookup"><span data-stu-id="5eee7-174">Number of unknown users.</span></span>|
|<span data-ttu-id="5eee7-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-175">conflictUserCount</span></span>|<span data-ttu-id="5eee7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-176">Int32</span></span>|<span data-ttu-id="5eee7-177">Anzahl der Benutzer mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="5eee7-177">Number of conflict users.</span></span>|
|<span data-ttu-id="5eee7-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5eee7-178">notApplicableUserCount</span></span>|<span data-ttu-id="5eee7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="5eee7-179">Int32</span></span>|<span data-ttu-id="5eee7-180">Anzahl der nicht anwendbaren Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5eee7-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="5eee7-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="5eee7-181">Response</span></span>
<span data-ttu-id="5eee7-182">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5eee7-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eee7-183">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5eee7-183">Example</span></span>
### <a name="request"></a><span data-ttu-id="5eee7-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5eee7-184">Request</span></span>
<span data-ttu-id="5eee7-185">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5eee7-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
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

### <a name="response"></a><span data-ttu-id="5eee7-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="5eee7-186">Response</span></span>
<span data-ttu-id="5eee7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5eee7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





