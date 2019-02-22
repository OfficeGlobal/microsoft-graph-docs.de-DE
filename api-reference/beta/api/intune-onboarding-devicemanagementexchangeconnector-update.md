---
title: deviceManagementExchangeConnector aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d8979bf3455c52e52eac735c025dbd45ac38382
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169244"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="05fc2-103">deviceManagementExchangeConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="05fc2-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="05fc2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="05fc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05fc2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="05fc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05fc2-106">Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="05fc2-106">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05fc2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="05fc2-107">Prerequisites</span></span>
<span data-ttu-id="05fc2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="05fc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05fc2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="05fc2-110">Permission type</span></span>|<span data-ttu-id="05fc2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="05fc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05fc2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="05fc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05fc2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05fc2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05fc2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="05fc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05fc2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05fc2-115">Not supported.</span></span>|
|<span data-ttu-id="05fc2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="05fc2-116">Application</span></span>|<span data-ttu-id="05fc2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05fc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05fc2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="05fc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="05fc2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="05fc2-119">Request headers</span></span>
|<span data-ttu-id="05fc2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="05fc2-120">Header</span></span>|<span data-ttu-id="05fc2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="05fc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05fc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05fc2-122">Authorization</span></span>|<span data-ttu-id="05fc2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="05fc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05fc2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="05fc2-124">Accept</span></span>|<span data-ttu-id="05fc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05fc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05fc2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="05fc2-126">Request body</span></span>
<span data-ttu-id="05fc2-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="05fc2-127">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="05fc2-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="05fc2-128">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="05fc2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05fc2-129">Property</span></span>|<span data-ttu-id="05fc2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="05fc2-130">Type</span></span>|<span data-ttu-id="05fc2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05fc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05fc2-132">id</span><span class="sxs-lookup"><span data-stu-id="05fc2-132">id</span></span>|<span data-ttu-id="05fc2-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="05fc2-133">String</span></span>|<span data-ttu-id="05fc2-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="05fc2-134">Not yet documented</span></span>|
|<span data-ttu-id="05fc2-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="05fc2-135">lastSyncDateTime</span></span>|<span data-ttu-id="05fc2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05fc2-136">DateTimeOffset</span></span>|<span data-ttu-id="05fc2-137">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="05fc2-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="05fc2-138">status</span><span class="sxs-lookup"><span data-stu-id="05fc2-138">status</span></span>|[<span data-ttu-id="05fc2-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="05fc2-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="05fc2-140">Exchange Connector-Status.</span><span class="sxs-lookup"><span data-stu-id="05fc2-140">Exchange Connector Status.</span></span> <span data-ttu-id="05fc2-141">Mögliche Werte: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="05fc2-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="05fc2-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="05fc2-142">primarySmtpAddress</span></span>|<span data-ttu-id="05fc2-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="05fc2-143">String</span></span>|<span data-ttu-id="05fc2-144">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="05fc2-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="05fc2-145">serverName</span><span class="sxs-lookup"><span data-stu-id="05fc2-145">serverName</span></span>|<span data-ttu-id="05fc2-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="05fc2-146">String</span></span>|<span data-ttu-id="05fc2-147">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="05fc2-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="05fc2-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="05fc2-148">connectorServerName</span></span>|<span data-ttu-id="05fc2-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="05fc2-149">String</span></span>|<span data-ttu-id="05fc2-150">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="05fc2-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="05fc2-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="05fc2-151">exchangeConnectorType</span></span>|[<span data-ttu-id="05fc2-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="05fc2-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="05fc2-153">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="05fc2-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="05fc2-154">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="05fc2-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="05fc2-155">Version</span><span class="sxs-lookup"><span data-stu-id="05fc2-155">version</span></span>|<span data-ttu-id="05fc2-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="05fc2-156">String</span></span>|<span data-ttu-id="05fc2-157">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="05fc2-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="05fc2-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="05fc2-158">exchangeAlias</span></span>|<span data-ttu-id="05fc2-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="05fc2-159">String</span></span>|<span data-ttu-id="05fc2-160">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="05fc2-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="05fc2-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="05fc2-161">exchangeOrganization</span></span>|<span data-ttu-id="05fc2-162">String</span><span class="sxs-lookup"><span data-stu-id="05fc2-162">String</span></span>|<span data-ttu-id="05fc2-163">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="05fc2-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="05fc2-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="05fc2-164">Response</span></span>
<span data-ttu-id="05fc2-165">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="05fc2-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05fc2-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="05fc2-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="05fc2-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="05fc2-167">Request</span></span>
<span data-ttu-id="05fc2-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="05fc2-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="05fc2-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="05fc2-169">Response</span></span>
<span data-ttu-id="05fc2-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05fc2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```




