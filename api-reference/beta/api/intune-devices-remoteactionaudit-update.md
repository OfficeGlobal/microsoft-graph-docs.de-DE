---
title: RemoteActionAudit aktualisieren
description: Aktualisieren Sie die Eigenschaften eines RemoteActionAudit-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76c61651ab18b838f2cd403036b21b3895614b19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958481"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="7d16f-103">RemoteActionAudit aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7d16f-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="7d16f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7d16f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d16f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7d16f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d16f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d16f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d16f-107">Aktualisieren Sie die Eigenschaften eines [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7d16f-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d16f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d16f-108">Prerequisites</span></span>
<span data-ttu-id="7d16f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d16f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d16f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d16f-111">Permission type</span></span>|<span data-ttu-id="7d16f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d16f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d16f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d16f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d16f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d16f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7d16f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d16f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d16f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d16f-116">Not supported.</span></span>|
|<span data-ttu-id="7d16f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d16f-117">Application</span></span>|<span data-ttu-id="7d16f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d16f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d16f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d16f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="7d16f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d16f-120">Request headers</span></span>
|<span data-ttu-id="7d16f-121">Header</span><span class="sxs-lookup"><span data-stu-id="7d16f-121">Header</span></span>|<span data-ttu-id="7d16f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7d16f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d16f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d16f-123">Authorization</span></span>|<span data-ttu-id="7d16f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7d16f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d16f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7d16f-125">Accept</span></span>|<span data-ttu-id="7d16f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d16f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d16f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d16f-127">Request body</span></span>
<span data-ttu-id="7d16f-128">Geben Sie im Textkörper Anforderung für das Objekt [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7d16f-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="7d16f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="7d16f-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="7d16f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d16f-130">Property</span></span>|<span data-ttu-id="7d16f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7d16f-131">Type</span></span>|<span data-ttu-id="7d16f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d16f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d16f-133">id</span><span class="sxs-lookup"><span data-stu-id="7d16f-133">id</span></span>|<span data-ttu-id="7d16f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d16f-134">String</span></span>|<span data-ttu-id="7d16f-135">Berichts-ID</span><span class="sxs-lookup"><span data-stu-id="7d16f-135">Report Id.</span></span>|
|<span data-ttu-id="7d16f-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7d16f-136">deviceDisplayName</span></span>|<span data-ttu-id="7d16f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d16f-137">String</span></span>|<span data-ttu-id="7d16f-138">Name des Aufnahmegeräts Intune.</span><span class="sxs-lookup"><span data-stu-id="7d16f-138">Intune device name.</span></span>|
|<span data-ttu-id="7d16f-139">userName</span><span class="sxs-lookup"><span data-stu-id="7d16f-139">userName</span></span>|<span data-ttu-id="7d16f-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d16f-140">String</span></span>|<span data-ttu-id="7d16f-141">\[veraltete\] verwenden Sie stattdessen InitiatedByUserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7d16f-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="7d16f-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7d16f-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="7d16f-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d16f-143">String</span></span>|<span data-ttu-id="7d16f-144">Benutzer, der die Aktion Gerät gestartet UPN-Format vorliegt.</span><span class="sxs-lookup"><span data-stu-id="7d16f-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="7d16f-145">Aktion</span><span class="sxs-lookup"><span data-stu-id="7d16f-145">action</span></span>|[<span data-ttu-id="7d16f-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="7d16f-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="7d16f-147">Der Name der Aktion.</span><span class="sxs-lookup"><span data-stu-id="7d16f-147">The action name.</span></span> <span data-ttu-id="7d16f-148">Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="7d16f-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="7d16f-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="7d16f-149">requestDateTime</span></span>|<span data-ttu-id="7d16f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d16f-150">DateTimeOffset</span></span>|<span data-ttu-id="7d16f-151">Zeit, wenn die Aktion ausgestellt wurde, in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="7d16f-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="7d16f-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7d16f-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="7d16f-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d16f-153">String</span></span>|<span data-ttu-id="7d16f-154">UPN des Besitzers Gerät.</span><span class="sxs-lookup"><span data-stu-id="7d16f-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="7d16f-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="7d16f-155">deviceIMEI</span></span>|<span data-ttu-id="7d16f-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d16f-156">String</span></span>|<span data-ttu-id="7d16f-157">IMEI des Geräts.</span><span class="sxs-lookup"><span data-stu-id="7d16f-157">IMEI of the device.</span></span>|
|<span data-ttu-id="7d16f-158">actionState</span><span class="sxs-lookup"><span data-stu-id="7d16f-158">actionState</span></span>|[<span data-ttu-id="7d16f-159">actionState</span><span class="sxs-lookup"><span data-stu-id="7d16f-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7d16f-160">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="7d16f-160">Action state.</span></span> <span data-ttu-id="7d16f-161">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7d16f-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d16f-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d16f-162">Response</span></span>
<span data-ttu-id="7d16f-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7d16f-163">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d16f-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d16f-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d16f-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d16f-165">Request</span></span>
<span data-ttu-id="7d16f-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d16f-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 399

{
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

### <a name="response"></a><span data-ttu-id="7d16f-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d16f-167">Response</span></span>
<span data-ttu-id="7d16f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d16f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





