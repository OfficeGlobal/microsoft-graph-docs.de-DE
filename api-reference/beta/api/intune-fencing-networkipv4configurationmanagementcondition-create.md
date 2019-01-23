---
title: Erstellen von networkIPv4ConfigurationManagementCondition
description: Erstellen eines neuen networkIPv4ConfigurationManagementCondition-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 385e24e7b20624a82f7744957668d7a36280af11
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394754"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="152f1-103">Erstellen von networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="152f1-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="152f1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="152f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="152f1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="152f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="152f1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="152f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="152f1-107">Erstellen eines neuen [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="152f1-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="152f1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="152f1-108">Prerequisites</span></span>
<span data-ttu-id="152f1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="152f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="152f1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="152f1-111">Permission type</span></span>|<span data-ttu-id="152f1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="152f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="152f1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="152f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="152f1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="152f1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="152f1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="152f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="152f1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="152f1-116">Not supported.</span></span>|
|<span data-ttu-id="152f1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="152f1-117">Application</span></span>|<span data-ttu-id="152f1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="152f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="152f1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="152f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="152f1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="152f1-120">Request headers</span></span>
|<span data-ttu-id="152f1-121">Header</span><span class="sxs-lookup"><span data-stu-id="152f1-121">Header</span></span>|<span data-ttu-id="152f1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="152f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="152f1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="152f1-123">Authorization</span></span>|<span data-ttu-id="152f1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="152f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="152f1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="152f1-125">Accept</span></span>|<span data-ttu-id="152f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="152f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="152f1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="152f1-127">Request body</span></span>
<span data-ttu-id="152f1-128">Geben Sie im Textkörper Anforderung für das Objekt networkIPv4ConfigurationManagementCondition eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="152f1-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="152f1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die networkIPv4ConfigurationManagementCondition erstellen.</span><span class="sxs-lookup"><span data-stu-id="152f1-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="152f1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="152f1-130">Property</span></span>|<span data-ttu-id="152f1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="152f1-131">Type</span></span>|<span data-ttu-id="152f1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="152f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="152f1-133">id</span><span class="sxs-lookup"><span data-stu-id="152f1-133">id</span></span>|<span data-ttu-id="152f1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-134">String</span></span>|<span data-ttu-id="152f1-135">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="152f1-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="152f1-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="152f1-136">System generated value assigned when created.</span></span> <span data-ttu-id="152f1-137">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="152f1-138">uniqueName</span></span>|<span data-ttu-id="152f1-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-139">String</span></span>|<span data-ttu-id="152f1-140">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="152f1-140">Unique name for the management condition.</span></span> <span data-ttu-id="152f1-141">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="152f1-141">Used in management condition expressions.</span></span> <span data-ttu-id="152f1-142">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="152f1-143">displayName</span></span>|<span data-ttu-id="152f1-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-144">String</span></span>|<span data-ttu-id="152f1-145">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="152f1-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="152f1-146">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-147">description</span><span class="sxs-lookup"><span data-stu-id="152f1-147">description</span></span>|<span data-ttu-id="152f1-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-148">String</span></span>|<span data-ttu-id="152f1-149">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="152f1-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="152f1-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="152f1-151">createdDateTime</span></span>|<span data-ttu-id="152f1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="152f1-152">DateTimeOffset</span></span>|<span data-ttu-id="152f1-153">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="152f1-153">The time the management condition was created.</span></span> <span data-ttu-id="152f1-154">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="152f1-154">Generated service side.</span></span> <span data-ttu-id="152f1-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="152f1-156">modifiedDateTime</span></span>|<span data-ttu-id="152f1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="152f1-157">DateTimeOffset</span></span>|<span data-ttu-id="152f1-158">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="152f1-158">The time the management condition was last modified.</span></span> <span data-ttu-id="152f1-159">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="152f1-159">Updated service side.</span></span> <span data-ttu-id="152f1-160">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-161">eTag</span><span class="sxs-lookup"><span data-stu-id="152f1-161">eTag</span></span>|<span data-ttu-id="152f1-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-162">String</span></span>|<span data-ttu-id="152f1-163">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="152f1-163">ETag of the management condition.</span></span> <span data-ttu-id="152f1-164">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="152f1-164">Updated service side.</span></span> <span data-ttu-id="152f1-165">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="152f1-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="152f1-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="152f1-166">applicablePlatforms</span></span>|<span data-ttu-id="152f1-167">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="152f1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="152f1-168">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="152f1-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="152f1-169">Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="152f1-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="152f1-170">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="152f1-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="152f1-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="152f1-171">ipV4Prefix</span></span>|<span data-ttu-id="152f1-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-172">String</span></span>|<span data-ttu-id="152f1-173">Das IPv4-Subnetz mit verbunden sein.</span><span class="sxs-lookup"><span data-stu-id="152f1-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="152f1-174">Diese Vorgaben unter 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="152f1-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="152f1-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="152f1-175">ipV4Gateway</span></span>|<span data-ttu-id="152f1-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-176">String</span></span>|<span data-ttu-id="152f1-177">Das Gateway IPv4-Adresse.</span><span class="sxs-lookup"><span data-stu-id="152f1-177">The IPv4 gateway address.</span></span> <span data-ttu-id="152f1-178">z. B. 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="152f1-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="152f1-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="152f1-179">ipV4DHCPServer</span></span>|<span data-ttu-id="152f1-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152f1-180">String</span></span>|<span data-ttu-id="152f1-181">Die IPv4-Adresse des DHCP-Servers für den Adapter.</span><span class="sxs-lookup"><span data-stu-id="152f1-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="152f1-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="152f1-182">ipV4DNSServerList</span></span>|<span data-ttu-id="152f1-183">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="152f1-183">String collection</span></span>|<span data-ttu-id="152f1-184">Die IPv4-DNS-Server für den Adapter konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="152f1-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="152f1-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="152f1-185">dnsSuffixList</span></span>|<span data-ttu-id="152f1-186">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="152f1-186">String collection</span></span>|<span data-ttu-id="152f1-187">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="152f1-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="152f1-188">Diese Vorgaben unter seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="152f1-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="152f1-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="152f1-189">Response</span></span>
<span data-ttu-id="152f1-190">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="152f1-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="152f1-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="152f1-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="152f1-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="152f1-192">Request</span></span>
<span data-ttu-id="152f1-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="152f1-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="152f1-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="152f1-194">Response</span></span>
<span data-ttu-id="152f1-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="152f1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




