---
title: DeviceManagementExchangeOnPremisesPolicy aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementExchangeOnPremisesPolicy-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 633f1b80895bd84c27c57b5cee26aa286b1d0e49
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407207"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="14e42-103">DeviceManagementExchangeOnPremisesPolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="14e42-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="14e42-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="14e42-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14e42-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14e42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14e42-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="14e42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e42-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="14e42-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14e42-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="14e42-108">Prerequisites</span></span>
<span data-ttu-id="14e42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="14e42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="14e42-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14e42-111">Permission type</span></span>|<span data-ttu-id="14e42-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14e42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14e42-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14e42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14e42-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e42-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="14e42-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14e42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14e42-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14e42-116">Not supported.</span></span>|
|<span data-ttu-id="14e42-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14e42-117">Application</span></span>|<span data-ttu-id="14e42-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14e42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14e42-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14e42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="14e42-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14e42-120">Request headers</span></span>
|<span data-ttu-id="14e42-121">Header</span><span class="sxs-lookup"><span data-stu-id="14e42-121">Header</span></span>|<span data-ttu-id="14e42-122">Wert</span><span class="sxs-lookup"><span data-stu-id="14e42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14e42-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="14e42-123">Authorization</span></span>|<span data-ttu-id="14e42-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="14e42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14e42-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="14e42-125">Accept</span></span>|<span data-ttu-id="14e42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14e42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14e42-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14e42-127">Request body</span></span>
<span data-ttu-id="14e42-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="14e42-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="14e42-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="14e42-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="14e42-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14e42-130">Property</span></span>|<span data-ttu-id="14e42-131">Typ</span><span class="sxs-lookup"><span data-stu-id="14e42-131">Type</span></span>|<span data-ttu-id="14e42-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14e42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e42-133">id</span><span class="sxs-lookup"><span data-stu-id="14e42-133">id</span></span>|<span data-ttu-id="14e42-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14e42-134">String</span></span>|<span data-ttu-id="14e42-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="14e42-135">Not yet documented</span></span>|
|<span data-ttu-id="14e42-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="14e42-136">notificationContent</span></span>|<span data-ttu-id="14e42-137">Binär</span><span class="sxs-lookup"><span data-stu-id="14e42-137">Binary</span></span>|<span data-ttu-id="14e42-138">Der Text der Benachrichtigung, die Benutzern unter Quarantäne gestellte e-Mails durch diese Richtlinie gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="14e42-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="14e42-139">Hierbei handelt es sich um UTF8 codiert HTML-Byte-Array.</span><span class="sxs-lookup"><span data-stu-id="14e42-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="14e42-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="14e42-140">defaultAccessLevel</span></span>|[<span data-ttu-id="14e42-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="14e42-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="14e42-142">Access-Standardzustand in Exchange.</span><span class="sxs-lookup"><span data-stu-id="14e42-142">Default access state in Exchange.</span></span> <span data-ttu-id="14e42-143">Diese Regel gilt global für die gesamte Exchange-Organisation.</span><span class="sxs-lookup"><span data-stu-id="14e42-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="14e42-144">Mögliche Werte: sind `none`, `allow`, `block` und `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="14e42-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="14e42-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="14e42-145">accessRules</span></span>|<span data-ttu-id="14e42-146">[DeviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="14e42-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="14e42-147">Die Liste der Gerätezugriffs Regeln im Exchange.</span><span class="sxs-lookup"><span data-stu-id="14e42-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="14e42-148">Die Access-Regeln gelten global für die gesamte Exchange-Organisation</span><span class="sxs-lookup"><span data-stu-id="14e42-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="14e42-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="14e42-149">knownDeviceClasses</span></span>|<span data-ttu-id="14e42-150">[DeviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="14e42-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="14e42-151">Die Liste der Geräteklassen bekannt, dass Exchange</span><span class="sxs-lookup"><span data-stu-id="14e42-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="14e42-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="14e42-152">Response</span></span>
<span data-ttu-id="14e42-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="14e42-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14e42-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14e42-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="14e42-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14e42-155">Request</span></span>
<span data-ttu-id="14e42-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14e42-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14e42-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="14e42-157">Response</span></span>
<span data-ttu-id="14e42-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14e42-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




