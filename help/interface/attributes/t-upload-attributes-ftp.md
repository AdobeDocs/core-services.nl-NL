---
description: Als u niet uploadt met slepen en neerzetten, kunt u klantkenmerkgegevens via FTP uploaden naar de Experience Cloud.
keywords: Customer Attributes;core services
solution: Experience Cloud
title: 'Upload het bestand met klantkenmerkgegevens via FTP '
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Optioneel - Het gegevensbestand uploaden via FTP

Als u niet uploadt met slepen en neerzetten, kunt u klantkenmerkgegevens via FTP uploaden naar de Experience Cloud.

U kunt de gegevens uploaden nadat u een bron voor klantkenmerken en een FTP-account in de Experience Cloud hebt gemaakt. U maakt één FTP-account per kenmerkbron. De geüploade bestanden worden opgeslagen in de hoofdmap van dat account. De gegevens moeten een `.csv` indeling hebben, met een tweede `.fin` bestand dat aangeeft dat het uploaden is voltooid.

>[!IMPORTANT]
>
>Controleer de [gegevensbestandsvereisten voor het uploaden van klantkenmerken](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) voordat u het bestand uploadt.

Het uploaden van bestanden naar de FTP-site met klantkenmerken kan worden uitgevoerd via FTP of SFTP:

* U hebt een client nodig die SFTP-verbindingen ondersteunt.
* U kunt verbinding maken met SFTP via gebruikersnaam/wachtwoord of zonder wachtwoord, zoals [hier](https://docs.adobe.com/help/en/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html)wordt beschreven.

**Het gegevensbestand uploaden via FTP**

1. [Een bron voor klantkenmerken maken en het gegevensbestand uploaden...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Controleer of u bent aangemeld bij uw FTP-site op `ftp.adobe.com/<sftpname>`.

1. Klik op **[!UICONTROL Actions]** > **[!UICONTROL File Upload]**.

1. Upload een `.fin` bestand, zodat het bestand kan worden opgehaald.

   Het bestandstype `.fin` is door de gebruiker gemaakt en geeft aan dat het uploaden is voltooid. Het kan een leeg notebookbestand zijn. Als u bijvoorbeeld uploadt [!DNL crs123.csv], uploadt u ook [!DNL crs123.fin].

   Als het uploaden is voltooid, worden beide bestanden verplaatst naar een map die **verwerkt** wordt genoemd.

   Zie [Gegevensbestandsvereisten voor het uploaden van klantkenmerken](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) voor belangrijke informatie over bestandsnamen en structuur.
