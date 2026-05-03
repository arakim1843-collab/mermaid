graph TD
    %% Definisi Gaya Visual untuk Kotak Variabel
    classDef independen fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,rx:5,ry:5,color:#000;
    classDef dependen fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,rx:5,ry:5,color:#000;

    %% Kotak Variabel Independen (X)
    subgraph "Variabel Independen (X)"
        X1[<b>Manajemen Waktu (X1)</b><br/>- Perencanaan<br/>- Skala Prioritas<br/>- Penjadwalan]:::independen
        
        X2[<b>Tingkat Stres (X2)</b><br/>- Tuntutan Peran Ganda<br/>- Tekanan Waktu<br/>- Gejala Psikologis/Fisik]:::independen
    end

    %% Kotak Variabel Dependen (Y)
    subgraph "Variabel Dependen (Y)"
        Y[<b>Produktivitas Kerja (Y)</b><br/>- Kualitas Output<br/>- Kuantitas Output<br/>- Efisiensi Waktu]:::dependen
    end

    %% Hubungan Hipotesis (Panah)
    X1 -- "H1 (+)" --> Y
    X2 -- "H2 (-)" --> Y
    
    %% Garis Simultan
    (X1) -.- (X2)
    
    %% Keterangan di tengah untuk Simultan
    Simultan{H3}
    X1 -.-> Simultan
    X2 -.-> Simultan
    Simultan ==> Y
