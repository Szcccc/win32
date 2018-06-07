---
Description: Compares two Unicode strings.
ms.assetid: D2703180-946C-4762-AFBA-1E882B01B944
title: RtlCompareUnicodeString function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# RtlCompareUnicodeString function

Compares two Unicode strings.

## Syntax


```C++
LONG RtlCompareUnicodeString(
  _In_ PCUNICODE_STRING String1,
  _In_ PCUNICODE_STRING String2,
  _In_ BOOLEAN          CaseInSensitive
);
```



## Parameters

<dl> <dt>

*String1* \[in\]
</dt> <dd>

Pointer to the first string.

</dd> <dt>

*String2* \[in\]
</dt> <dd>

Pointer to the second string.

</dd> <dt>

*CaseInSensitive* \[in\]
</dt> <dd>

If **TRUE**, case should be ignored when doing the comparison.

</dd> </dl>

## Return value

A signed value that gives the results of the comparison:



| Return code                                                                               | Description                                     |
|-------------------------------------------------------------------------------------------|-------------------------------------------------|
| <dl> <dt>**Zero**</dt> </dl>       | *String1* equals *String2*.<br/>          |
| <dl> <dt>**&lt; Zero**</dt> </dl>  | *String1* is less than *String2*.<br/>    |
| <dl> <dt>**&gt; Zero** </dt> </dl> | *String1* is greater than *String2*.<br/> |



 

## Requirements



|                                     |                                                                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                                                                              |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                                                    |
| Target platform<br/>          | <dl> <dt>[Universal](http://go.microsoft.com/fwlink/p/?linkid=531356)</dt> </dl> |
| Header<br/>                   | <dl> <dt>Wdm.h (include Wdm.h, Ntddk.h, or Ntifs.h)</dt> </dl>                   |
| Library<br/>                  | <dl> <dt>Ntdll.lib</dt> </dl>                                                    |
| DLL<br/>                      | <dl> <dt>Ntdll.dll</dt> </dl>                                                    |



## See also

<dl> <dt>

[**RtlCompareString**](https://msdn.microsoft.com/59d023d4-a2b4-4183-9572-cb48621c76fb)
</dt> <dt>

[**RtlEqualString**](https://msdn.microsoft.com/f8244276-0cf6-4315-9f4a-85890194dad8)
</dt> </dl>

 

 



