---
title: registryKeyState-Ressourcentyp
description: Enthält Informationen zu Registrierungsschlüssel Änderungen im Zusammenhang mit der Warnung und dem Prozess, der die Registrierungsschlüssel geändert hat.
localization_priority: Normal
ms.openlocfilehash: d07b0b6f502794154b400444eaf3854535e04547
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994426"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="7622a-103">registryKeyState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7622a-103">registryKeyState resource type</span></span>

<span data-ttu-id="7622a-104">Enthält Informationen zu Registrierungsschlüssel Änderungen im Zusammenhang mit der Warnung und dem Prozess, der die Registrierungsschlüssel geändert hat.</span><span class="sxs-lookup"><span data-stu-id="7622a-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="7622a-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7622a-105">Properties</span></span>

| <span data-ttu-id="7622a-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7622a-106">Property</span></span>     | <span data-ttu-id="7622a-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7622a-107">Type</span></span>        | <span data-ttu-id="7622a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7622a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7622a-109">Struktur</span><span class="sxs-lookup"><span data-stu-id="7622a-109">hive</span></span>|<span data-ttu-id="7622a-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="7622a-110">registryHive</span></span>|<span data-ttu-id="7622a-111">Eine [Windows-Registrierungsstruktur](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="7622a-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="7622a-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="7622a-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="7622a-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="7622a-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="7622a-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="7622a-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="7622a-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="7622a-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="7622a-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="7622a-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="7622a-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="7622a-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="7622a-118">HKEY_USERS\\. Standard.</span><span class="sxs-lookup"><span data-stu-id="7622a-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="7622a-119">Mögliche Werte: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="7622a-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="7622a-120">Schlüssel</span><span class="sxs-lookup"><span data-stu-id="7622a-120">key</span></span>|<span data-ttu-id="7622a-121">String</span><span class="sxs-lookup"><span data-stu-id="7622a-121">String</span></span>|<span data-ttu-id="7622a-122">Aktueller (d.h. Geänderter) Registrierungsschlüssel (schließt HIVE aus).</span><span class="sxs-lookup"><span data-stu-id="7622a-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7622a-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="7622a-123">oldKey</span></span>|<span data-ttu-id="7622a-124">String</span><span class="sxs-lookup"><span data-stu-id="7622a-124">String</span></span>|<span data-ttu-id="7622a-125">Vorheriger (d. h. vor geänderter) Registrierungsschlüssel (schließt HIVE aus).</span><span class="sxs-lookup"><span data-stu-id="7622a-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7622a-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="7622a-126">oldValueData</span></span>|<span data-ttu-id="7622a-127">String</span><span class="sxs-lookup"><span data-stu-id="7622a-127">String</span></span>|<span data-ttu-id="7622a-128">Frühere (d. h. geänderte) Registrierungsschlüssel Wertdaten (Inhalte).</span><span class="sxs-lookup"><span data-stu-id="7622a-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7622a-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="7622a-129">oldValueName</span></span>|<span data-ttu-id="7622a-130">String</span><span class="sxs-lookup"><span data-stu-id="7622a-130">String</span></span>|<span data-ttu-id="7622a-131">Vorheriger (also vor geänderter) Registrierungsschlüssel-Wertname.</span><span class="sxs-lookup"><span data-stu-id="7622a-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="7622a-132">Vorgang</span><span class="sxs-lookup"><span data-stu-id="7622a-132">operation</span></span>|<span data-ttu-id="7622a-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="7622a-133">registryOperation</span></span>|<span data-ttu-id="7622a-134">Vorgang, der den Namen und/oder Wert des Registrierungsschlüssels geändert hat.</span><span class="sxs-lookup"><span data-stu-id="7622a-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="7622a-135">Mögliche Werte sind: `unknown`, `create`, `modify` und `delete`.</span><span class="sxs-lookup"><span data-stu-id="7622a-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="7622a-136">processId</span><span class="sxs-lookup"><span data-stu-id="7622a-136">processId</span></span>|<span data-ttu-id="7622a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7622a-137">Int32</span></span>|<span data-ttu-id="7622a-138">Prozess-ID (PID) des Prozesses, der den Registrierungsschlüssel geändert hat (Prozessdetails werden in der Alert ' Processes '-Auflistung angezeigt).</span><span class="sxs-lookup"><span data-stu-id="7622a-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="7622a-139">valueData</span><span class="sxs-lookup"><span data-stu-id="7622a-139">valueData</span></span>|<span data-ttu-id="7622a-140">String</span><span class="sxs-lookup"><span data-stu-id="7622a-140">String</span></span>|<span data-ttu-id="7622a-141">Aktuelle (d.h. geänderte) Registrierungsschlüssel Wertdaten (Inhalte).</span><span class="sxs-lookup"><span data-stu-id="7622a-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7622a-142">valueName</span><span class="sxs-lookup"><span data-stu-id="7622a-142">valueName</span></span>|<span data-ttu-id="7622a-143">String</span><span class="sxs-lookup"><span data-stu-id="7622a-143">String</span></span>|<span data-ttu-id="7622a-144">Aktueller (d.h. Geänderter) Registrierungsschlüssel-Wertname</span><span class="sxs-lookup"><span data-stu-id="7622a-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="7622a-145">valueType</span><span class="sxs-lookup"><span data-stu-id="7622a-145">valueType</span></span>|<span data-ttu-id="7622a-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="7622a-146">registryValueType</span></span>|[<span data-ttu-id="7622a-147">Registrierungsschlüssel-Werttyp</span><span class="sxs-lookup"><span data-stu-id="7622a-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="7622a-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="7622a-148">REG_BINARY</span></span></li> <li><span data-ttu-id="7622a-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7622a-149">REG_DWORD</span></span></li> <li><span data-ttu-id="7622a-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7622a-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7622a-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7622a-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="7622a-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="7622a-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="7622a-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="7622a-153">REG_LINK</span></span></li> <li><span data-ttu-id="7622a-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="7622a-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="7622a-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="7622a-155">REG_NONE</span></span></li> <li><span data-ttu-id="7622a-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="7622a-156">REG_QWORD</span></span></li> <li><span data-ttu-id="7622a-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7622a-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7622a-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="7622a-158">REG_SZ</span></span></li></ul> <span data-ttu-id="7622a-159">Mögliche Werte sind: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian` und `sz`.</span><span class="sxs-lookup"><span data-stu-id="7622a-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7622a-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7622a-160">JSON representation</span></span>

<span data-ttu-id="7622a-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7622a-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
