---
title: Windows10PFXImportCertificateProfile erstellen
description: Erstellen eines neuen windows10PFXImportCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78b9c6443b7f22d76df289ad232dbef8f05d0280
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980453"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="482bd-103">Windows10PFXImportCertificateProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="482bd-103">Create windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="482bd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="482bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="482bd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="482bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="482bd-106">Erstellen eines neuen [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="482bd-106">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="482bd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="482bd-107">Prerequisites</span></span>
<span data-ttu-id="482bd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="482bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="482bd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="482bd-110">Permission type</span></span>|<span data-ttu-id="482bd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="482bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="482bd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="482bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="482bd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="482bd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="482bd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="482bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="482bd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="482bd-115">Not supported.</span></span>|
|<span data-ttu-id="482bd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="482bd-116">Application</span></span>|<span data-ttu-id="482bd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="482bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="482bd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="482bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="482bd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="482bd-119">Request headers</span></span>
|<span data-ttu-id="482bd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="482bd-120">Header</span></span>|<span data-ttu-id="482bd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="482bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="482bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="482bd-122">Authorization</span></span>|<span data-ttu-id="482bd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="482bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="482bd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="482bd-124">Accept</span></span>|<span data-ttu-id="482bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="482bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="482bd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="482bd-126">Request body</span></span>
<span data-ttu-id="482bd-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows10PFXImportCertificateProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="482bd-127">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="482bd-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10PFXImportCertificateProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="482bd-128">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="482bd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="482bd-129">Property</span></span>|<span data-ttu-id="482bd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="482bd-130">Type</span></span>|<span data-ttu-id="482bd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="482bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="482bd-132">id</span><span class="sxs-lookup"><span data-stu-id="482bd-132">id</span></span>|<span data-ttu-id="482bd-133">String</span><span class="sxs-lookup"><span data-stu-id="482bd-133">String</span></span>|<span data-ttu-id="482bd-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="482bd-134">Key of the entity.</span></span> <span data-ttu-id="482bd-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="482bd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="482bd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="482bd-137">DateTimeOffset</span></span>|<span data-ttu-id="482bd-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="482bd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="482bd-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="482bd-140">roleScopeTagIds</span></span>|<span data-ttu-id="482bd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="482bd-141">String collection</span></span>|<span data-ttu-id="482bd-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="482bd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="482bd-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="482bd-144">supportsScopeTags</span></span>|<span data-ttu-id="482bd-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="482bd-145">Boolean</span></span>|<span data-ttu-id="482bd-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="482bd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="482bd-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="482bd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="482bd-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="482bd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="482bd-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="482bd-149">This property is read-only.</span></span> <span data-ttu-id="482bd-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="482bd-151">createdDateTime</span></span>|<span data-ttu-id="482bd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="482bd-152">DateTimeOffset</span></span>|<span data-ttu-id="482bd-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="482bd-153">DateTime the object was created.</span></span> <span data-ttu-id="482bd-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-155">description</span><span class="sxs-lookup"><span data-stu-id="482bd-155">description</span></span>|<span data-ttu-id="482bd-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="482bd-156">String</span></span>|<span data-ttu-id="482bd-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="482bd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="482bd-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="482bd-159">displayName</span></span>|<span data-ttu-id="482bd-160">String</span><span class="sxs-lookup"><span data-stu-id="482bd-160">String</span></span>|<span data-ttu-id="482bd-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="482bd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="482bd-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-163">Version</span><span class="sxs-lookup"><span data-stu-id="482bd-163">version</span></span>|<span data-ttu-id="482bd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="482bd-164">Int32</span></span>|<span data-ttu-id="482bd-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="482bd-165">Version of the device configuration.</span></span> <span data-ttu-id="482bd-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="482bd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="482bd-167">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="482bd-167">keyStorageProvider</span></span>|[<span data-ttu-id="482bd-168">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="482bd-168">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="482bd-169">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="482bd-169">Not yet documented.</span></span> <span data-ttu-id="482bd-170">Mögliche Werte sind: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="482bd-170">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="482bd-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="482bd-171">Response</span></span>
<span data-ttu-id="482bd-172">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="482bd-172">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="482bd-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="482bd-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="482bd-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="482bd-174">Request</span></span>
<span data-ttu-id="482bd-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="482bd-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="482bd-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="482bd-176">Response</span></span>
<span data-ttu-id="482bd-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="482bd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




