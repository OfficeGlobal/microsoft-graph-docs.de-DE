---
title: RemoteActionAudits aufListen
description: AufListen von Eigenschaften und Beziehungen der Remote Action Audit-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b70d7f7a2434078a36b639c4afab02ac204cb59
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989400"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="6f53a-103">RemoteActionAudits aufListen</span><span class="sxs-lookup"><span data-stu-id="6f53a-103">List remoteActionAudits</span></span>

> <span data-ttu-id="6f53a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f53a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f53a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6f53a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f53a-106">AufListen von Eigenschaften und Beziehungen der [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6f53a-106">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f53a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f53a-107">Prerequisites</span></span>
<span data-ttu-id="6f53a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f53a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f53a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f53a-110">Permission type</span></span>|<span data-ttu-id="6f53a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f53a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f53a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f53a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f53a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f53a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6f53a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f53a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f53a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f53a-115">Not supported.</span></span>|
|<span data-ttu-id="6f53a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f53a-116">Application</span></span>|<span data-ttu-id="6f53a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f53a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f53a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f53a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="6f53a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f53a-119">Request headers</span></span>
|<span data-ttu-id="6f53a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f53a-120">Header</span></span>|<span data-ttu-id="6f53a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6f53a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f53a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f53a-122">Authorization</span></span>|<span data-ttu-id="6f53a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f53a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f53a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f53a-124">Accept</span></span>|<span data-ttu-id="6f53a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f53a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f53a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f53a-126">Request body</span></span>
<span data-ttu-id="6f53a-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6f53a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f53a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f53a-128">Response</span></span>
<span data-ttu-id="6f53a-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6f53a-129">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f53a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f53a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f53a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f53a-131">Request</span></span>
<span data-ttu-id="6f53a-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f53a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="6f53a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f53a-133">Response</span></span>
<span data-ttu-id="6f53a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f53a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
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
  ]
}
```




