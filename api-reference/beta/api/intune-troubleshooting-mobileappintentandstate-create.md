---
title: Erstellen von mobileAppIntentAndState
description: Erstellen eines neuen MobileAppIntentAndState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 94aeb4551fac9534cf2c88a973b0d37fd49aa048
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399822"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="fde3b-103">Erstellen von mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="fde3b-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="fde3b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fde3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fde3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fde3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fde3b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fde3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fde3b-107">Erstellen eines neuen [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fde3b-107">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fde3b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fde3b-108">Prerequisites</span></span>
<span data-ttu-id="fde3b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fde3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fde3b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fde3b-111">Permission type</span></span>|<span data-ttu-id="fde3b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fde3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fde3b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fde3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fde3b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fde3b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fde3b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fde3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fde3b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fde3b-116">Not supported.</span></span>|
|<span data-ttu-id="fde3b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fde3b-117">Application</span></span>|<span data-ttu-id="fde3b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fde3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fde3b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fde3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="fde3b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fde3b-120">Request headers</span></span>
|<span data-ttu-id="fde3b-121">Header</span><span class="sxs-lookup"><span data-stu-id="fde3b-121">Header</span></span>|<span data-ttu-id="fde3b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fde3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fde3b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fde3b-123">Authorization</span></span>|<span data-ttu-id="fde3b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fde3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fde3b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fde3b-125">Accept</span></span>|<span data-ttu-id="fde3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fde3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fde3b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fde3b-127">Request body</span></span>
<span data-ttu-id="fde3b-128">Geben Sie im Textkörper Anforderung für das Objekt MobileAppIntentAndState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fde3b-128">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="fde3b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MobileAppIntentAndState erstellen.</span><span class="sxs-lookup"><span data-stu-id="fde3b-129">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="fde3b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fde3b-130">Property</span></span>|<span data-ttu-id="fde3b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fde3b-131">Type</span></span>|<span data-ttu-id="fde3b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fde3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde3b-133">id</span><span class="sxs-lookup"><span data-stu-id="fde3b-133">id</span></span>|<span data-ttu-id="fde3b-134">String</span><span class="sxs-lookup"><span data-stu-id="fde3b-134">String</span></span>|<span data-ttu-id="fde3b-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="fde3b-135">UUID for the object</span></span>|
|<span data-ttu-id="fde3b-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fde3b-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="fde3b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fde3b-137">String</span></span>|<span data-ttu-id="fde3b-138">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="fde3b-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="fde3b-139">userId</span><span class="sxs-lookup"><span data-stu-id="fde3b-139">userId</span></span>|<span data-ttu-id="fde3b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fde3b-140">String</span></span>|<span data-ttu-id="fde3b-141">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="fde3b-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="fde3b-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="fde3b-142">mobileAppList</span></span>|<span data-ttu-id="fde3b-143">[MobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="fde3b-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="fde3b-144">Die Liste der Nutzlast Intents und Status für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fde3b-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="fde3b-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="fde3b-145">Response</span></span>
<span data-ttu-id="fde3b-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fde3b-146">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fde3b-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fde3b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="fde3b-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fde3b-148">Request</span></span>
<span data-ttu-id="fde3b-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fde3b-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fde3b-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="fde3b-150">Response</span></span>
<span data-ttu-id="fde3b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fde3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```




