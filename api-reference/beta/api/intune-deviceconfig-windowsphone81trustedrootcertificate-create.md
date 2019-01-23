---
title: Erstellen von windowsPhone81TrustedRootCertificate
description: Erstellen eines neuen windowsPhone81TrustedRootCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbabf0ad844712aab587e62830f0fc3654db19d4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417294"
---
# <a name="create-windowsphone81trustedrootcertificate"></a><span data-ttu-id="0c4da-103">Erstellen von windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0c4da-103">Create windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="0c4da-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0c4da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c4da-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c4da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c4da-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c4da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c4da-107">Erstellen eines neuen [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c4da-107">Create a new [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c4da-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c4da-108">Prerequisites</span></span>
<span data-ttu-id="0c4da-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0c4da-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c4da-111">Permission type</span></span>|<span data-ttu-id="0c4da-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c4da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c4da-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c4da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c4da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c4da-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c4da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c4da-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c4da-116">Not supported.</span></span>|
|<span data-ttu-id="0c4da-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c4da-117">Application</span></span>|<span data-ttu-id="0c4da-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c4da-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c4da-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c4da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c4da-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c4da-120">Request headers</span></span>
|<span data-ttu-id="0c4da-121">Header</span><span class="sxs-lookup"><span data-stu-id="0c4da-121">Header</span></span>|<span data-ttu-id="0c4da-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0c4da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c4da-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0c4da-123">Authorization</span></span>|<span data-ttu-id="0c4da-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c4da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c4da-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c4da-125">Accept</span></span>|<span data-ttu-id="0c4da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4da-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c4da-127">Request body</span></span>
<span data-ttu-id="0c4da-128">Geben Sie im Textkörper Anforderung für das Objekt windowsPhone81TrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0c4da-128">In the request body, supply a JSON representation for the windowsPhone81TrustedRootCertificate object.</span></span>

<span data-ttu-id="0c4da-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windowsPhone81TrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="0c4da-129">The following table shows the properties that are required when you create the windowsPhone81TrustedRootCertificate.</span></span>

|<span data-ttu-id="0c4da-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c4da-130">Property</span></span>|<span data-ttu-id="0c4da-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0c4da-131">Type</span></span>|<span data-ttu-id="0c4da-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c4da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c4da-133">id</span><span class="sxs-lookup"><span data-stu-id="0c4da-133">id</span></span>|<span data-ttu-id="0c4da-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c4da-134">String</span></span>|<span data-ttu-id="0c4da-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0c4da-135">Key of the entity.</span></span> <span data-ttu-id="0c4da-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c4da-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0c4da-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c4da-138">DateTimeOffset</span></span>|<span data-ttu-id="0c4da-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c4da-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0c4da-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c4da-141">roleScopeTagIds</span></span>|<span data-ttu-id="0c4da-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0c4da-142">String collection</span></span>|<span data-ttu-id="0c4da-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0c4da-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0c4da-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0c4da-145">supportsScopeTags</span></span>|<span data-ttu-id="0c4da-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c4da-146">Boolean</span></span>|<span data-ttu-id="0c4da-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c4da-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0c4da-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0c4da-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0c4da-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0c4da-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0c4da-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0c4da-150">This property is read-only.</span></span> <span data-ttu-id="0c4da-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c4da-152">createdDateTime</span></span>|<span data-ttu-id="0c4da-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c4da-153">DateTimeOffset</span></span>|<span data-ttu-id="0c4da-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c4da-154">DateTime the object was created.</span></span> <span data-ttu-id="0c4da-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-156">description</span><span class="sxs-lookup"><span data-stu-id="0c4da-156">description</span></span>|<span data-ttu-id="0c4da-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c4da-157">String</span></span>|<span data-ttu-id="0c4da-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0c4da-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c4da-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0c4da-160">displayName</span></span>|<span data-ttu-id="0c4da-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c4da-161">String</span></span>|<span data-ttu-id="0c4da-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0c4da-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c4da-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-164">Version</span><span class="sxs-lookup"><span data-stu-id="0c4da-164">version</span></span>|<span data-ttu-id="0c4da-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0c4da-165">Int32</span></span>|<span data-ttu-id="0c4da-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0c4da-166">Version of the device configuration.</span></span> <span data-ttu-id="0c4da-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c4da-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c4da-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0c4da-168">trustedRootCertificate</span></span>|<span data-ttu-id="0c4da-169">Binär</span><span class="sxs-lookup"><span data-stu-id="0c4da-169">Binary</span></span>|<span data-ttu-id="0c4da-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="0c4da-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="0c4da-171">Aus</span><span class="sxs-lookup"><span data-stu-id="0c4da-171">certFileName</span></span>|<span data-ttu-id="0c4da-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c4da-172">String</span></span>|<span data-ttu-id="0c4da-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0c4da-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="0c4da-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c4da-174">Response</span></span>
<span data-ttu-id="0c4da-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0c4da-175">If successful, this method returns a `201 Created` response code and a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4da-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c4da-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c4da-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c4da-177">Request</span></span>
<span data-ttu-id="0c4da-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c4da-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="0c4da-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c4da-179">Response</span></span>
<span data-ttu-id="0c4da-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c4da-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




