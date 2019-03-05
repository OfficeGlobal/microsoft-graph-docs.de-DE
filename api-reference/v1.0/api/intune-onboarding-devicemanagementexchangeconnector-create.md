---
title: deviceManagementExchangeConnector erstellen
description: Erstellen eines neuen deviceManagementExchangeConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 292562a2a7083e63f083d0ccad5e11071a27ce96
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256441"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="de142-103">deviceManagementExchangeConnector erstellen</span><span class="sxs-lookup"><span data-stu-id="de142-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="de142-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="de142-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de142-105">Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="de142-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de142-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="de142-106">Prerequisites</span></span>
<span data-ttu-id="de142-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="de142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="de142-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de142-109">Permission type</span></span>|<span data-ttu-id="de142-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de142-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de142-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de142-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de142-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de142-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de142-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de142-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de142-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de142-114">Not supported.</span></span>|
|<span data-ttu-id="de142-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de142-115">Application</span></span>|<span data-ttu-id="de142-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de142-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de142-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de142-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="de142-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de142-118">Request headers</span></span>
|<span data-ttu-id="de142-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="de142-119">Header</span></span>|<span data-ttu-id="de142-120">Wert</span><span class="sxs-lookup"><span data-stu-id="de142-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de142-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de142-121">Authorization</span></span>|<span data-ttu-id="de142-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="de142-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de142-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="de142-123">Accept</span></span>|<span data-ttu-id="de142-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de142-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de142-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de142-125">Request body</span></span>
<span data-ttu-id="de142-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementExchangeConnector an.</span><span class="sxs-lookup"><span data-stu-id="de142-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="de142-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementExchangeConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="de142-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="de142-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de142-128">Property</span></span>|<span data-ttu-id="de142-129">Typ</span><span class="sxs-lookup"><span data-stu-id="de142-129">Type</span></span>|<span data-ttu-id="de142-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de142-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de142-131">id</span><span class="sxs-lookup"><span data-stu-id="de142-131">id</span></span>|<span data-ttu-id="de142-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de142-132">String</span></span>|<span data-ttu-id="de142-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="de142-133">Not yet documented</span></span>|
|<span data-ttu-id="de142-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="de142-134">lastSyncDateTime</span></span>|<span data-ttu-id="de142-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de142-135">DateTimeOffset</span></span>|<span data-ttu-id="de142-136">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="de142-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="de142-137">status</span><span class="sxs-lookup"><span data-stu-id="de142-137">status</span></span>|[<span data-ttu-id="de142-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="de142-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="de142-139">Exchange Connector-Status.</span><span class="sxs-lookup"><span data-stu-id="de142-139">Exchange Connector Status.</span></span> <span data-ttu-id="de142-140">Mögliche Werte: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="de142-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="de142-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="de142-141">primarySmtpAddress</span></span>|<span data-ttu-id="de142-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de142-142">String</span></span>|<span data-ttu-id="de142-143">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="de142-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="de142-144">serverName</span><span class="sxs-lookup"><span data-stu-id="de142-144">serverName</span></span>|<span data-ttu-id="de142-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de142-145">String</span></span>|<span data-ttu-id="de142-146">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="de142-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="de142-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="de142-147">connectorServerName</span></span>|<span data-ttu-id="de142-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de142-148">String</span></span>|<span data-ttu-id="de142-149">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="de142-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="de142-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="de142-150">exchangeConnectorType</span></span>|[<span data-ttu-id="de142-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="de142-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="de142-152">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="de142-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="de142-153">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="de142-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="de142-154">Version</span><span class="sxs-lookup"><span data-stu-id="de142-154">version</span></span>|<span data-ttu-id="de142-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de142-155">String</span></span>|<span data-ttu-id="de142-156">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="de142-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="de142-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="de142-157">exchangeAlias</span></span>|<span data-ttu-id="de142-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de142-158">String</span></span>|<span data-ttu-id="de142-159">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="de142-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="de142-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="de142-160">exchangeOrganization</span></span>|<span data-ttu-id="de142-161">String</span><span class="sxs-lookup"><span data-stu-id="de142-161">String</span></span>|<span data-ttu-id="de142-162">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="de142-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="de142-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="de142-163">Response</span></span>
<span data-ttu-id="de142-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="de142-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de142-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de142-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="de142-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de142-166">Request</span></span>
<span data-ttu-id="de142-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de142-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="de142-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="de142-168">Response</span></span>
<span data-ttu-id="de142-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de142-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



