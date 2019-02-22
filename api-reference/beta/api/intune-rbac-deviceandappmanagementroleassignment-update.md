---
title: DeviceAndAppManagementRoleAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79565b8461f57b7abab761981903b24b98a5f692
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163511"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="87bdc-103">DeviceAndAppManagementRoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="87bdc-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="87bdc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87bdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87bdc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="87bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87bdc-106">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="87bdc-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87bdc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87bdc-107">Prerequisites</span></span>
<span data-ttu-id="87bdc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87bdc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87bdc-110">Permission type</span></span>|<span data-ttu-id="87bdc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87bdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87bdc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87bdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87bdc-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87bdc-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="87bdc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87bdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87bdc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87bdc-115">Not supported.</span></span>|
|<span data-ttu-id="87bdc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87bdc-116">Application</span></span>|<span data-ttu-id="87bdc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87bdc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87bdc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87bdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="87bdc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87bdc-119">Request headers</span></span>
|<span data-ttu-id="87bdc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87bdc-120">Header</span></span>|<span data-ttu-id="87bdc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="87bdc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87bdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87bdc-122">Authorization</span></span>|<span data-ttu-id="87bdc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87bdc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87bdc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="87bdc-124">Accept</span></span>|<span data-ttu-id="87bdc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87bdc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87bdc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87bdc-126">Request body</span></span>
<span data-ttu-id="87bdc-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="87bdc-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="87bdc-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="87bdc-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="87bdc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87bdc-129">Property</span></span>|<span data-ttu-id="87bdc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="87bdc-130">Type</span></span>|<span data-ttu-id="87bdc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87bdc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87bdc-132">id</span><span class="sxs-lookup"><span data-stu-id="87bdc-132">id</span></span>|<span data-ttu-id="87bdc-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87bdc-133">String</span></span>|<span data-ttu-id="87bdc-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="87bdc-134">Key of the entity.</span></span> <span data-ttu-id="87bdc-135">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="87bdc-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="87bdc-136">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="87bdc-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="87bdc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="87bdc-137">displayName</span></span>|<span data-ttu-id="87bdc-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87bdc-138">String</span></span>|<span data-ttu-id="87bdc-139">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="87bdc-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="87bdc-140">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="87bdc-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="87bdc-141">description</span><span class="sxs-lookup"><span data-stu-id="87bdc-141">description</span></span>|<span data-ttu-id="87bdc-142">String</span><span class="sxs-lookup"><span data-stu-id="87bdc-142">String</span></span>|<span data-ttu-id="87bdc-143">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="87bdc-143">Description of the Role Assignment.</span></span> <span data-ttu-id="87bdc-144">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="87bdc-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="87bdc-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="87bdc-145">scopeMembers</span></span>|<span data-ttu-id="87bdc-146">String collection</span><span class="sxs-lookup"><span data-stu-id="87bdc-146">String collection</span></span>|<span data-ttu-id="87bdc-147">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="87bdc-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="87bdc-148">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="87bdc-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="87bdc-149">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="87bdc-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="87bdc-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="87bdc-150">scopeType</span></span>|[<span data-ttu-id="87bdc-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="87bdc-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="87bdc-152">Gibt den Typ des Bereichs für eine Rollenzuweisung an.</span><span class="sxs-lookup"><span data-stu-id="87bdc-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="87bdc-153">Der Standardtyp "ResourceScope" ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="87bdc-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="87bdc-154">Für "allDevices", "AllLicensedUsers" und "AllDevicesAndLicensedUsers" sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="87bdc-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="87bdc-155">Von [RoleAssignment](../resources/intune-rbac-roleassignment.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="87bdc-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="87bdc-156">Mögliche Werte: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="87bdc-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="87bdc-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="87bdc-157">resourceScopes</span></span>|<span data-ttu-id="87bdc-158">String collection</span><span class="sxs-lookup"><span data-stu-id="87bdc-158">String collection</span></span>|<span data-ttu-id="87bdc-159">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="87bdc-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="87bdc-160">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="87bdc-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="87bdc-161">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="87bdc-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="87bdc-162">members</span><span class="sxs-lookup"><span data-stu-id="87bdc-162">members</span></span>|<span data-ttu-id="87bdc-163">String collection</span><span class="sxs-lookup"><span data-stu-id="87bdc-163">String collection</span></span>|<span data-ttu-id="87bdc-164">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="87bdc-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="87bdc-165">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="87bdc-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="87bdc-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="87bdc-166">Response</span></span>
<span data-ttu-id="87bdc-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="87bdc-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87bdc-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87bdc-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="87bdc-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87bdc-169">Request</span></span>
<span data-ttu-id="87bdc-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87bdc-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="87bdc-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="87bdc-171">Response</span></span>
<span data-ttu-id="87bdc-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87bdc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```




