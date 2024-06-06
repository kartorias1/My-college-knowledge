In module declaration, using parameter `OUTPUT_FILE` instead of `INFILE` in the document.

### Header data for bmp image
There is no **BMP_header** and **out_BMP** variable, assume **BMP_Header** is an array of 54 elements sized 8-bit.
```verilog
reg [7:0] BMP_header[0:BMP_HEADER_NUM];
```
and the writing to output file using out_BMP variable will be replaced from
```verilog

```