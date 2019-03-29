---
title: DeviceAndAppManagementRoleAssignment erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 047eb5fd57214d9f30c193e6fd51d6cd1643eac8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964724"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="b5da4-103">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="b5da4-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="b5da4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5da4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5da4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b5da4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5da4-106">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5da4-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5da4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5da4-107">Prerequisites</span></span>
<span data-ttu-id="b5da4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5da4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5da4-110">Permission type</span></span>|<span data-ttu-id="b5da4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5da4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5da4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5da4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5da4-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5da4-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b5da4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5da4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5da4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5da4-115">Not supported.</span></span>|
|<span data-ttu-id="b5da4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5da4-116">Application</span></span>|<span data-ttu-id="b5da4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5da4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5da4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5da4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b5da4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5da4-119">Request headers</span></span>
|<span data-ttu-id="b5da4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b5da4-120">Header</span></span>|<span data-ttu-id="b5da4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b5da4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5da4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5da4-122">Authorization</span></span>|<span data-ttu-id="b5da4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5da4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5da4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5da4-124">Accept</span></span>|<span data-ttu-id="b5da4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5da4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5da4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5da4-126">Request body</span></span>
<span data-ttu-id="b5da4-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="b5da4-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="b5da4-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5da4-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="b5da4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5da4-129">Property</span></span>|<span data-ttu-id="b5da4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b5da4-130">Type</span></span>|<span data-ttu-id="b5da4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5da4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5da4-132">id</span><span class="sxs-lookup"><span data-stu-id="b5da4-132">id</span></span>|<span data-ttu-id="b5da4-133">String</span><span class="sxs-lookup"><span data-stu-id="b5da4-133">String</span></span>|<span data-ttu-id="b5da4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b5da4-134">Key of the entity.</span></span> <span data-ttu-id="b5da4-135">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="b5da4-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="b5da4-136">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5da4-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b5da4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b5da4-137">displayName</span></span>|<span data-ttu-id="b5da4-138">String</span><span class="sxs-lookup"><span data-stu-id="b5da4-138">String</span></span>|<span data-ttu-id="b5da4-139">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b5da4-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="b5da4-140">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5da4-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b5da4-141">description</span><span class="sxs-lookup"><span data-stu-id="b5da4-141">description</span></span>|<span data-ttu-id="b5da4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5da4-142">String</span></span>|<span data-ttu-id="b5da4-143">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b5da4-143">Description of the Role Assignment.</span></span> <span data-ttu-id="b5da4-144">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5da4-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b5da4-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="b5da4-145">scopeMembers</span></span>|<span data-ttu-id="b5da4-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b5da4-146">String collection</span></span>|<span data-ttu-id="b5da4-147">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b5da4-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b5da4-148">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5da4-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b5da4-149">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5da4-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b5da4-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="b5da4-150">scopeType</span></span>|[<span data-ttu-id="b5da4-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="b5da4-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="b5da4-152">Gibt den Typ des Bereichs für eine Rollenzuweisung an.</span><span class="sxs-lookup"><span data-stu-id="b5da4-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="b5da4-153">Der Standardtyp "ResourceScope" ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="b5da4-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="b5da4-154">Für "allDevices", "AllLicensedUsers" und "AllDevicesAndLicensedUsers" sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="b5da4-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="b5da4-155">Von [RoleAssignment](../resources/intune-rbac-roleassignment.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b5da4-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="b5da4-156">Mögliche Werte sind: `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="b5da4-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="b5da4-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b5da4-157">resourceScopes</span></span>|<span data-ttu-id="b5da4-158">String collection</span><span class="sxs-lookup"><span data-stu-id="b5da4-158">String collection</span></span>|<span data-ttu-id="b5da4-159">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b5da4-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b5da4-160">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5da4-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b5da4-161">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5da4-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b5da4-162">members</span><span class="sxs-lookup"><span data-stu-id="b5da4-162">members</span></span>|<span data-ttu-id="b5da4-163">String collection</span><span class="sxs-lookup"><span data-stu-id="b5da4-163">String collection</span></span>|<span data-ttu-id="b5da4-164">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b5da4-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="b5da4-165">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5da4-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b5da4-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5da4-166">Response</span></span>
<span data-ttu-id="b5da4-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b5da4-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5da4-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5da4-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5da4-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5da4-169">Request</span></span>
<span data-ttu-id="b5da4-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5da4-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
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

### <a name="response"></a><span data-ttu-id="b5da4-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5da4-171">Response</span></span>
<span data-ttu-id="b5da4-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5da4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




