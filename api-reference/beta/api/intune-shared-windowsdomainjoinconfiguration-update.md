---
title: WindowsDomainJoinConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windowsDomainJoinConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2e0700a630d3009520b290da269b213623bdf48a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571662"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="c6271-103">WindowsDomainJoinConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c6271-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="c6271-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="c6271-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c6271-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6271-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6271-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c6271-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6271-107">Aktualisieren der Eigenschaften eines [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6271-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6271-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c6271-108">Prerequisites</span></span>
<span data-ttu-id="c6271-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c6271-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6271-111">Permission type</span></span>|<span data-ttu-id="c6271-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6271-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6271-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6271-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c6271-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="c6271-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c6271-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6271-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c6271-116">&nbsp;&nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="c6271-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c6271-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6271-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6271-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6271-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6271-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6271-119">Not supported.</span></span>|
|<span data-ttu-id="c6271-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6271-120">Application</span></span>|<span data-ttu-id="c6271-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6271-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6271-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6271-122">HTTP Request</span></span>

<span data-ttu-id="c6271-123">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="c6271-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="c6271-124">**Registrierungs**</span><span class="sxs-lookup"><span data-stu-id="c6271-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c6271-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6271-125">Request headers</span></span>
|<span data-ttu-id="c6271-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c6271-126">Header</span></span>|<span data-ttu-id="c6271-127">Wert</span><span class="sxs-lookup"><span data-stu-id="c6271-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6271-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6271-128">Authorization</span></span>|<span data-ttu-id="c6271-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c6271-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6271-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c6271-130">Accept</span></span>|<span data-ttu-id="c6271-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c6271-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6271-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6271-132">Request body</span></span>
<span data-ttu-id="c6271-133">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c6271-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="c6271-134">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c6271-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="c6271-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6271-135">Property</span></span>|<span data-ttu-id="c6271-136">Typ</span><span class="sxs-lookup"><span data-stu-id="c6271-136">Type</span></span>|<span data-ttu-id="c6271-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6271-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6271-138">id</span><span class="sxs-lookup"><span data-stu-id="c6271-138">id</span></span>|<span data-ttu-id="c6271-139">String</span><span class="sxs-lookup"><span data-stu-id="c6271-139">String</span></span>|<span data-ttu-id="c6271-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c6271-140">Key of the entity.</span></span> <span data-ttu-id="c6271-141">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-142">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="c6271-142">**Device configuration**</span></span>|
|<span data-ttu-id="c6271-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="c6271-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="c6271-144">String</span><span class="sxs-lookup"><span data-stu-id="c6271-144">String</span></span>|<span data-ttu-id="c6271-145">Active Directory-Domänenname, der beitreten soll.</span><span class="sxs-lookup"><span data-stu-id="c6271-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="c6271-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="c6271-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="c6271-147">String</span><span class="sxs-lookup"><span data-stu-id="c6271-147">String</span></span>|<span data-ttu-id="c6271-148">Fester Präfix für Computername.</span><span class="sxs-lookup"><span data-stu-id="c6271-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="c6271-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="c6271-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="c6271-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c6271-150">Int32</span></span>|<span data-ttu-id="c6271-151">Dynamisch generierte Zeichen, die als Suffix für den Computernamen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c6271-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="c6271-152">Gültige Werte 3 bis 14</span><span class="sxs-lookup"><span data-stu-id="c6271-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="c6271-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6271-153">createdDateTime</span></span>|<span data-ttu-id="c6271-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6271-154">DateTimeOffset</span></span>|<span data-ttu-id="c6271-155">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6271-155">DateTime the object was created.</span></span> <span data-ttu-id="c6271-156">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-157">description</span><span class="sxs-lookup"><span data-stu-id="c6271-157">description</span></span>|<span data-ttu-id="c6271-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6271-158">String</span></span>|<span data-ttu-id="c6271-159">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c6271-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c6271-160">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-161">displayName</span><span class="sxs-lookup"><span data-stu-id="c6271-161">displayName</span></span>|<span data-ttu-id="c6271-162">String</span><span class="sxs-lookup"><span data-stu-id="c6271-162">String</span></span>|<span data-ttu-id="c6271-163">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c6271-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c6271-164">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6271-165">lastModifiedDateTime</span></span>|<span data-ttu-id="c6271-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6271-166">DateTimeOffset</span></span>|<span data-ttu-id="c6271-167">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6271-167">DateTime the object was last modified.</span></span> <span data-ttu-id="c6271-168">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="c6271-169">organizationalUnit</span></span>|<span data-ttu-id="c6271-170">String</span><span class="sxs-lookup"><span data-stu-id="c6271-170">String</span></span>|<span data-ttu-id="c6271-171">Organisationseinheit (Organizational Unit, OU), in der das Computerkonto erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="c6271-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="c6271-172">Wenn dieser Parameter NULL ist, wird der bekannte Computerobjekt Container als veröffentlicht in der Domäne verwendet.</span><span class="sxs-lookup"><span data-stu-id="c6271-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="c6271-173">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c6271-173">roleScopeTagIds</span></span>|<span data-ttu-id="c6271-174">String collection</span><span class="sxs-lookup"><span data-stu-id="c6271-174">String collection</span></span>|<span data-ttu-id="c6271-175">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c6271-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c6271-176">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c6271-177">supportsScopeTags</span></span>|<span data-ttu-id="c6271-178">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c6271-178">Boolean</span></span>|<span data-ttu-id="c6271-179">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6271-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c6271-180">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="c6271-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c6271-181">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c6271-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c6271-182">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6271-182">This property is read-only.</span></span> <span data-ttu-id="c6271-183">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6271-184">Version</span><span class="sxs-lookup"><span data-stu-id="c6271-184">version</span></span>|<span data-ttu-id="c6271-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c6271-185">Int32</span></span>|<span data-ttu-id="c6271-186">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c6271-186">Version of the device configuration.</span></span> <span data-ttu-id="c6271-187">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6271-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="c6271-188">Hinweis: die Unterstützung von Anforderungstext Körpern hängt vom Kontext des Aufrufs ab.</span><span class="sxs-lookup"><span data-stu-id="c6271-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="c6271-189">Nicht alle Eigenschaften sind für alle Workflows geeignet.</span><span class="sxs-lookup"><span data-stu-id="c6271-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="c6271-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6271-190">Response</span></span>
<span data-ttu-id="c6271-191">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c6271-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6271-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6271-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6271-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6271-193">Request</span></span>
<span data-ttu-id="c6271-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6271-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 344

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="c6271-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6271-195">Response</span></span>
<span data-ttu-id="c6271-196">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6271-196">Here is an example of the response.</span></span> <span data-ttu-id="c6271-197">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="c6271-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c6271-198">Von tatsächlichen aufrufen zurückgegebene Eigenschaften variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="c6271-198">Properties returned by actual calls vary according to the context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```



