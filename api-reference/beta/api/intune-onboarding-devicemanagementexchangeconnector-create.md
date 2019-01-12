---
title: deviceManagementExchangeConnector erstellen
description: Erstellen eines neuen deviceManagementExchangeConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72552f83ad36c5be2302180c7e57ef8bbadfa887
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963570"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="506fc-103">deviceManagementExchangeConnector erstellen</span><span class="sxs-lookup"><span data-stu-id="506fc-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="506fc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="506fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="506fc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="506fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="506fc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="506fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="506fc-107">Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="506fc-107">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="506fc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="506fc-108">Prerequisites</span></span>
<span data-ttu-id="506fc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="506fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="506fc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="506fc-111">Permission type</span></span>|<span data-ttu-id="506fc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="506fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="506fc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="506fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="506fc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="506fc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="506fc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="506fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="506fc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="506fc-116">Not supported.</span></span>|
|<span data-ttu-id="506fc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="506fc-117">Application</span></span>|<span data-ttu-id="506fc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="506fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="506fc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="506fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="506fc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="506fc-120">Request headers</span></span>
|<span data-ttu-id="506fc-121">Header</span><span class="sxs-lookup"><span data-stu-id="506fc-121">Header</span></span>|<span data-ttu-id="506fc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="506fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="506fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="506fc-123">Authorization</span></span>|<span data-ttu-id="506fc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="506fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="506fc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="506fc-125">Accept</span></span>|<span data-ttu-id="506fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="506fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="506fc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="506fc-127">Request body</span></span>
<span data-ttu-id="506fc-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementExchangeConnector an.</span><span class="sxs-lookup"><span data-stu-id="506fc-128">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="506fc-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementExchangeConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="506fc-129">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="506fc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="506fc-130">Property</span></span>|<span data-ttu-id="506fc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="506fc-131">Type</span></span>|<span data-ttu-id="506fc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="506fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="506fc-133">id</span><span class="sxs-lookup"><span data-stu-id="506fc-133">id</span></span>|<span data-ttu-id="506fc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="506fc-134">String</span></span>|<span data-ttu-id="506fc-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="506fc-135">Not yet documented</span></span>|
|<span data-ttu-id="506fc-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="506fc-136">lastSyncDateTime</span></span>|<span data-ttu-id="506fc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="506fc-137">DateTimeOffset</span></span>|<span data-ttu-id="506fc-138">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="506fc-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="506fc-139">status</span><span class="sxs-lookup"><span data-stu-id="506fc-139">status</span></span>|[<span data-ttu-id="506fc-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="506fc-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="506fc-141">Exchange Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="506fc-141">Exchange Connector Status.</span></span> <span data-ttu-id="506fc-142">Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="506fc-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="506fc-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="506fc-143">primarySmtpAddress</span></span>|<span data-ttu-id="506fc-144">String</span><span class="sxs-lookup"><span data-stu-id="506fc-144">String</span></span>|<span data-ttu-id="506fc-145">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="506fc-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="506fc-146">serverName</span><span class="sxs-lookup"><span data-stu-id="506fc-146">serverName</span></span>|<span data-ttu-id="506fc-147">String</span><span class="sxs-lookup"><span data-stu-id="506fc-147">String</span></span>|<span data-ttu-id="506fc-148">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="506fc-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="506fc-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="506fc-149">connectorServerName</span></span>|<span data-ttu-id="506fc-150">String</span><span class="sxs-lookup"><span data-stu-id="506fc-150">String</span></span>|<span data-ttu-id="506fc-151">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="506fc-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="506fc-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="506fc-152">exchangeConnectorType</span></span>|[<span data-ttu-id="506fc-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="506fc-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="506fc-154">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="506fc-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="506fc-155">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="506fc-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="506fc-156">Version</span><span class="sxs-lookup"><span data-stu-id="506fc-156">version</span></span>|<span data-ttu-id="506fc-157">String</span><span class="sxs-lookup"><span data-stu-id="506fc-157">String</span></span>|<span data-ttu-id="506fc-158">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="506fc-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="506fc-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="506fc-159">exchangeAlias</span></span>|<span data-ttu-id="506fc-160">String</span><span class="sxs-lookup"><span data-stu-id="506fc-160">String</span></span>|<span data-ttu-id="506fc-161">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="506fc-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="506fc-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="506fc-162">exchangeOrganization</span></span>|<span data-ttu-id="506fc-163">String</span><span class="sxs-lookup"><span data-stu-id="506fc-163">String</span></span>|<span data-ttu-id="506fc-164">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="506fc-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="506fc-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="506fc-165">Response</span></span>
<span data-ttu-id="506fc-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="506fc-166">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="506fc-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="506fc-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="506fc-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="506fc-168">Request</span></span>
<span data-ttu-id="506fc-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="506fc-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="506fc-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="506fc-170">Response</span></span>
<span data-ttu-id="506fc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="506fc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





