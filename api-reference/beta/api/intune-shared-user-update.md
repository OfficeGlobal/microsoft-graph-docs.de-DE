---
title: Benutzer aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Benutzerobjekts aktualisieren.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcc1b23233c00af44b4566a3483a0ba263ebd6c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171092"
---
# <a name="update-user"></a><span data-ttu-id="2ccb5-103">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2ccb5-103">Update user</span></span>

> <span data-ttu-id="2ccb5-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ccb5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ccb5-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ccb5-107">Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ccb5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2ccb5-108">Prerequisites</span></span>

<span data-ttu-id="2ccb5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ccb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="2ccb5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ccb5-111">Permission type</span></span>|<span data-ttu-id="2ccb5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ccb5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ccb5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ccb5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2ccb5-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="2ccb5-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2ccb5-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ccb5-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2ccb5-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="2ccb5-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="2ccb5-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ccb5-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2ccb5-118">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="2ccb5-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2ccb5-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ccb5-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="2ccb5-120">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="2ccb5-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2ccb5-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ccb5-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ccb5-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ccb5-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ccb5-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ccb5-123">Not supported.</span></span>|
|<span data-ttu-id="2ccb5-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ccb5-124">Application</span></span>|<span data-ttu-id="2ccb5-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ccb5-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ccb5-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ccb5-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="2ccb5-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ccb5-127">Request headers</span></span>

|<span data-ttu-id="2ccb5-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2ccb5-128">Header</span></span>|<span data-ttu-id="2ccb5-129">Wert</span><span class="sxs-lookup"><span data-stu-id="2ccb5-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ccb5-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ccb5-130">Authorization</span></span>|<span data-ttu-id="2ccb5-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2ccb5-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ccb5-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2ccb5-132">Accept</span></span>|<span data-ttu-id="2ccb5-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2ccb5-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ccb5-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ccb5-134">Request body</span></span>

<span data-ttu-id="2ccb5-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune-shared-user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="2ccb5-136">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune-shared-user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="2ccb5-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ccb5-137">Property</span></span>|<span data-ttu-id="2ccb5-138">Typ</span><span class="sxs-lookup"><span data-stu-id="2ccb5-138">Type</span></span>|<span data-ttu-id="2ccb5-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ccb5-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ccb5-140">id</span><span class="sxs-lookup"><span data-stu-id="2ccb5-140">id</span></span>|<span data-ttu-id="2ccb5-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ccb5-141">String</span></span>|<span data-ttu-id="2ccb5-142">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="2ccb5-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="2ccb5-143">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="2ccb5-143">**Onboarding**</span></span>|
|<span data-ttu-id="2ccb5-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="2ccb5-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="2ccb5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2ccb5-145">Int32</span></span>|<span data-ttu-id="2ccb5-146">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="2ccb5-147">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="2ccb5-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ccb5-148">Response</span></span>

<span data-ttu-id="2ccb5-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ccb5-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ccb5-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ccb5-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ccb5-151">Request</span></span>

<span data-ttu-id="2ccb5-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="2ccb5-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ccb5-153">Response</span></span>

<span data-ttu-id="2ccb5-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ccb5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



