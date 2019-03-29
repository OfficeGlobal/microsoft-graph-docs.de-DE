---
title: targetedManagedAppConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppConfiguration- Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7e811ad24c2a91f3b95ae3e6deb7e949b069035
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957168"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="3a51b-103">targetedManagedAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3a51b-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="3a51b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3a51b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a51b-105">Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)- Objekts.</span><span class="sxs-lookup"><span data-stu-id="3a51b-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a51b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3a51b-106">Prerequisites</span></span>
<span data-ttu-id="3a51b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a51b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a51b-109">Permission type</span></span>|<span data-ttu-id="3a51b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a51b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a51b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a51b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a51b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a51b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a51b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a51b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a51b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a51b-114">Not supported.</span></span>|
|<span data-ttu-id="3a51b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a51b-115">Application</span></span>|<span data-ttu-id="3a51b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a51b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a51b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a51b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3a51b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a51b-118">Request headers</span></span>
|<span data-ttu-id="3a51b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3a51b-119">Header</span></span>|<span data-ttu-id="3a51b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3a51b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a51b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a51b-121">Authorization</span></span>|<span data-ttu-id="3a51b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3a51b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a51b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3a51b-123">Accept</span></span>|<span data-ttu-id="3a51b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a51b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a51b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a51b-125">Request body</span></span>
<span data-ttu-id="3a51b-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3a51b-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="3a51b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3a51b-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="3a51b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a51b-128">Property</span></span>|<span data-ttu-id="3a51b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3a51b-129">Type</span></span>|<span data-ttu-id="3a51b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a51b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a51b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="3a51b-131">displayName</span></span>|<span data-ttu-id="3a51b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a51b-132">String</span></span>|<span data-ttu-id="3a51b-133">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a51b-133">Policy display name.</span></span> <span data-ttu-id="3a51b-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a51b-135">description</span><span class="sxs-lookup"><span data-stu-id="3a51b-135">description</span></span>|<span data-ttu-id="3a51b-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a51b-136">String</span></span>|<span data-ttu-id="3a51b-137">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a51b-137">The policy's description.</span></span> <span data-ttu-id="3a51b-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a51b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a51b-139">createdDateTime</span></span>|<span data-ttu-id="3a51b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a51b-140">DateTimeOffset</span></span>|<span data-ttu-id="3a51b-141">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a51b-141">The date and time the policy was created.</span></span> <span data-ttu-id="3a51b-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a51b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a51b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3a51b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a51b-144">DateTimeOffset</span></span>|<span data-ttu-id="3a51b-145">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a51b-145">Last time the policy was modified.</span></span> <span data-ttu-id="3a51b-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a51b-147">id</span><span class="sxs-lookup"><span data-stu-id="3a51b-147">id</span></span>|<span data-ttu-id="3a51b-148">String</span><span class="sxs-lookup"><span data-stu-id="3a51b-148">String</span></span>|<span data-ttu-id="3a51b-149">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3a51b-149">Key of the entity.</span></span> <span data-ttu-id="3a51b-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a51b-151">Version</span><span class="sxs-lookup"><span data-stu-id="3a51b-151">version</span></span>|<span data-ttu-id="3a51b-152">String</span><span class="sxs-lookup"><span data-stu-id="3a51b-152">String</span></span>|<span data-ttu-id="3a51b-153">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="3a51b-153">Version of the entity.</span></span> <span data-ttu-id="3a51b-154">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a51b-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="3a51b-155">customSettings</span></span>|<span data-ttu-id="3a51b-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3a51b-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3a51b-157">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a51b-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="3a51b-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="3a51b-158">deployedAppCount</span></span>|<span data-ttu-id="3a51b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3a51b-159">Int32</span></span>|<span data-ttu-id="3a51b-160">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3a51b-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="3a51b-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3a51b-161">isAssigned</span></span>|<span data-ttu-id="3a51b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a51b-162">Boolean</span></span>|<span data-ttu-id="3a51b-163">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3a51b-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="3a51b-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a51b-164">Response</span></span>
<span data-ttu-id="3a51b-165">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a51b-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a51b-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a51b-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a51b-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a51b-167">Request</span></span>
<span data-ttu-id="3a51b-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a51b-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="3a51b-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a51b-169">Response</span></span>
<span data-ttu-id="3a51b-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a51b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



