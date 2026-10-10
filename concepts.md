# ● Kalt — Concepts & patterns

## → event carried state transfers

The events enclose all the data for the domain, rather than serving as basic change notifications or a smaller subset of the entity. When a source system modifies data, it broadcasts an event carrying the detailed state, enabling downstream consumer systems to replicate and maintain local copies of the information. 

With all required data locally accessible, consumer services can execute processing and queries directly without making remote network calls back to the originating service, which reduces network traffic while improving performance, availability, and system decoupling.

This also ensures we never introduce 