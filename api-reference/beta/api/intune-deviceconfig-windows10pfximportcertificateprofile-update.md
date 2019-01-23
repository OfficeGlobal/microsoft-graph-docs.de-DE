---
title: Windows10PFXImportCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows10PFXImportCertificateProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eae2c39f2244dab4db2b4b034f04d2ce11008c2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408803"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="d78ef-103">Windows10PFXImportCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d78ef-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="d78ef-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d78ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d78ef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d78ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d78ef-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d78ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d78ef-107">Aktualisieren Sie die Eigenschaften eines [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d78ef-107">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d78ef-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d78ef-108">Prerequisites</span></span>
<span data-ttu-id="d78ef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d78ef-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d78ef-111">Permission type</span></span>|<span data-ttu-id="d78ef-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d78ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d78ef-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d78ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d78ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d78ef-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d78ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d78ef-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d78ef-116">Not supported.</span></span>|
|<span data-ttu-id="d78ef-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d78ef-117">Application</span></span>|<span data-ttu-id="d78ef-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d78ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d78ef-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d78ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d78ef-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d78ef-120">Request headers</span></span>
|<span data-ttu-id="d78ef-121">Header</span><span class="sxs-lookup"><span data-stu-id="d78ef-121">Header</span></span>|<span data-ttu-id="d78ef-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d78ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d78ef-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d78ef-123">Authorization</span></span>|<span data-ttu-id="d78ef-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d78ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d78ef-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d78ef-125">Accept</span></span>|<span data-ttu-id="d78ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d78ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d78ef-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d78ef-127">Request body</span></span>
<span data-ttu-id="d78ef-128">Geben Sie im Textkörper Anforderung für das Objekt [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d78ef-128">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="d78ef-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d78ef-129">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="d78ef-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d78ef-130">Property</span></span>|<span data-ttu-id="d78ef-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d78ef-131">Type</span></span>|<span data-ttu-id="d78ef-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d78ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78ef-133">id</span><span class="sxs-lookup"><span data-stu-id="d78ef-133">id</span></span>|<span data-ttu-id="d78ef-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d78ef-134">String</span></span>|<span data-ttu-id="d78ef-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d78ef-135">Key of the entity.</span></span> <span data-ttu-id="d78ef-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d78ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d78ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78ef-138">DateTimeOffset</span></span>|<span data-ttu-id="d78ef-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d78ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d78ef-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d78ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="d78ef-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d78ef-142">String collection</span></span>|<span data-ttu-id="d78ef-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="d78ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d78ef-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d78ef-145">supportsScopeTags</span></span>|<span data-ttu-id="d78ef-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78ef-146">Boolean</span></span>|<span data-ttu-id="d78ef-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d78ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d78ef-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="d78ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d78ef-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d78ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d78ef-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d78ef-150">This property is read-only.</span></span> <span data-ttu-id="d78ef-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d78ef-152">createdDateTime</span></span>|<span data-ttu-id="d78ef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78ef-153">DateTimeOffset</span></span>|<span data-ttu-id="d78ef-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d78ef-154">DateTime the object was created.</span></span> <span data-ttu-id="d78ef-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-156">description</span><span class="sxs-lookup"><span data-stu-id="d78ef-156">description</span></span>|<span data-ttu-id="d78ef-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d78ef-157">String</span></span>|<span data-ttu-id="d78ef-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d78ef-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d78ef-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d78ef-160">displayName</span></span>|<span data-ttu-id="d78ef-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d78ef-161">String</span></span>|<span data-ttu-id="d78ef-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d78ef-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d78ef-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-164">Version</span><span class="sxs-lookup"><span data-stu-id="d78ef-164">version</span></span>|<span data-ttu-id="d78ef-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d78ef-165">Int32</span></span>|<span data-ttu-id="d78ef-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d78ef-166">Version of the device configuration.</span></span> <span data-ttu-id="d78ef-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78ef-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78ef-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d78ef-168">keyStorageProvider</span></span>|[<span data-ttu-id="d78ef-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d78ef-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d78ef-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d78ef-170">Not yet documented.</span></span> <span data-ttu-id="d78ef-171">Mögliche Werte sind: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="d78ef-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="d78ef-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="d78ef-172">Response</span></span>
<span data-ttu-id="d78ef-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d78ef-173">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78ef-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d78ef-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="d78ef-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d78ef-175">Request</span></span>
<span data-ttu-id="d78ef-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d78ef-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="d78ef-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="d78ef-177">Response</span></span>
<span data-ttu-id="d78ef-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d78ef-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```




