---
title: Ressourcentyp registryKeyState
description: Enthält Informationen zur Registrierung wichtige Änderungen im Zusammenhang mit der Benachrichtigung, und der Prozess, der die Registrierungsschlüssel geändert.
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017898"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="8704b-103">Ressourcentyp registryKeyState</span><span class="sxs-lookup"><span data-stu-id="8704b-103">registryKeyState resource type</span></span>

<span data-ttu-id="8704b-104">Enthält Informationen zur Registrierung wichtige Änderungen im Zusammenhang mit der Benachrichtigung, und der Prozess, der die Registrierungsschlüssel geändert.</span><span class="sxs-lookup"><span data-stu-id="8704b-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="8704b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8704b-105">Properties</span></span>

| <span data-ttu-id="8704b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8704b-106">Property</span></span>     | <span data-ttu-id="8704b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="8704b-107">Type</span></span>        | <span data-ttu-id="8704b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8704b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8704b-109">Struktur</span><span class="sxs-lookup"><span data-stu-id="8704b-109">hive</span></span>|<span data-ttu-id="8704b-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="8704b-110">registryHive</span></span>|<span data-ttu-id="8704b-111">Ein [Windows-Registrierungsstruktur](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="8704b-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="8704b-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="8704b-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="8704b-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="8704b-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="8704b-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="8704b-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="8704b-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="8704b-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="8704b-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="8704b-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="8704b-117">HKEY_LOCAL_MACHINE\SYSTEM</span><span class="sxs-lookup"><span data-stu-id="8704b-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="8704b-118">HKEY_USERS\\. Die standardmäßigen.</span><span class="sxs-lookup"><span data-stu-id="8704b-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="8704b-119">Mögliche Werte sind: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem` und `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="8704b-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="8704b-120">Key</span><span class="sxs-lookup"><span data-stu-id="8704b-120">key</span></span>|<span data-ttu-id="8704b-121">String</span><span class="sxs-lookup"><span data-stu-id="8704b-121">String</span></span>|<span data-ttu-id="8704b-122">Aktuelle (d. h. geänderten) Registrierungsschlüssel (schließt die Struktur).</span><span class="sxs-lookup"><span data-stu-id="8704b-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="8704b-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="8704b-123">oldKey</span></span>|<span data-ttu-id="8704b-124">String</span><span class="sxs-lookup"><span data-stu-id="8704b-124">String</span></span>|<span data-ttu-id="8704b-125">Frühere (d. h., bevor geändert) Registrierungsschlüssel (schließt die Struktur).</span><span class="sxs-lookup"><span data-stu-id="8704b-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="8704b-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="8704b-126">oldValueData</span></span>|<span data-ttu-id="8704b-127">String</span><span class="sxs-lookup"><span data-stu-id="8704b-127">String</span></span>|<span data-ttu-id="8704b-128">Frühere (d. h., bevor geändert) Schlüsselwert Registrierungsdaten (Inhalt).</span><span class="sxs-lookup"><span data-stu-id="8704b-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="8704b-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="8704b-129">oldValueName</span></span>|<span data-ttu-id="8704b-130">String</span><span class="sxs-lookup"><span data-stu-id="8704b-130">String</span></span>|<span data-ttu-id="8704b-131">Frühere (d. h., bevor geändert) Registrierung Schlüsselwertname.</span><span class="sxs-lookup"><span data-stu-id="8704b-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="8704b-132">Operation</span><span class="sxs-lookup"><span data-stu-id="8704b-132">operation</span></span>|<span data-ttu-id="8704b-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="8704b-133">registryOperation</span></span>|<span data-ttu-id="8704b-134">Der Vorgang, der der Name des Registrierungsschlüssels und/oder Wert geändert.</span><span class="sxs-lookup"><span data-stu-id="8704b-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="8704b-135">Mögliche Werte: sind `unknown`, `create`, `modify` und `delete`.</span><span class="sxs-lookup"><span data-stu-id="8704b-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="8704b-136">processId</span><span class="sxs-lookup"><span data-stu-id="8704b-136">processId</span></span>|<span data-ttu-id="8704b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8704b-137">Int32</span></span>|<span data-ttu-id="8704b-138">Werden Sie ID (PID) des Prozesses, der den Registrierungsschlüssel (Prozess, der in der Auflistung Warnung 'Prozesse' Details angezeigt werden) geändert.</span><span class="sxs-lookup"><span data-stu-id="8704b-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="8704b-139">valueData</span><span class="sxs-lookup"><span data-stu-id="8704b-139">valueData</span></span>|<span data-ttu-id="8704b-140">String</span><span class="sxs-lookup"><span data-stu-id="8704b-140">String</span></span>|<span data-ttu-id="8704b-141">Aktuelle (d. h. geänderten) Schlüsselwert Registrierungsdaten (Inhalt).</span><span class="sxs-lookup"><span data-stu-id="8704b-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="8704b-142">Wertname</span><span class="sxs-lookup"><span data-stu-id="8704b-142">valueName</span></span>|<span data-ttu-id="8704b-143">String</span><span class="sxs-lookup"><span data-stu-id="8704b-143">String</span></span>|<span data-ttu-id="8704b-144">Aktuelle (d. h. geänderten) Registrierung Schlüsselwertname</span><span class="sxs-lookup"><span data-stu-id="8704b-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="8704b-145">Werttyp</span><span class="sxs-lookup"><span data-stu-id="8704b-145">valueType</span></span>|<span data-ttu-id="8704b-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="8704b-146">registryValueType</span></span>|[<span data-ttu-id="8704b-147">Schlüsselwert Registrierungstyp</span><span class="sxs-lookup"><span data-stu-id="8704b-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="8704b-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="8704b-148">REG_BINARY</span></span></li> <li><span data-ttu-id="8704b-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="8704b-149">REG_DWORD</span></span></li> <li><span data-ttu-id="8704b-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="8704b-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="8704b-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="8704b-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="8704b-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="8704b-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="8704b-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="8704b-153">REG_LINK</span></span></li> <li><span data-ttu-id="8704b-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="8704b-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="8704b-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="8704b-155">REG_NONE</span></span></li> <li><span data-ttu-id="8704b-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="8704b-156">REG_QWORD</span></span></li> <li><span data-ttu-id="8704b-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="8704b-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="8704b-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="8704b-158">REG_SZ</span></span></li></ul> <span data-ttu-id="8704b-159">Mögliche Werte sind: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian` und `sz`.</span><span class="sxs-lookup"><span data-stu-id="8704b-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8704b-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8704b-160">JSON representation</span></span>

<span data-ttu-id="8704b-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8704b-161">The following is a JSON representation of the resource.</span></span>

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