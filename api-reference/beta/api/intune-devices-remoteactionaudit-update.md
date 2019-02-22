---
title: Remote Action Audit aktualisieren
description: Aktualisieren der Eigenschaften eines Remote Action Audit-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6105145c9e284c1f522c85f6a1237dcb2320fa28
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170224"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="d3620-103">Remote Action Audit aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d3620-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="d3620-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3620-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3620-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d3620-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3620-106">Aktualisieren der Eigenschaften eines [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d3620-106">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3620-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3620-107">Prerequisites</span></span>
<span data-ttu-id="d3620-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d3620-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3620-110">Permission type</span></span>|<span data-ttu-id="d3620-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3620-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3620-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3620-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3620-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3620-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d3620-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3620-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3620-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3620-115">Not supported.</span></span>|
|<span data-ttu-id="d3620-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3620-116">Application</span></span>|<span data-ttu-id="d3620-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3620-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3620-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3620-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="d3620-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3620-119">Request headers</span></span>
|<span data-ttu-id="d3620-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3620-120">Header</span></span>|<span data-ttu-id="d3620-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d3620-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3620-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3620-122">Authorization</span></span>|<span data-ttu-id="d3620-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3620-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3620-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d3620-124">Accept</span></span>|<span data-ttu-id="d3620-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3620-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3620-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3620-126">Request body</span></span>
<span data-ttu-id="d3620-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d3620-127">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="d3620-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d3620-128">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="d3620-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3620-129">Property</span></span>|<span data-ttu-id="d3620-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d3620-130">Type</span></span>|<span data-ttu-id="d3620-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3620-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3620-132">id</span><span class="sxs-lookup"><span data-stu-id="d3620-132">id</span></span>|<span data-ttu-id="d3620-133">String</span><span class="sxs-lookup"><span data-stu-id="d3620-133">String</span></span>|<span data-ttu-id="d3620-134">Berichts-ID.</span><span class="sxs-lookup"><span data-stu-id="d3620-134">Report Id.</span></span>|
|<span data-ttu-id="d3620-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d3620-135">deviceDisplayName</span></span>|<span data-ttu-id="d3620-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3620-136">String</span></span>|<span data-ttu-id="d3620-137">InTune-Gerätename.</span><span class="sxs-lookup"><span data-stu-id="d3620-137">Intune device name.</span></span>|
|<span data-ttu-id="d3620-138">userName</span><span class="sxs-lookup"><span data-stu-id="d3620-138">userName</span></span>|<span data-ttu-id="d3620-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3620-139">String</span></span>|<span data-ttu-id="d3620-140">\[veraltet verwenden\] Sie stattdessen Eigenschaften initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="d3620-140">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="d3620-141">Eigenschaften initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="d3620-141">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="d3620-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3620-142">String</span></span>|<span data-ttu-id="d3620-143">Benutzer, der die Geräte Aktion initiiert hat, Format ist UPN.</span><span class="sxs-lookup"><span data-stu-id="d3620-143">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="d3620-144">Aktion</span><span class="sxs-lookup"><span data-stu-id="d3620-144">action</span></span>|[<span data-ttu-id="d3620-145">Remote-Steuerung</span><span class="sxs-lookup"><span data-stu-id="d3620-145">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="d3620-146">Der Name der Aktion.</span><span class="sxs-lookup"><span data-stu-id="d3620-146">The action name.</span></span> <span data-ttu-id="d3620-147">Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures`,,,,,,,, `factoryResetKeepEnrollmentData`,, `shutDown` ,,,,,, `updateDeviceAccount` `automaticRedeployment` `locateDevice` .</span><span class="sxs-lookup"><span data-stu-id="d3620-147">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="d3620-148">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="d3620-148">requestDateTime</span></span>|<span data-ttu-id="d3620-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3620-149">DateTimeOffset</span></span>|<span data-ttu-id="d3620-150">Zeitpunkt der Ausgabe der Aktion in UTC.</span><span class="sxs-lookup"><span data-stu-id="d3620-150">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="d3620-151">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d3620-151">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="d3620-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3620-152">String</span></span>|<span data-ttu-id="d3620-153">UPN des Geräte Besitzers.</span><span class="sxs-lookup"><span data-stu-id="d3620-153">Upn of the device owner.</span></span>|
|<span data-ttu-id="d3620-154">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="d3620-154">deviceIMEI</span></span>|<span data-ttu-id="d3620-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3620-155">String</span></span>|<span data-ttu-id="d3620-156">IMEI des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d3620-156">IMEI of the device.</span></span>|
|<span data-ttu-id="d3620-157">actionState</span><span class="sxs-lookup"><span data-stu-id="d3620-157">actionState</span></span>|[<span data-ttu-id="d3620-158">actionState</span><span class="sxs-lookup"><span data-stu-id="d3620-158">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d3620-159">Aktionsstatus.</span><span class="sxs-lookup"><span data-stu-id="d3620-159">Action state.</span></span> <span data-ttu-id="d3620-160">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d3620-160">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="d3620-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3620-161">Response</span></span>
<span data-ttu-id="d3620-162">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d3620-162">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3620-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3620-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3620-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3620-164">Request</span></span>
<span data-ttu-id="d3620-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3620-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a><span data-ttu-id="d3620-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3620-166">Response</span></span>
<span data-ttu-id="d3620-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3620-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```




