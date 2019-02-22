---
title: targetedManagedAppConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppConfiguration- Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9594677f767707123d7b9d82b60bfad07d2148a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159738"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="520ee-103">targetedManagedAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="520ee-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="520ee-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="520ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="520ee-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="520ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="520ee-106">Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)- Objekts.</span><span class="sxs-lookup"><span data-stu-id="520ee-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="520ee-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="520ee-107">Prerequisites</span></span>
<span data-ttu-id="520ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="520ee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="520ee-110">Permission type</span></span>|<span data-ttu-id="520ee-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="520ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="520ee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="520ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="520ee-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="520ee-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="520ee-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="520ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="520ee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="520ee-115">Not supported.</span></span>|
|<span data-ttu-id="520ee-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="520ee-116">Application</span></span>|<span data-ttu-id="520ee-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="520ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="520ee-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="520ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="520ee-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="520ee-119">Request headers</span></span>
|<span data-ttu-id="520ee-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="520ee-120">Header</span></span>|<span data-ttu-id="520ee-121">Wert</span><span class="sxs-lookup"><span data-stu-id="520ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="520ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="520ee-122">Authorization</span></span>|<span data-ttu-id="520ee-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="520ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="520ee-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="520ee-124">Accept</span></span>|<span data-ttu-id="520ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="520ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="520ee-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="520ee-126">Request body</span></span>
<span data-ttu-id="520ee-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="520ee-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="520ee-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="520ee-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="520ee-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="520ee-129">Property</span></span>|<span data-ttu-id="520ee-130">Typ</span><span class="sxs-lookup"><span data-stu-id="520ee-130">Type</span></span>|<span data-ttu-id="520ee-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="520ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="520ee-132">displayName</span><span class="sxs-lookup"><span data-stu-id="520ee-132">displayName</span></span>|<span data-ttu-id="520ee-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520ee-133">String</span></span>|<span data-ttu-id="520ee-134">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="520ee-134">Policy display name.</span></span> <span data-ttu-id="520ee-135">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-136">description</span><span class="sxs-lookup"><span data-stu-id="520ee-136">description</span></span>|<span data-ttu-id="520ee-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520ee-137">String</span></span>|<span data-ttu-id="520ee-138">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="520ee-138">The policy's description.</span></span> <span data-ttu-id="520ee-139">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="520ee-140">createdDateTime</span></span>|<span data-ttu-id="520ee-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="520ee-141">DateTimeOffset</span></span>|<span data-ttu-id="520ee-142">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="520ee-142">The date and time the policy was created.</span></span> <span data-ttu-id="520ee-143">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="520ee-144">lastModifiedDateTime</span></span>|<span data-ttu-id="520ee-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="520ee-145">DateTimeOffset</span></span>|<span data-ttu-id="520ee-146">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="520ee-146">Last time the policy was modified.</span></span> <span data-ttu-id="520ee-147">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-148">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="520ee-148">roleScopeTagIds</span></span>|<span data-ttu-id="520ee-149">String collection</span><span class="sxs-lookup"><span data-stu-id="520ee-149">String collection</span></span>|<span data-ttu-id="520ee-150">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="520ee-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="520ee-151">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-152">id</span><span class="sxs-lookup"><span data-stu-id="520ee-152">id</span></span>|<span data-ttu-id="520ee-153">string</span><span class="sxs-lookup"><span data-stu-id="520ee-153">String</span></span>|<span data-ttu-id="520ee-154">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="520ee-154">Key of the entity.</span></span> <span data-ttu-id="520ee-155">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-156">Version</span><span class="sxs-lookup"><span data-stu-id="520ee-156">version</span></span>|<span data-ttu-id="520ee-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520ee-157">String</span></span>|<span data-ttu-id="520ee-158">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="520ee-158">Version of the entity.</span></span> <span data-ttu-id="520ee-159">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="520ee-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="520ee-160">customSettings</span></span>|<span data-ttu-id="520ee-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="520ee-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="520ee-162">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="520ee-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="520ee-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="520ee-163">deployedAppCount</span></span>|<span data-ttu-id="520ee-164">Int32</span><span class="sxs-lookup"><span data-stu-id="520ee-164">Int32</span></span>|<span data-ttu-id="520ee-165">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="520ee-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="520ee-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="520ee-166">isAssigned</span></span>|<span data-ttu-id="520ee-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520ee-167">Boolean</span></span>|<span data-ttu-id="520ee-168">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="520ee-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="520ee-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="520ee-169">Response</span></span>
<span data-ttu-id="520ee-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="520ee-170">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="520ee-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="520ee-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="520ee-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="520ee-172">Request</span></span>
<span data-ttu-id="520ee-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="520ee-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="520ee-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="520ee-174">Response</span></span>
<span data-ttu-id="520ee-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="520ee-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```




