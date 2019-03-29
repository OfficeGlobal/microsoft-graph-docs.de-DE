---
title: DeviceManagementExchangeOnPremisesPolicy aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeOnPremisesPolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80d05e29cb478071feef6152fda7af930b0b3652
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973397"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="0aafc-103">DeviceManagementExchangeOnPremisesPolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0aafc-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="0aafc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0aafc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aafc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0aafc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aafc-106">Aktualisieren der Eigenschaften eines [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0aafc-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aafc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0aafc-107">Prerequisites</span></span>
<span data-ttu-id="0aafc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aafc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aafc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0aafc-110">Permission type</span></span>|<span data-ttu-id="0aafc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0aafc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aafc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0aafc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0aafc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aafc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0aafc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0aafc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aafc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0aafc-115">Not supported.</span></span>|
|<span data-ttu-id="0aafc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0aafc-116">Application</span></span>|<span data-ttu-id="0aafc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0aafc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aafc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aafc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0aafc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0aafc-119">Request headers</span></span>
|<span data-ttu-id="0aafc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0aafc-120">Header</span></span>|<span data-ttu-id="0aafc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0aafc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aafc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aafc-122">Authorization</span></span>|<span data-ttu-id="0aafc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0aafc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aafc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0aafc-124">Accept</span></span>|<span data-ttu-id="0aafc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0aafc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aafc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0aafc-126">Request body</span></span>
<span data-ttu-id="0aafc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0aafc-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="0aafc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0aafc-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="0aafc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0aafc-129">Property</span></span>|<span data-ttu-id="0aafc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0aafc-130">Type</span></span>|<span data-ttu-id="0aafc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aafc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aafc-132">id</span><span class="sxs-lookup"><span data-stu-id="0aafc-132">id</span></span>|<span data-ttu-id="0aafc-133">String</span><span class="sxs-lookup"><span data-stu-id="0aafc-133">String</span></span>|<span data-ttu-id="0aafc-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0aafc-134">Not yet documented</span></span>|
|<span data-ttu-id="0aafc-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="0aafc-135">notificationContent</span></span>|<span data-ttu-id="0aafc-136">Binär</span><span class="sxs-lookup"><span data-stu-id="0aafc-136">Binary</span></span>|<span data-ttu-id="0aafc-137">Benachrichtigungstext, der an Benutzer gesendet wird, die von dieser Richtlinie isoliert werden.</span><span class="sxs-lookup"><span data-stu-id="0aafc-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="0aafc-138">Dies ist ein UTF8-codiertes Bytearray.</span><span class="sxs-lookup"><span data-stu-id="0aafc-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="0aafc-139">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0aafc-139">defaultAccessLevel</span></span>|[<span data-ttu-id="0aafc-140">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0aafc-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="0aafc-141">Standardzugriffsstatus in Exchange.</span><span class="sxs-lookup"><span data-stu-id="0aafc-141">Default access state in Exchange.</span></span> <span data-ttu-id="0aafc-142">Diese Regel gilt global für die gesamte Exchange-Organisation.</span><span class="sxs-lookup"><span data-stu-id="0aafc-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="0aafc-143">Mögliche Werte sind: `none`, `allow`, `block` und `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="0aafc-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="0aafc-144">accessRules</span><span class="sxs-lookup"><span data-stu-id="0aafc-144">accessRules</span></span>|<span data-ttu-id="0aafc-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0aafc-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="0aafc-146">Die Liste der Gerätezugriffsregeln in Exchange.</span><span class="sxs-lookup"><span data-stu-id="0aafc-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="0aafc-147">Die Zugriffsregeln gelten global für die gesamte Exchange-Organisation.</span><span class="sxs-lookup"><span data-stu-id="0aafc-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="0aafc-148">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="0aafc-148">knownDeviceClasses</span></span>|<span data-ttu-id="0aafc-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0aafc-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="0aafc-150">Die Liste der Geräteklassen, die Exchange bekannt ist</span><span class="sxs-lookup"><span data-stu-id="0aafc-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="0aafc-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aafc-151">Response</span></span>
<span data-ttu-id="0aafc-152">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0aafc-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aafc-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0aafc-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aafc-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aafc-154">Request</span></span>
<span data-ttu-id="0aafc-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0aafc-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0aafc-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aafc-156">Response</span></span>
<span data-ttu-id="0aafc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0aafc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```




