---
title: Obtaining Information About a Parallel Port
author: windows-driver-content
description: Obtaining Information About a Parallel Port
MS-HAID:
- 'vspd\_20405e28-f051-40cf-8cd5-b2f8e0b1ff87.xml'
- 'parports.obtaining\_information\_about\_a\_parallel\_port'
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: d8ae2296-05b6-419a-93cc-00fcb12d41fe
keywords: ["parallel ports WDK , obtaining information"]
---

# Obtaining Information About a Parallel Port


## <a href="" id="ddk-obtaining-information-about-a-parallel-port-kg"></a>


Before a client uses a parallel port, it can obtain information about the following:

-   Resources used by the parallel port

-   Hardware capabilities of the parallel port

-   [Parallel port callback routines](https://msdn.microsoft.com/library/windows/hardware/ff544307) that a kernel-mode driver can use

A client uses the following internal device control requests to obtain the above information:

[**IOCTL\_INTERNAL\_GET\_PARALLEL\_PORT\_INFO**](https://msdn.microsoft.com/library/windows/hardware/ff544002)

[**IOCTL\_INTERNAL\_GET\_MORE\_PARALLEL\_PORT\_INFO**](https://msdn.microsoft.com/library/windows/hardware/ff543996)

[**IOCTL\_INTERNAL\_GET\_PARALLEL\_PNP\_INFO**](https://msdn.microsoft.com/library/windows/hardware/ff543997)

A client releases parallel port information by using an [**IOCTL\_INTERNAL\_RELEASE\_PARALLEL\_PORT\_INFO**](https://msdn.microsoft.com/library/windows/hardware/ff544047) request.

 

 


--------------------


