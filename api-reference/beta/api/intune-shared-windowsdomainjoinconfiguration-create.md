---
title: WindowsDomainJoinConfiguration erstellen
description: Erstellen eines neuen windowsDomainJoinConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 23cce64cfd6040a5605c6eaba022e39aae745c59
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571865"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="33b3b-103">WindowsDomainJoinConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="33b3b-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="33b3b-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="33b3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33b3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33b3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33b3b-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="33b3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b3b-107">Erstellen eines neuen [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b3b-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33b3b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33b3b-108">Prerequisites</span></span>
<span data-ttu-id="33b3b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33b3b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33b3b-111">Permission type</span></span>|<span data-ttu-id="33b3b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33b3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b3b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33b3b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="33b3b-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="33b3b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="33b3b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b3b-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="33b3b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33b3b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b3b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33b3b-117">Not supported.</span></span>|
|<span data-ttu-id="33b3b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33b3b-118">Application</span></span>|<span data-ttu-id="33b3b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33b3b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b3b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b3b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33b3b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33b3b-121">Request headers</span></span>

|<span data-ttu-id="33b3b-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33b3b-122">Header</span></span>|<span data-ttu-id="33b3b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="33b3b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33b3b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33b3b-124">Authorization</span></span>|<span data-ttu-id="33b3b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33b3b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33b3b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33b3b-126">Accept</span></span>|<span data-ttu-id="33b3b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="33b3b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b3b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33b3b-128">Request body</span></span>

<span data-ttu-id="33b3b-129">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsDomainJoinConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="33b3b-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="33b3b-130">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsDomainJoinConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33b3b-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="33b3b-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33b3b-131">Property</span></span>|<span data-ttu-id="33b3b-132">Typ</span><span class="sxs-lookup"><span data-stu-id="33b3b-132">Type</span></span>|<span data-ttu-id="33b3b-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33b3b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b3b-134">id</span><span class="sxs-lookup"><span data-stu-id="33b3b-134">id</span></span>|<span data-ttu-id="33b3b-135">String</span><span class="sxs-lookup"><span data-stu-id="33b3b-135">String</span></span>|<span data-ttu-id="33b3b-136">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33b3b-136">Key of the entity.</span></span> <span data-ttu-id="33b3b-137">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-138">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="33b3b-138">**Device configuration**</span></span>|
|<span data-ttu-id="33b3b-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="33b3b-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="33b3b-140">String</span><span class="sxs-lookup"><span data-stu-id="33b3b-140">String</span></span>|<span data-ttu-id="33b3b-141">Active Directory-Domänenname, der beitreten soll.</span><span class="sxs-lookup"><span data-stu-id="33b3b-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="33b3b-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="33b3b-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="33b3b-143">String</span><span class="sxs-lookup"><span data-stu-id="33b3b-143">String</span></span>|<span data-ttu-id="33b3b-144">Fester Präfix für Computername.</span><span class="sxs-lookup"><span data-stu-id="33b3b-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="33b3b-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="33b3b-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="33b3b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="33b3b-146">Int32</span></span>|<span data-ttu-id="33b3b-147">Dynamisch generierte Zeichen, die als Suffix für den Computernamen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="33b3b-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="33b3b-148">Gültige Werte 3 bis 14</span><span class="sxs-lookup"><span data-stu-id="33b3b-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="33b3b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33b3b-149">createdDateTime</span></span>|<span data-ttu-id="33b3b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b3b-150">DateTimeOffset</span></span>|<span data-ttu-id="33b3b-151">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b3b-151">DateTime the object was created.</span></span> <span data-ttu-id="33b3b-152">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-153">description</span><span class="sxs-lookup"><span data-stu-id="33b3b-153">description</span></span>|<span data-ttu-id="33b3b-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33b3b-154">String</span></span>|<span data-ttu-id="33b3b-155">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33b3b-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33b3b-156">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-157">displayName</span><span class="sxs-lookup"><span data-stu-id="33b3b-157">displayName</span></span>|<span data-ttu-id="33b3b-158">String</span><span class="sxs-lookup"><span data-stu-id="33b3b-158">String</span></span>|<span data-ttu-id="33b3b-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33b3b-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33b3b-160">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33b3b-161">lastModifiedDateTime</span></span>|<span data-ttu-id="33b3b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b3b-162">DateTimeOffset</span></span>|<span data-ttu-id="33b3b-163">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b3b-163">DateTime the object was last modified.</span></span> <span data-ttu-id="33b3b-164">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="33b3b-165">organizationalUnit</span></span>|<span data-ttu-id="33b3b-166">String</span><span class="sxs-lookup"><span data-stu-id="33b3b-166">String</span></span>|<span data-ttu-id="33b3b-167">Organisationseinheit (Organizational Unit, OU), in der das Computerkonto erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="33b3b-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="33b3b-168">Wenn dieser Parameter NULL ist, wird der bekannte Computerobjekt Container als veröffentlicht in der Domäne verwendet.</span><span class="sxs-lookup"><span data-stu-id="33b3b-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="33b3b-169">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="33b3b-169">roleScopeTagIds</span></span>|<span data-ttu-id="33b3b-170">String collection</span><span class="sxs-lookup"><span data-stu-id="33b3b-170">String collection</span></span>|<span data-ttu-id="33b3b-171">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="33b3b-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33b3b-172">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33b3b-173">supportsScopeTags</span></span>|<span data-ttu-id="33b3b-174">Boolesch</span><span class="sxs-lookup"><span data-stu-id="33b3b-174">Boolean</span></span>|<span data-ttu-id="33b3b-175">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33b3b-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33b3b-176">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="33b3b-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33b3b-177">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="33b3b-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33b3b-178">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b3b-178">This property is read-only.</span></span> <span data-ttu-id="33b3b-179">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33b3b-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b3b-180">Version</span><span class="sxs-lookup"><span data-stu-id="33b3b-180">version</span></span>|<span data-ttu-id="33b3b-181">Int32</span><span class="sxs-lookup"><span data-stu-id="33b3b-181">Int32</span></span>|<span data-ttu-id="33b3b-182">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33b3b-182">Version of the device configuration.</span></span> <span data-ttu-id="33b3b-183">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b3b-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="33b3b-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b3b-184">Response</span></span>

<span data-ttu-id="33b3b-185">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33b3b-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b3b-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33b3b-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="33b3b-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b3b-187">Request</span></span>

<span data-ttu-id="33b3b-188">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33b3b-188">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 559

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```

### <a name="response"></a><span data-ttu-id="33b3b-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b3b-189">Response</span></span>

<span data-ttu-id="33b3b-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33b3b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```



