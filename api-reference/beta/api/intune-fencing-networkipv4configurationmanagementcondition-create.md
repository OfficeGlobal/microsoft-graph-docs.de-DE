---
title: Erstellen von networkIPv4ConfigurationManagementCondition
description: Erstellen eines neuen networkIPv4ConfigurationManagementCondition-Objekts.
ms.openlocfilehash: f42bd52da9175192a71ed0be2b36f8f656f6a538
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065381"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="f3011-103">Erstellen von networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f3011-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="f3011-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3011-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3011-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3011-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3011-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3011-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3011-107">Erstellen eines neuen [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3011-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3011-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3011-108">Prerequisites</span></span>
<span data-ttu-id="f3011-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3011-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3011-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3011-111">Permission type</span></span>|<span data-ttu-id="f3011-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3011-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3011-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3011-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3011-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3011-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3011-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3011-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3011-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3011-116">Not supported.</span></span>|
|<span data-ttu-id="f3011-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3011-117">Application</span></span>|<span data-ttu-id="f3011-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3011-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3011-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3011-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="f3011-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3011-120">Request headers</span></span>
|<span data-ttu-id="f3011-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3011-121">Header</span></span>|<span data-ttu-id="f3011-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f3011-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3011-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3011-123">Authorization</span></span>|<span data-ttu-id="f3011-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3011-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3011-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3011-125">Accept</span></span>|<span data-ttu-id="f3011-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3011-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3011-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3011-127">Request body</span></span>
<span data-ttu-id="f3011-128">Geben Sie im Textkörper Anforderung für das Objekt networkIPv4ConfigurationManagementCondition eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f3011-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="f3011-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die networkIPv4ConfigurationManagementCondition erstellen.</span><span class="sxs-lookup"><span data-stu-id="f3011-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="f3011-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3011-130">Property</span></span>|<span data-ttu-id="f3011-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f3011-131">Type</span></span>|<span data-ttu-id="f3011-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3011-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3011-133">id</span><span class="sxs-lookup"><span data-stu-id="f3011-133">id</span></span>|<span data-ttu-id="f3011-134">String</span><span class="sxs-lookup"><span data-stu-id="f3011-134">String</span></span>|<span data-ttu-id="f3011-135">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f3011-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="f3011-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f3011-136">System generated value assigned when created.</span></span> <span data-ttu-id="f3011-137">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f3011-138">uniqueName</span></span>|<span data-ttu-id="f3011-139">String</span><span class="sxs-lookup"><span data-stu-id="f3011-139">String</span></span>|<span data-ttu-id="f3011-140">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f3011-140">Unique name for the management condition.</span></span> <span data-ttu-id="f3011-141">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3011-141">Used in management condition expressions.</span></span> <span data-ttu-id="f3011-142">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f3011-143">displayName</span></span>|<span data-ttu-id="f3011-144">String</span><span class="sxs-lookup"><span data-stu-id="f3011-144">String</span></span>|<span data-ttu-id="f3011-145">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f3011-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="f3011-146">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-147">description</span><span class="sxs-lookup"><span data-stu-id="f3011-147">description</span></span>|<span data-ttu-id="f3011-148">String</span><span class="sxs-lookup"><span data-stu-id="f3011-148">String</span></span>|<span data-ttu-id="f3011-149">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f3011-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="f3011-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3011-151">createdDateTime</span></span>|<span data-ttu-id="f3011-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3011-152">DateTimeOffset</span></span>|<span data-ttu-id="f3011-153">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f3011-153">The time the management condition was created.</span></span> <span data-ttu-id="f3011-154">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="f3011-154">Generated service side.</span></span> <span data-ttu-id="f3011-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3011-156">modifiedDateTime</span></span>|<span data-ttu-id="f3011-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3011-157">DateTimeOffset</span></span>|<span data-ttu-id="f3011-158">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f3011-158">The time the management condition was last modified.</span></span> <span data-ttu-id="f3011-159">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="f3011-159">Updated service side.</span></span> <span data-ttu-id="f3011-160">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-161">eTag</span><span class="sxs-lookup"><span data-stu-id="f3011-161">eTag</span></span>|<span data-ttu-id="f3011-162">String</span><span class="sxs-lookup"><span data-stu-id="f3011-162">String</span></span>|<span data-ttu-id="f3011-163">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f3011-163">ETag of the management condition.</span></span> <span data-ttu-id="f3011-164">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="f3011-164">Updated service side.</span></span> <span data-ttu-id="f3011-165">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f3011-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3011-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f3011-166">applicablePlatforms</span></span>|<span data-ttu-id="f3011-167">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f3011-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f3011-168">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f3011-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f3011-169">Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f3011-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="f3011-170">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="f3011-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="f3011-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="f3011-171">ipV4Prefix</span></span>|<span data-ttu-id="f3011-172">String</span><span class="sxs-lookup"><span data-stu-id="f3011-172">String</span></span>|<span data-ttu-id="f3011-173">Das IPv4-Subnetz mit verbunden sein.</span><span class="sxs-lookup"><span data-stu-id="f3011-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="f3011-174">Diese Vorgaben unter 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="f3011-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="f3011-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="f3011-175">ipV4Gateway</span></span>|<span data-ttu-id="f3011-176">String</span><span class="sxs-lookup"><span data-stu-id="f3011-176">String</span></span>|<span data-ttu-id="f3011-177">Das Gateway IPv4-Adresse.</span><span class="sxs-lookup"><span data-stu-id="f3011-177">The IPv4 gateway address.</span></span> <span data-ttu-id="f3011-178">z. B. 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="f3011-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="f3011-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="f3011-179">ipV4DHCPServer</span></span>|<span data-ttu-id="f3011-180">String</span><span class="sxs-lookup"><span data-stu-id="f3011-180">String</span></span>|<span data-ttu-id="f3011-181">Die IPv4-Adresse des DHCP-Servers für den Adapter.</span><span class="sxs-lookup"><span data-stu-id="f3011-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="f3011-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="f3011-182">ipV4DNSServerList</span></span>|<span data-ttu-id="f3011-183">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3011-183">String collection</span></span>|<span data-ttu-id="f3011-184">Die IPv4-DNS-Server für den Adapter konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="f3011-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="f3011-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="f3011-185">dnsSuffixList</span></span>|<span data-ttu-id="f3011-186">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3011-186">String collection</span></span>|<span data-ttu-id="f3011-187">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="f3011-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="f3011-188">Diese Vorgaben unter seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="f3011-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="f3011-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3011-189">Response</span></span>
<span data-ttu-id="f3011-190">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f3011-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3011-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3011-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3011-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3011-192">Request</span></span>
<span data-ttu-id="f3011-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3011-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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

### <a name="response"></a><span data-ttu-id="f3011-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3011-194">Response</span></span>
<span data-ttu-id="f3011-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3011-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





