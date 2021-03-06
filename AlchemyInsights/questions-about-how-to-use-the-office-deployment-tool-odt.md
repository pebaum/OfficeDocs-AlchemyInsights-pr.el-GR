---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του εργαλείου ανάπτυξης του Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010749"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Ερωτήσεις σχετικά με τον τρόπο χρήσης του εργαλείου ανάπτυξης του Office (ODT)

Κάντε λήψη του εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης της Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Μετά τη λήψη του αρχείου, εκτελέστε το εκτελέσιμο αρχείο αυτόματης εξαγωγής, το οποίο περιέχει το εκτελέσιμο αρχείο του εργαλείου ανάπτυξης του Office (setup.exe) και ένα δείγμα αρχείου ρύθμισης παραμέτρων (configuration.xml).
  
 **Για να εξαιρέσετε ή να καταργήσετε τις εφαρμογές της Microsoft 365 για εταιρικά προϊόντα από υπολογιστές-πελάτες:**
  
Κατά την εγκατάσταση των Εφαρμογών Microsoft 365 για μεγάλες επιχειρήσεις, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα. Για να το κάνετε αυτό, ακολουθήστε τα βήματα για την εγκατάσταση του Office με το ODT, αλλά συμπεριλάβετε το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων. Για παράδειγμα, αυτό το αρχείο ρύθμισης παραμέτρων εγκαθιστά όλες τις εφαρμογές του Microsoft 365 για εταιρικά προϊόντα εκτός από τον Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Επισκόπηση του εργαλείου ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

