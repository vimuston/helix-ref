# Helix reference data

GRCh38 (UCSC hg38, soft-masked) packed as 2-bit 1 Mb chunks, served by GitHub Pages for the
`helix` explorer. Each file: "REF1", u32 start, u32 length, 2-bit bases (A0 C1 G2 T3, first base in the
high bits), then N runs and soft-masked repeat runs (u32 count + u32 start/end pairs), all little-endian.
