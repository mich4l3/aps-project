Applied Cryptography & Blockchain: Self-Sovereign Identity (Erasmus+)

Descrizione del Progetto

Questo repository contiene il documento di progettazione e l'analisi di un sistema crittografico applicato, sviluppato per il corso di "Algoritmi e Protocolli per la Sicurezza" (Laurea Magistrale in Ingegneria Informatica, Università degli Studi di Salerno, A.A. 2024/2025).

Il progetto propone un'infrastruttura basata su Distributed Ledger Technology (DLT) per la gestione sicura e decentralizzata delle identità degli studenti all'interno del programma Erasmus+, adottando il paradigma della Self-Sovereign Identity (SSI).

Obiettivi e Contesto
L'obiettivo dello studio è superare le criticità legate ai tradizionali sistemi di gestione centralizzata delle identità (single point of failure, rischi per la privacy). La soluzione progettata restituisce all'utente il controllo esclusivo sui propri dati personali, fornendo alle università un meccanismo crittograficamente sicuro per verificare l'autenticità e l'integrità delle informazioni accademiche senza intermediali centrali.

Architettura e Tecnologie Implementate

Il sistema si fonda su tre pilastri tecnologici:

Distributed Ledger Technology (DLT / Blockchain)

Impiego di un'architettura decentralizzata (ispirata a modelli come Hyperledger) per garantire l'immutabilità dei registri e la trasparenza delle transazioni di validazione, eliminando la necessità di un'autorità centrale garante.

Merkle Trees e Verifiche Crittografiche

Progettazione di strutture dati basate su alberi di Merkle per assicurare l'integrità delle informazioni. Questo approccio permette la verifica efficiente di porzioni specifiche di dati (es. il superamento di un esame) senza dover esporre l'intero transcript dello studente, garantendo la minimizzazione dei dati.

Integrazione Hardware Wallet

Modellazione dell'uso di dispositivi fisici sicuri (Hardware Wallet) affidati agli studenti. I dispositivi sono preposti alla generazione, custodia e isolamento delle chiavi crittografiche private, fungendo da root of trust per l'autenticazione forte e garantendo la non-ripudiabilità delle operazioni.

Proprietà di Sicurezza Garantite

L'infrastruttura proposta è stata modellata per soddisfare i seguenti requisiti fondamentali:

Confidenzialità e Privacy: I dati sensibili non vengono registrati in chiaro sulla DLT, ma gestiti tramite proof crittografiche.

Integrità: Impossibilità di alterazione dei dati accademici retroattiva.

Autenticazione e Non-Ripudio: Garantiti dalla firma digitale apposta tramite l'elemento sicuro dell'Hardware Wallet.

Documentazione

L'analisi completa del threat model, la definizione degli attori, i requisiti architetturali e le valutazioni sulle prestazioni e limitazioni del sistema sono dettagliati nel file principale:
ProjectWork_ImparatoPenna_Group23.pdf

Autori: Gabriele Imparato, Michele Penna
