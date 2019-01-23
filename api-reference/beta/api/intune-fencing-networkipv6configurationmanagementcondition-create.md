---
title: Erstellen von networkIPv6ConfigurationManagementCondition
description: Erstellen eines neuen networkIPv6ConfigurationManagementCondition-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34db810cfcb62472a125d92487d6235b8f70d7ed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411925"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="a8a53-103">Erstellen von networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a8a53-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="a8a53-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a8a53-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8a53-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8a53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8a53-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8a53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8a53-107">Erstellen eines neuen [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a8a53-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8a53-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8a53-108">Prerequisites</span></span>
<span data-ttu-id="a8a53-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8a53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a8a53-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8a53-111">Permission type</span></span>|<span data-ttu-id="a8a53-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8a53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8a53-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8a53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8a53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8a53-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8a53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8a53-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8a53-116">Not supported.</span></span>|
|<span data-ttu-id="a8a53-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8a53-117">Application</span></span>|<span data-ttu-id="a8a53-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8a53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8a53-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8a53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="a8a53-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8a53-120">Request headers</span></span>
|<span data-ttu-id="a8a53-121">Header</span><span class="sxs-lookup"><span data-stu-id="a8a53-121">Header</span></span>|<span data-ttu-id="a8a53-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a8a53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8a53-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a8a53-123">Authorization</span></span>|<span data-ttu-id="a8a53-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8a53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8a53-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a8a53-125">Accept</span></span>|<span data-ttu-id="a8a53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8a53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a53-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8a53-127">Request body</span></span>
<span data-ttu-id="a8a53-128">Geben Sie im Textkörper Anforderung für das Objekt networkIPv6ConfigurationManagementCondition eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a8a53-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="a8a53-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die networkIPv6ConfigurationManagementCondition erstellen.</span><span class="sxs-lookup"><span data-stu-id="a8a53-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="a8a53-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8a53-130">Property</span></span>|<span data-ttu-id="a8a53-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a8a53-131">Type</span></span>|<span data-ttu-id="a8a53-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8a53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a53-133">id</span><span class="sxs-lookup"><span data-stu-id="a8a53-133">id</span></span>|<span data-ttu-id="a8a53-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-134">String</span></span>|<span data-ttu-id="a8a53-135">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a8a53-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="a8a53-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="a8a53-136">System generated value assigned when created.</span></span> <span data-ttu-id="a8a53-137">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="a8a53-138">uniqueName</span></span>|<span data-ttu-id="a8a53-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-139">String</span></span>|<span data-ttu-id="a8a53-140">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a8a53-140">Unique name for the management condition.</span></span> <span data-ttu-id="a8a53-141">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="a8a53-141">Used in management condition expressions.</span></span> <span data-ttu-id="a8a53-142">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-143">displayName</span><span class="sxs-lookup"><span data-stu-id="a8a53-143">displayName</span></span>|<span data-ttu-id="a8a53-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-144">String</span></span>|<span data-ttu-id="a8a53-145">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a8a53-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="a8a53-146">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-147">description</span><span class="sxs-lookup"><span data-stu-id="a8a53-147">description</span></span>|<span data-ttu-id="a8a53-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-148">String</span></span>|<span data-ttu-id="a8a53-149">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a8a53-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="a8a53-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8a53-151">createdDateTime</span></span>|<span data-ttu-id="a8a53-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8a53-152">DateTimeOffset</span></span>|<span data-ttu-id="a8a53-153">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="a8a53-153">The time the management condition was created.</span></span> <span data-ttu-id="a8a53-154">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="a8a53-154">Generated service side.</span></span> <span data-ttu-id="a8a53-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8a53-156">modifiedDateTime</span></span>|<span data-ttu-id="a8a53-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8a53-157">DateTimeOffset</span></span>|<span data-ttu-id="a8a53-158">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="a8a53-158">The time the management condition was last modified.</span></span> <span data-ttu-id="a8a53-159">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="a8a53-159">Updated service side.</span></span> <span data-ttu-id="a8a53-160">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-161">eTag</span><span class="sxs-lookup"><span data-stu-id="a8a53-161">eTag</span></span>|<span data-ttu-id="a8a53-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-162">String</span></span>|<span data-ttu-id="a8a53-163">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a8a53-163">ETag of the management condition.</span></span> <span data-ttu-id="a8a53-164">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="a8a53-164">Updated service side.</span></span> <span data-ttu-id="a8a53-165">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a53-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a8a53-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a8a53-166">applicablePlatforms</span></span>|<span data-ttu-id="a8a53-167">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a8a53-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a8a53-168">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a8a53-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="a8a53-169">Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="a8a53-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="a8a53-170">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="a8a53-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="a8a53-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="a8a53-171">ipV6Prefix</span></span>|<span data-ttu-id="a8a53-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-172">String</span></span>|<span data-ttu-id="a8a53-173">Die IPv6-Subnetz mit verbunden sein.</span><span class="sxs-lookup"><span data-stu-id="a8a53-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="a8a53-174">Diese Vorgaben unter 2001:db8:: / 32</span><span class="sxs-lookup"><span data-stu-id="a8a53-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="a8a53-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="a8a53-175">ipV6Gateway</span></span>|<span data-ttu-id="a8a53-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a53-176">String</span></span>|<span data-ttu-id="a8a53-177">Die IPv6-Gateway-Adresse zu.</span><span class="sxs-lookup"><span data-stu-id="a8a53-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="a8a53-178">z. B. 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="a8a53-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="a8a53-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="a8a53-179">ipV6DNSServerList</span></span>|<span data-ttu-id="a8a53-180">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a8a53-180">String collection</span></span>|<span data-ttu-id="a8a53-181">Eine IPv6-DNS-Server für den Adapter konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="a8a53-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="a8a53-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="a8a53-182">dnsSuffixList</span></span>|<span data-ttu-id="a8a53-183">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a8a53-183">String collection</span></span>|<span data-ttu-id="a8a53-184">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="a8a53-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="a8a53-185">Diese Vorgaben unter seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="a8a53-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="a8a53-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8a53-186">Response</span></span>
<span data-ttu-id="a8a53-187">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a8a53-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a53-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8a53-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8a53-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8a53-189">Request</span></span>
<span data-ttu-id="a8a53-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8a53-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a8a53-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8a53-191">Response</span></span>
<span data-ttu-id="a8a53-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8a53-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




