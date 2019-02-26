---
title: NetworkIPv4ConfigurationManagementCondition aktualisieren
description: Aktualisieren der Eigenschaften eines networkIPv4ConfigurationManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 455f0631331f67c161b543cd85dc30c97d75ac1a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149434"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="b3fd1-103">NetworkIPv4ConfigurationManagementCondition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b3fd1-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="b3fd1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3fd1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3fd1-106">Aktualisieren der Eigenschaften eines [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-106">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3fd1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3fd1-107">Prerequisites</span></span>
<span data-ttu-id="b3fd1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3fd1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3fd1-110">Permission type</span></span>|<span data-ttu-id="b3fd1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3fd1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3fd1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3fd1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3fd1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3fd1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3fd1-115">Not supported.</span></span>|
|<span data-ttu-id="b3fd1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3fd1-116">Application</span></span>|<span data-ttu-id="b3fd1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3fd1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3fd1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3fd1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="b3fd1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3fd1-119">Request headers</span></span>
|<span data-ttu-id="b3fd1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b3fd1-120">Header</span></span>|<span data-ttu-id="b3fd1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b3fd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3fd1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3fd1-122">Authorization</span></span>|<span data-ttu-id="b3fd1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3fd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3fd1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b3fd1-124">Accept</span></span>|<span data-ttu-id="b3fd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3fd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3fd1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3fd1-126">Request body</span></span>
<span data-ttu-id="b3fd1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-127">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="b3fd1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-128">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="b3fd1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3fd1-129">Property</span></span>|<span data-ttu-id="b3fd1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b3fd1-130">Type</span></span>|<span data-ttu-id="b3fd1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3fd1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3fd1-132">id</span><span class="sxs-lookup"><span data-stu-id="b3fd1-132">id</span></span>|<span data-ttu-id="b3fd1-133">string</span><span class="sxs-lookup"><span data-stu-id="b3fd1-133">String</span></span>|<span data-ttu-id="b3fd1-134">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="b3fd1-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-135">System generated value assigned when created.</span></span> <span data-ttu-id="b3fd1-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="b3fd1-137">uniqueName</span></span>|<span data-ttu-id="b3fd1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-138">String</span></span>|<span data-ttu-id="b3fd1-139">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-139">Unique name for the management condition.</span></span> <span data-ttu-id="b3fd1-140">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-140">Used in management condition expressions.</span></span> <span data-ttu-id="b3fd1-141">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b3fd1-142">displayName</span></span>|<span data-ttu-id="b3fd1-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-143">String</span></span>|<span data-ttu-id="b3fd1-144">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="b3fd1-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-146">description</span><span class="sxs-lookup"><span data-stu-id="b3fd1-146">description</span></span>|<span data-ttu-id="b3fd1-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-147">String</span></span>|<span data-ttu-id="b3fd1-148">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="b3fd1-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fd1-150">createdDateTime</span></span>|<span data-ttu-id="b3fd1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fd1-151">DateTimeOffset</span></span>|<span data-ttu-id="b3fd1-152">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-152">The time the management condition was created.</span></span> <span data-ttu-id="b3fd1-153">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-153">Generated service side.</span></span> <span data-ttu-id="b3fd1-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fd1-155">modifiedDateTime</span></span>|<span data-ttu-id="b3fd1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fd1-156">DateTimeOffset</span></span>|<span data-ttu-id="b3fd1-157">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-157">The time the management condition was last modified.</span></span> <span data-ttu-id="b3fd1-158">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-158">Updated service side.</span></span> <span data-ttu-id="b3fd1-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-160">eTag</span><span class="sxs-lookup"><span data-stu-id="b3fd1-160">eTag</span></span>|<span data-ttu-id="b3fd1-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-161">String</span></span>|<span data-ttu-id="b3fd1-162">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-162">ETag of the management condition.</span></span> <span data-ttu-id="b3fd1-163">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-163">Updated service side.</span></span> <span data-ttu-id="b3fd1-164">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd1-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b3fd1-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b3fd1-165">applicablePlatforms</span></span>|<span data-ttu-id="b3fd1-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b3fd1-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b3fd1-167">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b3fd1-168">Von [ManagementCondition](../resources/intune-fencing-managementcondition.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="b3fd1-169">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="b3fd1-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="b3fd1-170">ipV4Prefix</span></span>|<span data-ttu-id="b3fd1-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-171">String</span></span>|<span data-ttu-id="b3fd1-172">Das IPv4-Subnetz, mit dem eine Verbindung hergestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="b3fd1-173">z.b. 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="b3fd1-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="b3fd1-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="b3fd1-174">ipV4Gateway</span></span>|<span data-ttu-id="b3fd1-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-175">String</span></span>|<span data-ttu-id="b3fd1-176">Die Adresse des IPv4-Gateways.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-176">The IPv4 gateway address.</span></span> <span data-ttu-id="b3fd1-177">beispielsweise 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="b3fd1-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="b3fd1-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="b3fd1-178">ipV4DHCPServer</span></span>|<span data-ttu-id="b3fd1-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3fd1-179">String</span></span>|<span data-ttu-id="b3fd1-180">Die IPv4-Adresse des DHCP-Servers für den Adapter.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="b3fd1-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="b3fd1-181">ipV4DNSServerList</span></span>|<span data-ttu-id="b3fd1-182">String collection</span><span class="sxs-lookup"><span data-stu-id="b3fd1-182">String collection</span></span>|<span data-ttu-id="b3fd1-183">Die für den Adapter konfigurierten IPv4-DNS-Server.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="b3fd1-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="b3fd1-184">dnsSuffixList</span></span>|<span data-ttu-id="b3fd1-185">String collection</span><span class="sxs-lookup"><span data-stu-id="b3fd1-185">String collection</span></span>|<span data-ttu-id="b3fd1-186">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="b3fd1-187">beispielsweise Seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="b3fd1-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="b3fd1-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3fd1-188">Response</span></span>
<span data-ttu-id="b3fd1-189">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-189">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3fd1-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3fd1-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3fd1-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3fd1-191">Request</span></span>
<span data-ttu-id="b3fd1-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b3fd1-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3fd1-193">Response</span></span>
<span data-ttu-id="b3fd1-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3fd1-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




