---
title: Erstellen von remoteActionAudit
description: Erstellen eines neuen RemoteActionAudit-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 47ba3de19ca5cdc9b01bb3b65eb8b04e75831d87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396882"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="279d9-103">Erstellen von remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="279d9-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="279d9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="279d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="279d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="279d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="279d9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="279d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="279d9-107">Erstellen eines neuen [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="279d9-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="279d9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="279d9-108">Prerequisites</span></span>
<span data-ttu-id="279d9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="279d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="279d9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="279d9-111">Permission type</span></span>|<span data-ttu-id="279d9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="279d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="279d9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="279d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="279d9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279d9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="279d9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="279d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="279d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="279d9-116">Not supported.</span></span>|
|<span data-ttu-id="279d9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="279d9-117">Application</span></span>|<span data-ttu-id="279d9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="279d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="279d9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="279d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="279d9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="279d9-120">Request headers</span></span>
|<span data-ttu-id="279d9-121">Header</span><span class="sxs-lookup"><span data-stu-id="279d9-121">Header</span></span>|<span data-ttu-id="279d9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="279d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="279d9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="279d9-123">Authorization</span></span>|<span data-ttu-id="279d9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="279d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="279d9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="279d9-125">Accept</span></span>|<span data-ttu-id="279d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="279d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="279d9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="279d9-127">Request body</span></span>
<span data-ttu-id="279d9-128">Geben Sie im Textkörper Anforderung für das Objekt RemoteActionAudit eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="279d9-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="279d9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die RemoteActionAudit erstellen.</span><span class="sxs-lookup"><span data-stu-id="279d9-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="279d9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="279d9-130">Property</span></span>|<span data-ttu-id="279d9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="279d9-131">Type</span></span>|<span data-ttu-id="279d9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="279d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="279d9-133">id</span><span class="sxs-lookup"><span data-stu-id="279d9-133">id</span></span>|<span data-ttu-id="279d9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279d9-134">String</span></span>|<span data-ttu-id="279d9-135">Berichts-ID</span><span class="sxs-lookup"><span data-stu-id="279d9-135">Report Id.</span></span>|
|<span data-ttu-id="279d9-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="279d9-136">deviceDisplayName</span></span>|<span data-ttu-id="279d9-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279d9-137">String</span></span>|<span data-ttu-id="279d9-138">Name des Aufnahmegeräts Intune.</span><span class="sxs-lookup"><span data-stu-id="279d9-138">Intune device name.</span></span>|
|<span data-ttu-id="279d9-139">userName</span><span class="sxs-lookup"><span data-stu-id="279d9-139">userName</span></span>|<span data-ttu-id="279d9-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279d9-140">String</span></span>|<span data-ttu-id="279d9-141">\[veraltete\] verwenden Sie stattdessen InitiatedByUserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="279d9-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="279d9-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="279d9-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="279d9-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279d9-143">String</span></span>|<span data-ttu-id="279d9-144">Benutzer, der die Aktion Gerät gestartet UPN-Format vorliegt.</span><span class="sxs-lookup"><span data-stu-id="279d9-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="279d9-145">Aktion</span><span class="sxs-lookup"><span data-stu-id="279d9-145">action</span></span>|[<span data-ttu-id="279d9-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="279d9-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="279d9-147">Der Name der Aktion.</span><span class="sxs-lookup"><span data-stu-id="279d9-147">The action name.</span></span> <span data-ttu-id="279d9-148">Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="279d9-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="279d9-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="279d9-149">requestDateTime</span></span>|<span data-ttu-id="279d9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="279d9-150">DateTimeOffset</span></span>|<span data-ttu-id="279d9-151">Zeit, wenn die Aktion ausgestellt wurde, in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="279d9-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="279d9-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="279d9-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="279d9-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279d9-153">String</span></span>|<span data-ttu-id="279d9-154">UPN des Besitzers Gerät.</span><span class="sxs-lookup"><span data-stu-id="279d9-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="279d9-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="279d9-155">deviceIMEI</span></span>|<span data-ttu-id="279d9-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279d9-156">String</span></span>|<span data-ttu-id="279d9-157">IMEI des Geräts.</span><span class="sxs-lookup"><span data-stu-id="279d9-157">IMEI of the device.</span></span>|
|<span data-ttu-id="279d9-158">actionState</span><span class="sxs-lookup"><span data-stu-id="279d9-158">actionState</span></span>|[<span data-ttu-id="279d9-159">actionState</span><span class="sxs-lookup"><span data-stu-id="279d9-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="279d9-160">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="279d9-160">Action state.</span></span> <span data-ttu-id="279d9-161">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="279d9-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="279d9-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="279d9-162">Response</span></span>
<span data-ttu-id="279d9-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="279d9-163">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="279d9-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="279d9-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="279d9-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="279d9-165">Request</span></span>
<span data-ttu-id="279d9-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="279d9-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="279d9-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="279d9-167">Response</span></span>
<span data-ttu-id="279d9-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="279d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




