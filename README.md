# PatientsClinicalHistory
Progetto per l'esame di "Cloud Computing" della laurea magistrale in "Informatica".

## Spiegazione del sistema
Creazione di un sistema cloud in cui si offrono le seguenti funzionalità:

- **Funzionalità 1:** 
Un medico, un chirurgo o un infermiere carica dei dati, delle informazioni e delle cartelle cliniche dei suoi pazienti in maniera tale da poter gestire in maniera più semplice, immediata ed organizzata tutti i loro dati. 
Grazie al cloud, potrà accedere a tali dati in un qualsiasi momento e su qualsiasi dispositivo.

- **Funzionalità 2:** 
Un medico, un chirurgo o un infermiere può inserire in input dei sintomi manifestati da un suo paziente e, tramite i dati presenti nel sistema su quel paziente, è in grado di ottenere una lista di possibili cause e/o malattie grazie all'Intelligenza Artificiale.

- **Funzionalità 3:** 
Un medico, un chirurgo, un infermiere o un paziente può interagire con un chatbot in cui potrà chiedere delle informazioni su un paziente (o su se stesso se ci interagisce un paziente) e, il chatbot, grazie ai dati a sua disposizione sul paziente (o su se stesso se ci interagisce un paziente), potrà rispondergli nella maniera più accurata possibile.

- **Funzionalità 4:** 
Il sistema offrirà la funzionalità in cui un medico, un chirurgo, un infermiere o un paziente potrà inviare e ricevere delle e-mail e dei messaggi tramite whatsapp, telegram o sms e, in più, il paziente potrà ricevere delle notizie sulla struttura in cui è gestita la sua storia clinica (studio medico di famiglia, ospedale, una qualsiasi altra struttura clinica), come per esempio: delle visite gratis offerte dalla struttura, degli sconti, delle promozioni, etc.

## Servizi di Microsoft Azure che verranno utilizzati
Di seguito sono riportati i servizi che saranno utilizzati:
- **Azure Health Data Services:** archivia, gestisce e analizza in modo sicuro le cartelle cliniche dei pazienti, supportando standard sanitari come FHIR e DICOM. Consente approfondimenti in tempo reale, analisi avanzate e previsione delle malattie basata sull'Intelligenza Artificiale, garantendo la conformità alle normative sulla privacy come HIPAA e GDPR.
- **Azure Machine Learning:** utilizzata per creare e distribuire modelli predittivi per la diagnosi delle malattie in base ai sintomi dei pazienti.
- **Azure Health Bot:** utilizzata per creare un chatbot dedicato per la medicina.
- **Azure Communication Services:** utilizzata per inviare e ricevere e-mail, messaggi e sms tra medici e pazienti in modo sicuro.
- **Azure Data Factory:** utile per integrare ed elaborare i dati provenienti dalle piattaforme di messaggistica.
- **Azure Firewall, Azure VPN Gateway, Microsoft Defender for Cloud:** verranno utilizzati alcuni o tutti questi servizi per migliorare la sicurezza del sistema.
- **Azure SQL Database:** servizio che offre un database SQL per gestire i dati persistenti.

## Descrizione della struttura del progetto
- **Funzionalità 1:**
I dati di un paziente caricati saranno gestiti dal servizio "Azure Health Data Services" in maniera tale che gli attori interessati potranno visionare i dati inseriti nella maniera più semplice, immediata ed organizzata possibile. I dati verranno salvati nel DB relazionale offerto dal servizio "Azure SQL Database".

- **Funzionalità 2:**
Un modulo di Intelligenza Artificiale creato con il servizio "Azure Machine Learning" prenderà in input dei sintomi e, grazie ai dati del paziente attuali potrà ritornare in output un elenco di possibili cause e/o malattie.

- **Funzionalità 3:**
Verrà realizzato un chatbot su misura grazie al servizio "Azure Health Bot". salveremo i dati provenienti dal chatbot utili per future previsioni di possibili cause e/o malattie. I dati verranno salvati nel DB relazionale offerto dal servizio "Azure SQL Database".

- **Funzionalità 4:**
Verrà realizzato un sistema di scambio di e-mail, messaggi e sms tramite l'utilizzo del servizio "Azure Communication Services". Inoltre, tramite il servizio "Azure Data Factory" potremo salvare i dati provenienti dalle e-mail, dai messaggi, e dagli sms utili per future previsioni di possibili cause e/o malattie. I dati verranno salvati nel DB relazionale offerto dal servizio "Azure SQL Database".

- **Sicurezza del sistema:** verranno utilizzati alcuni o tutti questi servizi per migliorare la sicurezza del sistema: "Azure Firewall", "Azure VPN Gateway", "Microsoft Defender for Cloud".

## Vantaggi ottenuti utilizzando un ambiente Cloud
Grazie all'utilizzo di un ambiente cloud possiamo beneficiare dei seguenti vantaggi:
- **Accessibilità:** possiamo accedere ai servizi offerti dal cloud da un qualsiasi luogo e dispositivo con una connessione internet, favorendo il lavoro remoto e la collaborazione internazionale tra medici e pazienti.
- **Aggiornamenti, sicurezza e Manutenzione:** il provider si occuperà degli aggiornamenti, della sicurezza e della manutenzione del sistema cloud alleggerendo il carico IT interno.
- **Collaborazione Migliorata:** gli strumenti e le risorse che verranno condivise faciliteranno il lavoro di team distribuiti e, degli utenti del sistema, migliorando la comunicazione e la produttività tra di loro.

## Architettura cloud attuale del sistema
Di seguito è riportata l'architettura cloud attuale del sistema:
![Immagine architettura del progetto](/projectdocs/PatientClinicalHistorySchemes.drawio.png)










