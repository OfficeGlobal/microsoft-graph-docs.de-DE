---
title: Erstellen von androidTrustedRootCertificate
description: Erstellen eines neuen AndroidTrustedRootCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 901d3d94025a4a40c2d57c5c53e3cdb4ac30f0ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401446"
---
# <a name="create-androidtrustedrootcertificate"></a><span data-ttu-id="39cf6-103">Erstellen von androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="39cf6-103">Create androidTrustedRootCertificate</span></span>

> <span data-ttu-id="39cf6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="39cf6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39cf6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39cf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39cf6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39cf6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39cf6-107">Erstellen eines neuen [AndroidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="39cf6-107">Create a new [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39cf6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39cf6-108">Prerequisites</span></span>
<span data-ttu-id="39cf6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39cf6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39cf6-111">Permission type</span></span>|<span data-ttu-id="39cf6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39cf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39cf6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39cf6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39cf6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39cf6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39cf6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39cf6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39cf6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39cf6-116">Not supported.</span></span>|
|<span data-ttu-id="39cf6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39cf6-117">Application</span></span>|<span data-ttu-id="39cf6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39cf6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39cf6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39cf6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39cf6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39cf6-120">Request headers</span></span>
|<span data-ttu-id="39cf6-121">Header</span><span class="sxs-lookup"><span data-stu-id="39cf6-121">Header</span></span>|<span data-ttu-id="39cf6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="39cf6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39cf6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="39cf6-123">Authorization</span></span>|<span data-ttu-id="39cf6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39cf6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39cf6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="39cf6-125">Accept</span></span>|<span data-ttu-id="39cf6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39cf6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39cf6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39cf6-127">Request body</span></span>
<span data-ttu-id="39cf6-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidTrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="39cf6-128">In the request body, supply a JSON representation for the androidTrustedRootCertificate object.</span></span>

<span data-ttu-id="39cf6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidTrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="39cf6-129">The following table shows the properties that are required when you create the androidTrustedRootCertificate.</span></span>

|<span data-ttu-id="39cf6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39cf6-130">Property</span></span>|<span data-ttu-id="39cf6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="39cf6-131">Type</span></span>|<span data-ttu-id="39cf6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39cf6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39cf6-133">id</span><span class="sxs-lookup"><span data-stu-id="39cf6-133">id</span></span>|<span data-ttu-id="39cf6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39cf6-134">String</span></span>|<span data-ttu-id="39cf6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="39cf6-135">Key of the entity.</span></span> <span data-ttu-id="39cf6-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39cf6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39cf6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39cf6-138">DateTimeOffset</span></span>|<span data-ttu-id="39cf6-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="39cf6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="39cf6-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39cf6-141">roleScopeTagIds</span></span>|<span data-ttu-id="39cf6-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="39cf6-142">String collection</span></span>|<span data-ttu-id="39cf6-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="39cf6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39cf6-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39cf6-145">supportsScopeTags</span></span>|<span data-ttu-id="39cf6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="39cf6-146">Boolean</span></span>|<span data-ttu-id="39cf6-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39cf6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39cf6-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="39cf6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39cf6-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="39cf6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39cf6-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="39cf6-150">This property is read-only.</span></span> <span data-ttu-id="39cf6-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39cf6-152">createdDateTime</span></span>|<span data-ttu-id="39cf6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39cf6-153">DateTimeOffset</span></span>|<span data-ttu-id="39cf6-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="39cf6-154">DateTime the object was created.</span></span> <span data-ttu-id="39cf6-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-156">description</span><span class="sxs-lookup"><span data-stu-id="39cf6-156">description</span></span>|<span data-ttu-id="39cf6-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39cf6-157">String</span></span>|<span data-ttu-id="39cf6-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="39cf6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39cf6-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="39cf6-160">displayName</span></span>|<span data-ttu-id="39cf6-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39cf6-161">String</span></span>|<span data-ttu-id="39cf6-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="39cf6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39cf6-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-164">Version</span><span class="sxs-lookup"><span data-stu-id="39cf6-164">version</span></span>|<span data-ttu-id="39cf6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="39cf6-165">Int32</span></span>|<span data-ttu-id="39cf6-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="39cf6-166">Version of the device configuration.</span></span> <span data-ttu-id="39cf6-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39cf6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39cf6-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="39cf6-168">trustedRootCertificate</span></span>|<span data-ttu-id="39cf6-169">Binär</span><span class="sxs-lookup"><span data-stu-id="39cf6-169">Binary</span></span>|<span data-ttu-id="39cf6-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="39cf6-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="39cf6-171">Aus</span><span class="sxs-lookup"><span data-stu-id="39cf6-171">certFileName</span></span>|<span data-ttu-id="39cf6-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39cf6-172">String</span></span>|<span data-ttu-id="39cf6-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="39cf6-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="39cf6-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="39cf6-174">Response</span></span>
<span data-ttu-id="39cf6-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="39cf6-175">If successful, this method returns a `201 Created` response code and a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39cf6-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39cf6-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="39cf6-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39cf6-177">Request</span></span>
<span data-ttu-id="39cf6-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39cf6-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="39cf6-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="39cf6-179">Response</span></span>
<span data-ttu-id="39cf6-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39cf6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
  "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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




