---
title: Remote Action Audit erstellen
description: Erstellen eines neuen Remote Action Audit-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1686005b04e0e9fbf8376f7e14455937feff65af
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167431"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="3ba68-103">Remote Action Audit erstellen</span><span class="sxs-lookup"><span data-stu-id="3ba68-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="3ba68-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ba68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ba68-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3ba68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ba68-106">Erstellen eines neuen [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ba68-106">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ba68-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ba68-107">Prerequisites</span></span>
<span data-ttu-id="3ba68-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ba68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3ba68-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ba68-110">Permission type</span></span>|<span data-ttu-id="3ba68-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ba68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ba68-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ba68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ba68-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ba68-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3ba68-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ba68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ba68-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ba68-115">Not supported.</span></span>|
|<span data-ttu-id="3ba68-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ba68-116">Application</span></span>|<span data-ttu-id="3ba68-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ba68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ba68-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ba68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="3ba68-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ba68-119">Request headers</span></span>
|<span data-ttu-id="3ba68-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3ba68-120">Header</span></span>|<span data-ttu-id="3ba68-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3ba68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ba68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ba68-122">Authorization</span></span>|<span data-ttu-id="3ba68-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ba68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ba68-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3ba68-124">Accept</span></span>|<span data-ttu-id="3ba68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ba68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ba68-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ba68-126">Request body</span></span>
<span data-ttu-id="3ba68-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das Remote Action Audit-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="3ba68-127">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="3ba68-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der Remote Action Audit erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3ba68-128">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="3ba68-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ba68-129">Property</span></span>|<span data-ttu-id="3ba68-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3ba68-130">Type</span></span>|<span data-ttu-id="3ba68-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ba68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ba68-132">id</span><span class="sxs-lookup"><span data-stu-id="3ba68-132">id</span></span>|<span data-ttu-id="3ba68-133">String</span><span class="sxs-lookup"><span data-stu-id="3ba68-133">String</span></span>|<span data-ttu-id="3ba68-134">Berichts-ID.</span><span class="sxs-lookup"><span data-stu-id="3ba68-134">Report Id.</span></span>|
|<span data-ttu-id="3ba68-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3ba68-135">deviceDisplayName</span></span>|<span data-ttu-id="3ba68-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ba68-136">String</span></span>|<span data-ttu-id="3ba68-137">InTune-Gerätename.</span><span class="sxs-lookup"><span data-stu-id="3ba68-137">Intune device name.</span></span>|
|<span data-ttu-id="3ba68-138">userName</span><span class="sxs-lookup"><span data-stu-id="3ba68-138">userName</span></span>|<span data-ttu-id="3ba68-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ba68-139">String</span></span>|<span data-ttu-id="3ba68-140">\[veraltet verwenden\] Sie stattdessen Eigenschaften initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="3ba68-140">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="3ba68-141">Eigenschaften initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="3ba68-141">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="3ba68-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ba68-142">String</span></span>|<span data-ttu-id="3ba68-143">Benutzer, der die Geräte Aktion initiiert hat, Format ist UPN.</span><span class="sxs-lookup"><span data-stu-id="3ba68-143">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="3ba68-144">Aktion</span><span class="sxs-lookup"><span data-stu-id="3ba68-144">action</span></span>|[<span data-ttu-id="3ba68-145">Remote-Steuerung</span><span class="sxs-lookup"><span data-stu-id="3ba68-145">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="3ba68-146">Der Name der Aktion.</span><span class="sxs-lookup"><span data-stu-id="3ba68-146">The action name.</span></span> <span data-ttu-id="3ba68-147">Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures`,,,,,,,, `factoryResetKeepEnrollmentData`,, `shutDown` ,,,,,, `updateDeviceAccount` `automaticRedeployment` `locateDevice` .</span><span class="sxs-lookup"><span data-stu-id="3ba68-147">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="3ba68-148">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="3ba68-148">requestDateTime</span></span>|<span data-ttu-id="3ba68-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ba68-149">DateTimeOffset</span></span>|<span data-ttu-id="3ba68-150">Zeitpunkt der Ausgabe der Aktion in UTC.</span><span class="sxs-lookup"><span data-stu-id="3ba68-150">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="3ba68-151">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3ba68-151">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="3ba68-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ba68-152">String</span></span>|<span data-ttu-id="3ba68-153">UPN des Geräte Besitzers.</span><span class="sxs-lookup"><span data-stu-id="3ba68-153">Upn of the device owner.</span></span>|
|<span data-ttu-id="3ba68-154">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="3ba68-154">deviceIMEI</span></span>|<span data-ttu-id="3ba68-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ba68-155">String</span></span>|<span data-ttu-id="3ba68-156">IMEI des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3ba68-156">IMEI of the device.</span></span>|
|<span data-ttu-id="3ba68-157">actionState</span><span class="sxs-lookup"><span data-stu-id="3ba68-157">actionState</span></span>|[<span data-ttu-id="3ba68-158">actionState</span><span class="sxs-lookup"><span data-stu-id="3ba68-158">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3ba68-159">Aktionsstatus.</span><span class="sxs-lookup"><span data-stu-id="3ba68-159">Action state.</span></span> <span data-ttu-id="3ba68-160">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3ba68-160">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="3ba68-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ba68-161">Response</span></span>
<span data-ttu-id="3ba68-162">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3ba68-162">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ba68-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ba68-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ba68-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ba68-164">Request</span></span>
<span data-ttu-id="3ba68-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ba68-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
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

### <a name="response"></a><span data-ttu-id="3ba68-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ba68-166">Response</span></span>
<span data-ttu-id="3ba68-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ba68-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




