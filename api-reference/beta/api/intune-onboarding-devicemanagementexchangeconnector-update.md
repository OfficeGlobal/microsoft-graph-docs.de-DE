---
title: deviceManagementExchangeConnector aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fad828df8c470e42b8a5ee27b3fa2c950149872c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978150"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="82192-103">deviceManagementExchangeConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="82192-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="82192-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82192-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82192-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="82192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82192-106">Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="82192-106">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82192-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="82192-107">Prerequisites</span></span>
<span data-ttu-id="82192-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82192-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82192-110">Permission type</span></span>|<span data-ttu-id="82192-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82192-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82192-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82192-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82192-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82192-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82192-115">Not supported.</span></span>|
|<span data-ttu-id="82192-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82192-116">Application</span></span>|<span data-ttu-id="82192-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82192-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82192-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="82192-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82192-119">Request headers</span></span>
|<span data-ttu-id="82192-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="82192-120">Header</span></span>|<span data-ttu-id="82192-121">Wert</span><span class="sxs-lookup"><span data-stu-id="82192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82192-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82192-122">Authorization</span></span>|<span data-ttu-id="82192-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="82192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82192-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="82192-124">Accept</span></span>|<span data-ttu-id="82192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82192-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82192-126">Request body</span></span>
<span data-ttu-id="82192-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="82192-127">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="82192-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="82192-128">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="82192-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82192-129">Property</span></span>|<span data-ttu-id="82192-130">Typ</span><span class="sxs-lookup"><span data-stu-id="82192-130">Type</span></span>|<span data-ttu-id="82192-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82192-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82192-132">id</span><span class="sxs-lookup"><span data-stu-id="82192-132">id</span></span>|<span data-ttu-id="82192-133">String</span><span class="sxs-lookup"><span data-stu-id="82192-133">String</span></span>|<span data-ttu-id="82192-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="82192-134">Not yet documented</span></span>|
|<span data-ttu-id="82192-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="82192-135">lastSyncDateTime</span></span>|<span data-ttu-id="82192-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82192-136">DateTimeOffset</span></span>|<span data-ttu-id="82192-137">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="82192-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="82192-138">status</span><span class="sxs-lookup"><span data-stu-id="82192-138">status</span></span>|[<span data-ttu-id="82192-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="82192-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="82192-140">Exchange Connector-Status.</span><span class="sxs-lookup"><span data-stu-id="82192-140">Exchange Connector Status.</span></span> <span data-ttu-id="82192-141">Mögliche Werte sind: `none`, `connectionPending`, `connected` und `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="82192-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="82192-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="82192-142">primarySmtpAddress</span></span>|<span data-ttu-id="82192-143">String</span><span class="sxs-lookup"><span data-stu-id="82192-143">String</span></span>|<span data-ttu-id="82192-144">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="82192-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="82192-145">serverName</span><span class="sxs-lookup"><span data-stu-id="82192-145">serverName</span></span>|<span data-ttu-id="82192-146">String</span><span class="sxs-lookup"><span data-stu-id="82192-146">String</span></span>|<span data-ttu-id="82192-147">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="82192-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="82192-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="82192-148">connectorServerName</span></span>|<span data-ttu-id="82192-149">String</span><span class="sxs-lookup"><span data-stu-id="82192-149">String</span></span>|<span data-ttu-id="82192-150">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="82192-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="82192-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="82192-151">exchangeConnectorType</span></span>|[<span data-ttu-id="82192-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="82192-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="82192-153">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="82192-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="82192-154">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="82192-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="82192-155">Version</span><span class="sxs-lookup"><span data-stu-id="82192-155">version</span></span>|<span data-ttu-id="82192-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82192-156">String</span></span>|<span data-ttu-id="82192-157">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="82192-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="82192-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="82192-158">exchangeAlias</span></span>|<span data-ttu-id="82192-159">String</span><span class="sxs-lookup"><span data-stu-id="82192-159">String</span></span>|<span data-ttu-id="82192-160">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="82192-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="82192-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="82192-161">exchangeOrganization</span></span>|<span data-ttu-id="82192-162">String</span><span class="sxs-lookup"><span data-stu-id="82192-162">String</span></span>|<span data-ttu-id="82192-163">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="82192-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="82192-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="82192-164">Response</span></span>
<span data-ttu-id="82192-165">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="82192-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82192-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82192-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="82192-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82192-167">Request</span></span>
<span data-ttu-id="82192-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82192-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82192-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="82192-169">Response</span></span>
<span data-ttu-id="82192-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82192-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




