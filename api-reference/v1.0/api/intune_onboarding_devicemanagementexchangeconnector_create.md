# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="f2e58-101">deviceManagementExchangeConnector erstellen</span><span class="sxs-lookup"><span data-stu-id="f2e58-101">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="f2e58-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f2e58-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2e58-103">Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f2e58-103">Create a new [plannerBucket](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2e58-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f2e58-104">Prerequisites</span></span>
<span data-ttu-id="f2e58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2e58-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2e58-107">Permission type</span></span>|<span data-ttu-id="f2e58-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2e58-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e58-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2e58-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f2e58-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e58-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f2e58-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2e58-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e58-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2e58-112">Not supported.</span></span>|
|<span data-ttu-id="f2e58-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2e58-113">Application</span></span>|<span data-ttu-id="f2e58-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2e58-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e58-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e58-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f2e58-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2e58-116">Request headers</span></span>
|<span data-ttu-id="f2e58-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2e58-117">Header</span></span>|<span data-ttu-id="f2e58-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f2e58-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e58-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e58-119">Authorization</span></span>|<span data-ttu-id="f2e58-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f2e58-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f2e58-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f2e58-121">Accept</span></span>|<span data-ttu-id="f2e58-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e58-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e58-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2e58-123">Request body</span></span>
<span data-ttu-id="f2e58-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementExchangeConnector an.</span><span class="sxs-lookup"><span data-stu-id="f2e58-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f2e58-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementExchangeConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="f2e58-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="f2e58-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2e58-126">Property</span></span>|<span data-ttu-id="f2e58-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f2e58-127">Type</span></span>|<span data-ttu-id="f2e58-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e58-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e58-129">id</span><span class="sxs-lookup"><span data-stu-id="f2e58-129">id</span></span>|<span data-ttu-id="f2e58-130">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-130">String</span></span>|<span data-ttu-id="f2e58-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f2e58-131">Not yet documented</span></span>|
|<span data-ttu-id="f2e58-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e58-132">lastSyncDateTime</span></span>|<span data-ttu-id="f2e58-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e58-133">DateTimeOffset</span></span>|<span data-ttu-id="f2e58-134">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="f2e58-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="f2e58-135">status</span><span class="sxs-lookup"><span data-stu-id="f2e58-135">status</span></span>|<span data-ttu-id="f2e58-136">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-136">String</span></span>|<span data-ttu-id="f2e58-137">Status von Exchange Connector. Mögliche Werte: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="f2e58-137">Exchange Connector Status Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="f2e58-138">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f2e58-138">primarySmtpAddress</span></span>|<span data-ttu-id="f2e58-139">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-139">String</span></span>|<span data-ttu-id="f2e58-140">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f2e58-140">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="f2e58-141">serverName</span><span class="sxs-lookup"><span data-stu-id="f2e58-141">servername</span></span>|<span data-ttu-id="f2e58-142">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-142">String</span></span>|<span data-ttu-id="f2e58-143">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="f2e58-143">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="f2e58-144">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="f2e58-144">exchangeConnectorType</span></span>|<span data-ttu-id="f2e58-145">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-145">String</span></span>|<span data-ttu-id="f2e58-146">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="f2e58-146">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="f2e58-147">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="f2e58-147">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="f2e58-148">Version</span><span class="sxs-lookup"><span data-stu-id="f2e58-148">version</span></span>|<span data-ttu-id="f2e58-149">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-149">String</span></span>|<span data-ttu-id="f2e58-150">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="f2e58-150">The version of the message.</span></span>|
|<span data-ttu-id="f2e58-151">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="f2e58-151">exchangeAlias</span></span>|<span data-ttu-id="f2e58-152">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-152">String</span></span>|<span data-ttu-id="f2e58-153">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="f2e58-153">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="f2e58-154">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="f2e58-154">exchangeOrganization</span></span>|<span data-ttu-id="f2e58-155">String</span><span class="sxs-lookup"><span data-stu-id="f2e58-155">String</span></span>|<span data-ttu-id="f2e58-156">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="f2e58-156">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="f2e58-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e58-157">Response</span></span>
<span data-ttu-id="f2e58-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f2e58-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e58-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2e58-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2e58-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e58-160">Request</span></span>
<span data-ttu-id="f2e58-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2e58-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 433

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="f2e58-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e58-162">Response</span></span>
<span data-ttu-id="f2e58-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2e58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 482

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



