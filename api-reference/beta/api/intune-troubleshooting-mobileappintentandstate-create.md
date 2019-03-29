---
title: MobileAppIntentAndState erstellen
description: Erstellen eines neuen mobileAppIntentAndState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c46a998b3be6c0cc501ab040f9452281210d3df2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972207"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="76b12-103">MobileAppIntentAndState erstellen</span><span class="sxs-lookup"><span data-stu-id="76b12-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="76b12-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76b12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76b12-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="76b12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76b12-106">Erstellen eines neuen [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="76b12-106">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76b12-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="76b12-107">Prerequisites</span></span>
<span data-ttu-id="76b12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b12-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76b12-110">Permission type</span></span>|<span data-ttu-id="76b12-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76b12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76b12-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76b12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76b12-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b12-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="76b12-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76b12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76b12-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76b12-115">Not supported.</span></span>|
|<span data-ttu-id="76b12-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76b12-116">Application</span></span>|<span data-ttu-id="76b12-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76b12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76b12-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76b12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="76b12-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76b12-119">Request headers</span></span>
|<span data-ttu-id="76b12-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="76b12-120">Header</span></span>|<span data-ttu-id="76b12-121">Wert</span><span class="sxs-lookup"><span data-stu-id="76b12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76b12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76b12-122">Authorization</span></span>|<span data-ttu-id="76b12-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="76b12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76b12-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="76b12-124">Accept</span></span>|<span data-ttu-id="76b12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76b12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76b12-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76b12-126">Request body</span></span>
<span data-ttu-id="76b12-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das mobileAppIntentAndState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="76b12-127">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="76b12-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der mobileAppIntentAndState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="76b12-128">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="76b12-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76b12-129">Property</span></span>|<span data-ttu-id="76b12-130">Typ</span><span class="sxs-lookup"><span data-stu-id="76b12-130">Type</span></span>|<span data-ttu-id="76b12-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76b12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b12-132">id</span><span class="sxs-lookup"><span data-stu-id="76b12-132">id</span></span>|<span data-ttu-id="76b12-133">String</span><span class="sxs-lookup"><span data-stu-id="76b12-133">String</span></span>|<span data-ttu-id="76b12-134">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="76b12-134">UUID for the object</span></span>|
|<span data-ttu-id="76b12-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="76b12-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="76b12-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76b12-136">String</span></span>|<span data-ttu-id="76b12-137">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="76b12-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="76b12-138">userId</span><span class="sxs-lookup"><span data-stu-id="76b12-138">userId</span></span>|<span data-ttu-id="76b12-139">String</span><span class="sxs-lookup"><span data-stu-id="76b12-139">String</span></span>|<span data-ttu-id="76b12-140">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="76b12-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="76b12-141">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="76b12-141">mobileAppList</span></span>|<span data-ttu-id="76b12-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="76b12-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="76b12-143">Die Liste der Payload-und Statusinformationen für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="76b12-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="76b12-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="76b12-144">Response</span></span>
<span data-ttu-id="76b12-145">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="76b12-145">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76b12-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76b12-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="76b12-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76b12-147">Request</span></span>
<span data-ttu-id="76b12-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76b12-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76b12-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="76b12-149">Response</span></span>
<span data-ttu-id="76b12-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76b12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




