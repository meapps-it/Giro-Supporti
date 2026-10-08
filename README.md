# GIRO SUPPORTI
PWA mobile-first senza login applicativo. Repository locale sostituibile in futuro con un adapter cloud. Dati e sequenza salvati sul dispositivo; le foto non vengono persistite. OCR Tesseract locale con modello italiano, obbligo di verifica; nessuna garanzia sulla scrittura a penna o sull'individuazione delle correzioni manoscritte. Le tappe ripetute condividono i dati MP e mantengono lo stato saltata per tappa. I giri chiusi sono modificabili, conservando la data fine e aggiornando modified. Storico visibile: oggi e 6 giorni precedenti; i dati più vecchi non vengono eliminati.

Avvio offline dopo un primo caricamento completo online. L'OCR usa asset locali pre-caricati dal service worker. Non sono presenti analytics o richieste a servizi OCR esterni. Eliminare i dati del browser elimina l'archivio personale.

Test: `node --test tests/*.test.js`. QA visuale Android e fotografie reali da effettuare sul dispositivo: nessun browser di QA disponibile nell'ambiente di creazione.
