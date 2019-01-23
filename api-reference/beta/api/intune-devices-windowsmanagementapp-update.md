---
title: WindowsManagementApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagementApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27ba9154598480972e1d7f2c9a8b5d28bb3ec4b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412408"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="b5f69-103">WindowsManagementApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b5f69-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="b5f69-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b5f69-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5f69-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5f69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5f69-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5f69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5f69-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5f69-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5f69-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5f69-108">Prerequisites</span></span>
<span data-ttu-id="b5f69-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5f69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b5f69-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5f69-111">Permission type</span></span>|<span data-ttu-id="b5f69-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5f69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5f69-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5f69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5f69-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5f69-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5f69-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5f69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5f69-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5f69-116">Not supported.</span></span>|
|<span data-ttu-id="b5f69-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5f69-117">Application</span></span>|<span data-ttu-id="b5f69-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5f69-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5f69-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5f69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="b5f69-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5f69-120">Request headers</span></span>
|<span data-ttu-id="b5f69-121">Header</span><span class="sxs-lookup"><span data-stu-id="b5f69-121">Header</span></span>|<span data-ttu-id="b5f69-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b5f69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5f69-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b5f69-123">Authorization</span></span>|<span data-ttu-id="b5f69-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5f69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5f69-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5f69-125">Accept</span></span>|<span data-ttu-id="b5f69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5f69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5f69-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5f69-127">Request body</span></span>
<span data-ttu-id="b5f69-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b5f69-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="b5f69-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5f69-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="b5f69-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5f69-130">Property</span></span>|<span data-ttu-id="b5f69-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b5f69-131">Type</span></span>|<span data-ttu-id="b5f69-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5f69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5f69-133">id</span><span class="sxs-lookup"><span data-stu-id="b5f69-133">id</span></span>|<span data-ttu-id="b5f69-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5f69-134">String</span></span>|<span data-ttu-id="b5f69-135">Eindeutiger Bezeichner für die Windows Management-app</span><span class="sxs-lookup"><span data-stu-id="b5f69-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="b5f69-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="b5f69-136">availableVersion</span></span>|<span data-ttu-id="b5f69-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5f69-137">String</span></span>|<span data-ttu-id="b5f69-138">Windows Management app verfügbare Version.</span><span class="sxs-lookup"><span data-stu-id="b5f69-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="b5f69-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5f69-139">Response</span></span>
<span data-ttu-id="b5f69-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b5f69-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5f69-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5f69-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5f69-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5f69-142">Request</span></span>
<span data-ttu-id="b5f69-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5f69-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="b5f69-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5f69-144">Response</span></span>
<span data-ttu-id="b5f69-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5f69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```




