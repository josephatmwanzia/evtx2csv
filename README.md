# evtx2csv
Converting Windows events logs from .evtx to csv
This advances on the work of https://github.com/omerbenamram/evtx.
Specificaly
- Processes evtx files from folders
- convert directly to csv files

For instalation of the evtxd file, follow these intructions https://medium.com/@salim.y.salimov/a-hassle-free-evtx-to-json-converter-not-only-for-windows-but-linux-and-mac-os-too-82adc4d9d158

USAGE
--------------------------
python3 evtx2csv_parser.py [path_to_evtxd] [path_to_folder_wit_log_files]

Note.
1. You must install the evtxd from here https://github.com/omerbenamram/evtx/releases/download/v0.8.1/evtx_dump-v0.8.1-x86_64-unknown-linux-gnu
2. make it executable: chmod +x [file]
3. The attribute xmlns (namespace links) is discarded
4. New lines are removed from final csv as they distort otput
5. Do not open csv file directly on excel. Instead use the load data from csv option.
6. Delimiter is '|'

Happy hunting ...
