---
title: assignResourceAccountToDevice-Aktion
description: Weist den Autopilot-Geräten ein Ressourcenkonto zu.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e46f12d33e26f15a87746720bfd1b418d4f21878
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631566"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="b38d2-103">assignResourceAccountToDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="b38d2-103">assignResourceAccountToDevice action</span></span>

> <span data-ttu-id="b38d2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b38d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b38d2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b38d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b38d2-106">Weist den Autopilot-Geräten ein Ressourcenkonto zu.</span><span class="sxs-lookup"><span data-stu-id="b38d2-106">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b38d2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b38d2-107">Prerequisites</span></span>
<span data-ttu-id="b38d2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b38d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b38d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b38d2-110">Permission type</span></span>|<span data-ttu-id="b38d2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b38d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b38d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b38d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b38d2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b38d2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b38d2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b38d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b38d2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b38d2-115">Not supported.</span></span>|
|<span data-ttu-id="b38d2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b38d2-116">Application</span></span>|<span data-ttu-id="b38d2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b38d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b38d2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b38d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="b38d2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b38d2-119">Request headers</span></span>
|<span data-ttu-id="b38d2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b38d2-120">Header</span></span>|<span data-ttu-id="b38d2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b38d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b38d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b38d2-122">Authorization</span></span>|<span data-ttu-id="b38d2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b38d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b38d2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b38d2-124">Accept</span></span>|<span data-ttu-id="b38d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b38d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b38d2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b38d2-126">Request body</span></span>
<span data-ttu-id="b38d2-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b38d2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b38d2-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b38d2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b38d2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b38d2-129">Property</span></span>|<span data-ttu-id="b38d2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b38d2-130">Type</span></span>|<span data-ttu-id="b38d2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b38d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b38d2-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b38d2-132">userPrincipalName</span></span>|<span data-ttu-id="b38d2-133">String</span><span class="sxs-lookup"><span data-stu-id="b38d2-133">String</span></span>|<span data-ttu-id="b38d2-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b38d2-134">Not yet documented</span></span>|
|<span data-ttu-id="b38d2-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="b38d2-135">addressableUserName</span></span>|<span data-ttu-id="b38d2-136">String</span><span class="sxs-lookup"><span data-stu-id="b38d2-136">String</span></span>|<span data-ttu-id="b38d2-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b38d2-137">Not yet documented</span></span>|
|<span data-ttu-id="b38d2-138">resourceAccountName</span><span class="sxs-lookup"><span data-stu-id="b38d2-138">resourceAccountName</span></span>|<span data-ttu-id="b38d2-139">String</span><span class="sxs-lookup"><span data-stu-id="b38d2-139">String</span></span>|<span data-ttu-id="b38d2-140">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b38d2-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b38d2-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b38d2-141">Response</span></span>
<span data-ttu-id="b38d2-142">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b38d2-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b38d2-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b38d2-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b38d2-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b38d2-144">Request</span></span>
<span data-ttu-id="b38d2-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b38d2-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice

Content-type: application/json
Content-length: 170

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "resourceAccountName": "Resource Account Name value"
}
```

### <a name="response"></a><span data-ttu-id="b38d2-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="b38d2-146">Response</span></span>
<span data-ttu-id="b38d2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b38d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




