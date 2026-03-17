graph TD
    subgraph Stage 1: The Backend Foundation
        S1[Step 1: Prove the Vault<br/>Spin up PostgreSQL via Docker & Test connection] --> S2[Step 2: Master the Engine<br/>Clean 10 rows with Python + DuckDB & Print to terminal]
        S2 --> S3[Step 3: Build the Bridge<br/>Push clean data from Python into PostgreSQL]
    end

    subgraph Stage 2: The Native Frontend
        S3 --> S4[Step 4: Draw the Glass<br/>Build empty GUI window with Qt Creator]
        S4 --> S5[Step 5: The Final Wire<br/>Connect C++ GUI to PostgreSQL and display data]
    end

    classDef backend fill:#336791,stroke:#FFE873,stroke-width:2px,color:white;
    classDef frontend fill:#41CD52,stroke:#222,stroke-width:2px,color:black;
    
    class S1,S2,S3 backend;
    class S4,S5 frontend;
