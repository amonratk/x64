# How to using auto size column of PHPExcel

## Configure

```bash
PHPExcel_Shared_Font::setAutoSizeMethod(PHPExcel_Shared_Font::AUTOSIZE_METHOD_EXACT);
```

## Identify to columns to set dimensions

Example

```bash
foreach(range('A', 'M') as $column) {
    $cellName = $column.$row;
    $objPHPExcel->getActiveSheet()->getColumnDimension($column)->setAutoSize(true);
    $cellValue = $mData->getAttributeLabel($hVariables[$nHeader-1]);
    $sheet->setCellValue($cellName, $cellValue);
    $nHeader++;
}
```