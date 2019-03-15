---
title: unassignResourceAccountFromDevice-Aktion
description: Aufheben der Zuweisung des Ressourcenkontos von einem Autopilot-Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ada22dab5e17d64315496ee9e0d7da25a5223740
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631554"
---
# <a name="unassignresourceaccountfromdevice-action"></a><span data-ttu-id="78a3b-103">unassignResourceAccountFromDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="78a3b-103">unassignResourceAccountFromDevice action</span></span>

> <span data-ttu-id="78a3b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78a3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78a3b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="78a3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78a3b-106">Aufheben der Zuweisung des Ressourcenkontos von einem Autopilot-Gerät.</span><span class="sxs-lookup"><span data-stu-id="78a3b-106">Unassigns the resource account from an Autopilot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78a3b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="78a3b-107">Prerequisites</span></span>
<span data-ttu-id="78a3b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="78a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="78a3b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78a3b-110">Permission type</span></span>|<span data-ttu-id="78a3b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78a3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78a3b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78a3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78a3b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78a3b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="78a3b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78a3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78a3b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78a3b-115">Not supported.</span></span>|
|<span data-ttu-id="78a3b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78a3b-116">Application</span></span>|<span data-ttu-id="78a3b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78a3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78a3b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78a3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="78a3b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78a3b-119">Request headers</span></span>
|<span data-ttu-id="78a3b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="78a3b-120">Header</span></span>|<span data-ttu-id="78a3b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="78a3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78a3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78a3b-122">Authorization</span></span>|<span data-ttu-id="78a3b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="78a3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78a3b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="78a3b-124">Accept</span></span>|<span data-ttu-id="78a3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78a3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78a3b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78a3b-126">Request body</span></span>
<span data-ttu-id="78a3b-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="78a3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78a3b-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="78a3b-128">Response</span></span>
<span data-ttu-id="78a3b-129">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78a3b-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="78a3b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78a3b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="78a3b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78a3b-131">Request</span></span>
<span data-ttu-id="78a3b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="78a3b-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

### <a name="response"></a><span data-ttu-id="78a3b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="78a3b-133">Response</span></span>
<span data-ttu-id="78a3b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78a3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




